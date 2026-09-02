---
name: Keep a dataset in sync with Ons API webhooks
description: Bulk-load once from the stream endpoints, then stay current with HMAC-verified webhook notifications, handling out-of-order delivery, the 24-hour redelivery window, and event loops.
api: openapi/nedap-ons-webhooks-openapi-original.yml
generated: '2026-09-02'
method: generated
source: https://ons-api.nl/english/technical/Webhooks.html
operations:
  - ClientAPI.streamAll
  - ClientAPI.streamUpdates
  - ClientAPI.streamDeletes
  - EmployeeAPI.streamAll
  - EmployeeAPI.streamUpdates
  - EmployeeAPI.streamDeletes
  - dossier.ReportAPI.streamAll
  - dossier.ReportAPI.streamUpdates
---

# Keep a dataset in sync with Ons API webhooks

The documented pattern is: **one bulk fetch, then subscribe.** Polling is the fallback
and always leaves you an interval behind.

## 1. Bulk load

```
GET /v0/xstream/clients/data      # ClientAPI.streamAll
GET /v0/xstream/employees/data    # EmployeeAPI.streamAll
GET /v0/xstream/reports/data      # dossier.ReportAPI.streamAll
```

These stream `application/x-ndjson`. Read them line by line; do not buffer the whole
body.

## 2. Subscribe

1. Generate a secret on the connector page in the Ons API Dashboard.
2. Stand up a **POST** endpoint over HTTPS. Register three URLs — development, staging
   and production. All versions of your connector share them; any finer routing is
   yours to do.
3. Select the Model + event-type combinations you need. Your selections are reviewed
   before the connector is promoted to the next stage, so ask for what you will use.
4. Allow up to **5 minutes** after saving before subscriptions reliably start or stop.
   Events only flow from customer environments with an active certificate.

## 3. Verify every notification

Nedap signs each POST with `X-Signature-SHA512` — an HMAC-SHA512 of the request payload
keyed on your secret.

- Correct HMAC → answer **200**.
- Incorrect HMAC → answer **401**.

At configuration time Nedap sends **two NOP events**, one correctly signed and one
deliberately wrong. If you answer 200 to both, you have not implemented verification.

## 4. Answer fast, process later

Anything that does not return 200 within **3 seconds** is a failed delivery. Accept,
enqueue, return 200, and handle in a separate process. Plan for **hundreds of events per
second** during bulk corrections, imports, redelivery, or catch-up after downtime.

## 5. What is in the notification

```json
{ "customerCode": "TE1002", "modelType": "client", "eventType": "UPDATE",
  "id": 4711, "timestamp": "2024-08-22T10:08:11+02:00", "amountOfRetries": 0 }
```

For CREATE/UPDATE/DELETE you get an id and nothing else — **fetch the resource back**
through the REST API to learn what changed. For CUSTOM events read the identifier from
`payload`; the top-level `id` on custom events is deprecated and is removed after
**2027-03-01**.

## 6. Assume disorder

Delivery order is **not** guaranteed. You will see an UPDATE for a client whose CREATE
has not arrived. The service runs multiple instances that prefetch in batches, and a
retried notification can land after a later one. Make your handler idempotent on
`modelType` + `id`, and treat any event as "go and re-read this record".

## 7. Recovery has a 24-hour window

Failed deliveries are **not retried automatically**. They are stored for **24 hours**,
capped at 1,000,000 events, then discarded.

```
PUT /webhooks/redeliver     # empty body, connector certificate, per stage
```

triggers redelivery of everything missed for your connector. If your endpoint is down
longer than 24 hours, those notifications are gone — build a resynchronisation path
(re-run step 1) rather than assuming you can catch up.

## 8. Do not create an event loop

If you respond to a notification by writing that same record back, you will receive
another event for it. Two integrations can trigger each other indefinitely. **Detect
that nothing actually changed and skip the write.** Nedap documents this failure mode
explicitly because it happens.
