---
name: Check authorization before reading a client record
description: Use the Ons Autorisatie scope and clearance operations to confirm a user may see a client before fetching any dossier data.
api: openapi/nedap-ons-authorization-openapi-original.json
generated: '2026-09-02'
method: generated
source: https://ons-api.nl/english/authorization/UsingAuthorizationAPIs.html
operations:
  - scopeForUser
  - scopeForEmployee
  - clearanceForUser
  - clearanceForEmployee
  - ClientAPI.byId
---

# Check authorization before reading a client record

Your certificate authenticates the **connector**, not the person on whose behalf it is
acting. Ons has its own rights model — Ons Autorisatie — and it is your job to consult
it. This is a care record; reading a client a user is not entitled to see is a real
disclosure, not a 403 you can retry past.

Run one of these two operations **before** any dossier read, then carry the acting user
through `X-Cupido-User-Name` / `X-Cupido-Active-Identity` on the fetch itself.

## One client: `clearanceForUser` / `clearanceForEmployee`

```
GET /v0/authorization/clearance_for_user?user_id=123&client_id=456&right=ClientReportsView
GET /v0/authorization/clearance_for_employee?employee_id=123&client_id=456&right=ClientReportsView
```

Returns a single field `active`. Proceed only when it is `true`.

## Many clients: `scopeForUser` / `scopeForEmployee`

```
GET /v0/authorization/scope_for_user?user_id=123&right=ClientReportsView
GET /v0/authorization/scope_for_employee?employee_id=123&right=ClientReportsView
```

Returns:

- `all` — boolean; `true` means every client is in scope for that right.
- `clientIds` — the explicit list; empty when `all` is `true`.

Filter your own result set against this. Do not fetch first and filter after.

## Then read

- `ClientAPI.byId` — `GET /v0/administration/clients/{id}`
- `ClientAPI.byBSN` — `GET /v0/administration/clients/by_bsn` (BSN is a Dutch citizen
  service number; treat it as the most sensitive field in the record)
- `dossier.ReportAPI.searchByClient` —
  `GET /v0/administration/dossier/reports/search_by_client`

## Failure modes worth knowing

- A right that does not exist, **or a right not linked to your connector's version**,
  returns `404` — not `403`. Do not read a 404 here as "no permission"; check the
  connector configuration in the Dashboard.
- `401` means insufficient rights on the API call itself; `403` means authentication
  failed (usually a certificate/environment mismatch).
- Request only the fields you need. Nedap publishes a data-minimisation guide because
  narrowing the request is a legal obligation in Dutch care, not an optimisation.
