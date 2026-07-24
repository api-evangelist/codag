---
name: Provision and rotate Codag org API keys
description: >-
  Create, list, and revoke the org-scoped API tokens that authenticate calls to
  the Codag compaction API, working against the caller's current org.
api: openapi/codag-openapi-original.json
operations:
  - get_current_org_api_org_get
  - list_current_org_keys_api_org_keys_get
  - create_current_org_key_api_org_keys_post
  - revoke_current_org_key_api_org_keys__key_id__delete
---

# Provision and rotate Codag org API keys

API tokens are scoped to an org. Use these operations to mint the Bearer token
used by `POST /v1/compact` and to rotate it safely.

## Steps

1. **Confirm the org.** Call `get_current_org_api_org_get` (`GET /api/org`) to see
   the org the session is bound to.

2. **List existing keys.** `list_current_org_keys_api_org_keys_get`
   (`GET /api/org/keys`).

3. **Create a key.** `create_current_org_key_api_org_keys_post`
   (`POST /api/org/keys`) with a `CreateKeyRequest` body (`{ "name": "<label>" }`,
   1-64 chars). Capture the returned token — it authenticates as
   `Authorization: Bearer <api-token>`.

4. **Rotate / revoke.** Revoke a compromised or retired key with
   `revoke_current_org_key_api_org_keys__key_id__delete`
   (`DELETE /api/org/keys/{key_id}`). Rotate by creating a new key, cutting traffic
   over, then revoking the old one.

## Rules
- All calls require an authenticated session (org membership); see
  `authentication/codag-authentication.yml`.
- Slug-addressed equivalents exist for managing a specific org:
  `create_key_api_orgs__slug__keys_post`, `revoke_key_api_orgs__slug__keys__key_id__delete`.
- Validation failures return HTTP 422 (`errors/codag-problem-types.yml`).
