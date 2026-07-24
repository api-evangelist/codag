---
name: Compress logs for an AI agent with Codag
description: >-
  Take a raw, oversized log dump and get back only the lines that matter as
  schema-valid JSON with real line numbers, so a coding agent can debug at a
  fraction of the tokens. Uses the free (no-auth) path or the authenticated Pro path.
api: openapi/codag-openapi-original.json
operations:
  - free_compact_endpoint_v1_free_compact_post
  - compact_endpoint_v1_compact_post
  - anonymous_token_endpoint_v1_anonymous_token_post
  - whoami_endpoint_v1_whoami_get
---

# Compress logs for an AI agent with Codag

Codag turns a huge log stream into just the lines that matter — ranked patterns,
each pointing at a real line number — so an agent answers from evidence without
exhausting its context window.

## Steps

1. **Pick a path.**
   - No account / quick trial: call `free_compact_endpoint_v1_free_compact_post`
     (`POST /v1/free/compact`) — deterministic drain, no auth (20 MB/mo free tier).
   - Authenticated / inference (Pro): use `compact_endpoint_v1_compact_post`
     (`POST /v1/compact`) with `Authorization: Bearer <api-token>`.
   - For anonymous authenticated use, first mint a token with
     `anonymous_token_endpoint_v1_anonymous_token_post` (`POST /v1/anonymous/token`).

2. **Send the logs.** POST a JSON body of raw log lines (the `lines` array; each
   line up to 262,144 chars, up to 1,000,000 lines) plus optional `service` and
   `source` for per-service breakdowns.

3. **Read the result.** The `CompactResponse` returns `text` (the compacted,
   line-cited output) and `stats`. Every kept line references a real input line
   number — nothing is summarized away or invented.

4. **(Optional) Verify identity.** Call `whoami_endpoint_v1_whoami_get`
   (`GET /v1/whoami`) to confirm which org/plan a Bearer token maps to.

## Rules
- Errors are `application/json` FastAPI validation envelopes (`{ "detail": [...] }`),
  HTTP 422 — see `errors/codag-problem-types.yml`.
- No client Idempotency-Key contract on the compaction endpoints
  (see `conventions/codag-conventions.yml`).
- Large jobs can be run asynchronously via `compact_job_create_endpoint_v1_compact_jobs_post`
  then polled with `compact_job_get_endpoint_v1_compact_jobs__job_id__get`.
