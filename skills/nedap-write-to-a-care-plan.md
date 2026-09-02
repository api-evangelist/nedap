---
name: Write to a client care plan safely
description: Create, activate and archive a care plan, with the retry and reversibility caveats that apply to every write on Ons API.
api: openapi/nedap-ons-openapi-original.json
generated: '2026-09-02'
method: generated
source: openapi/nedap-ons-openapi-original.json
operations:
  - dossier.CarePlanAPI.byClientId
  - dossier.CarePlanAPI.draftCarePlanByClientId
  - dossier.CarePlanAPI.newDraft
  - dossier.CarePlanAPI.create
  - dossier.CarePlanAPI.update
  - dossier.CarePlanAPI.activate
  - dossier.CarePlanAPI.archive
  - dossier.CarePlanAPI.activeCarePlanByClientId
  - dossier.CarePlanAPI.delete
---

# Write to a client care plan safely

Read `skills/nedap-authorize-before-reading-a-client.md` first — this flow writes to a
live care record.

## Read the current state

```
GET /v0/administration/dossier/care_plans/by_client/{client_id}          # byClientId
GET /v0/administration/dossier/care_plans/by_client/{client_id}/active   # activeCarePlanByClientId
GET /v0/administration/dossier/care_plans/by_client/{client_id}/draft    # draftCarePlanByClientId
```

A client has at most one active plan and at most one draft. Check for an existing draft
before creating another.

## Draft, edit, activate

```
POST /v0/administration/dossier/care_plans/by_client/{client_id}/new   # newDraft
PUT  /v0/administration/dossier/care_plans/{id}                        # update
POST /v0/administration/dossier/care_plans/{id}/activate               # activate
```

`dossier.CarePlanAPI.create` (`POST /v0/administration/dossier/care_plans`) creates a
plan directly; prefer `newDraft` when a client-scoped draft is what you mean.

## Retiring a plan

```
POST   /v0/administration/dossier/care_plans/{id}/archive   # archive
DELETE /v0/administration/dossier/care_plans/{id}           # delete
```

Prefer `archive`. `delete` removes the plan.

## The three caveats that apply to every write on this API

1. **No idempotency.** There is no `Idempotency-Key` header, parameter or convention
   anywhere in the 926-operation specification or the docs. If a POST times out you do
   not know whether it landed. **Re-read before you re-send** — `activeCarePlanByClientId`
   or `draftCarePlanByClientId` will tell you. A blind retry can duplicate a plan. A
   `409 Conflict` ("the given resource already exists or was changed by another call")
   is the only guard the API offers.
2. **No dry run.** Nothing on this API previews a write. Rehearse against
   `https://api-development.ons.io` with the fictional dataset and certificate customer
   code `TE1002` before touching staging or production.
3. **No documented reversal.** Nedap publishes no cancel, undo, restore or rollback
   operation and no window inside which a write can be taken back. `archive` moves a
   plan out of the active view — and archived documents stay readable, as
   `DocumentAPI.documentsByClientInPeriodIncludeArchived` shows — but **no un-archive
   operation is published and no retention period is stated.** Treat every write here as
   final from the API's point of view; recovery, if any, is a support ticket at
   <https://support.nedap-ons.nl/support/tickets>.

## Errors you will actually see

- `400` with an `ErrorResponse` — `errorResponseEntries[] { field, value, message }`.
- `404` — the plan or client does not exist, **or** the right is not linked to your
  connector version.
- `409` — someone else changed it, or it already exists.
- `429` — you exceeded 4 concurrent requests on this certificate. No `Retry-After` and
  no rate-limit headers are published; back off on your own schedule.
