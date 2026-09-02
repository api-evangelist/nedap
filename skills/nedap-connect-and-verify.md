---
name: Connect to Nedap Ons API and verify the certificate
description: Establish and prove a mutual-TLS connection to the right Ons environment before writing any integration code.
api: openapi/nedap-ons-openapi-original.json
generated: '2026-09-02'
method: generated
source: https://ons-api.nl/english/technical/Certificate_requirements.html
operations: []
---

# Connect to Nedap Ons API and verify the certificate

Ons API is mutual-TLS only. There is no API key, no bearer token and no OAuth flow. You
cannot obtain a credential yourself — a human completes an intake, has the connector
reviewed, submits a CSR, and receives a signed PEM back. Do not attempt to "sign up".

## Before you can call anything

1. An intake is submitted at <https://api-dashboard.ons.io/intake> and the connector is
   registered.
2. Generate a CSR locally. Key length **at least 4096 bits**. `CN`, `OU`, `O`, `L`, `ST`,
   `C` and email must all be filled in, and the CN must be
   `{technical_name_connector}-{customer_code}-{identification}` — for development the
   customer code is `TE1002`, e.g. `hr_integration-TE1002-free_text`.
   ```
   openssl req -out my_connector-TE1002-example.csr -new -newkey rsa:4096 -nodes \
     -keyout my_connector-TE1002-example.key
   ```
3. Upload the CSR in the Ons API Dashboard; a signed PEM comes back.
4. **Never share the `.key` file, including with Nedap.** If it is ever exposed, disable
   the certificate in the Dashboard and tell Nedap.

## Pick the right host

| Environment | Host | Data |
|---|---|---|
| DEVELOPMENT | `https://api-development.ons.io` | fictional, customer code `TE1002` |
| STAGING | `https://api-staging.ons.io` | a customer's test environment |
| PRODUCTION | `https://api.ons.io` | live care records |

A certificate is bound to one environment. Presenting a development certificate against
production returns **403**, not a helpful error.

## Prove the connection first

`GET /ping` is the only endpoint outside the `/v0/` prefix and returns `text/plain`.

```
GET https://api-development.ons.io/ping
```

- `200` — the certificate works for this environment.
- `403` — the certificate does not work with this URL.
- `495` — the certificate is invalid: expired, or not signed by the correct CA.

Do not proceed to any `/v0/` call until `/ping` returns 200.

## Transport requirements

- TLS 1.2 minimum; your client **must** send the SNI extension.
- Ciphers are restricted to eight suites (ECDHE/DHE with AES-GCM or CHACHA20-POLY1305).
- If your stack needs the full chain, fetch the environment's chain from
  `https://ons-api.nl/assets/{production,staging,development}-chain.pem`.
- On Windows, use a recent curl — 7.55.1 mishandles client certificates.

## Headers on every subsequent call

- `Accept: application/json` is **required**. A mismatch returns 406. Since mid-2024 XML
  is refused even when explicitly requested.
- `Content-Type: application/json` on POST and PUT.
- `User-Agent: connector/1.1+http://your-domain.com` — optional, but it is the only way
  Nedap can identify your traffic when something goes wrong, and there is no request-id
  header to correlate on instead.
