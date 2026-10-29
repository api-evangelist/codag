# Codag

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Codag is a Y Combinator (Summer 2026) developer-tools company building drop-in log compression for AI agents. It takes oversized infrastructure logs — from Kubernetes, Docker, AWS CloudWatch, Vercel, Railway, Datadog, Sentry, syslog and unstructured sources — and returns only the lines that matter as schema-valid JSON, ranked into patterns where every kept line cites a real log line number so nothing is summarized away or invented. This lets coding agents like Claude, Codex and Cursor debug from the evidence that matters at roughly 95% fewer tokens without exhausting their context window. Codag ships as a hosted HTTPS API (/v1/compact), an open-source Go CLI, and an MCP server, with a deterministic Rust log-templating engine (codag-drain) as the free/fallback path.

**Areas:** Company · Developer Tools · Logging · Observability · Log Compression · AI Agents · MCP · LLM Tooling · Debugging · Y Combinator

## Codag on APIs.io

Everything profiled for Codag is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/codag/](https://apis.io/providers/codag/)** — or go straight to one of the APIs or properties below.

### APIs (19)

- [Codag Activate API](https://apis.io/apis/codag/codag-activate-api/) — The Activate API from Codag — 2 operation(s) for activate.
- [Codag Admin API](https://apis.io/apis/codag/codag-admin-api/) — The Admin API from Codag — 2 operation(s) for admin.
- [Codag Anonymous API](https://apis.io/apis/codag/codag-anonymous-api/) — The Anonymous API from Codag — 1 operation(s) for anonymous.
- [Codag Auth API](https://apis.io/apis/codag/codag-auth-api/) — The Auth API from Codag — 4 operation(s) for auth.
- [Codag Billing API](https://apis.io/apis/codag/codag-billing-api/) — The billing API from Codag — 4 operation(s) for billing.
- [Codag Capsule API](https://apis.io/apis/codag/codag-capsule-api/) — The Capsule API from Codag — 1 operation(s) for capsule.
- [Codag Cli API](https://apis.io/apis/codag/codag-cli-api/) — The Cli API from Codag — 2 operation(s) for cli.
- [Codag Compact API](https://apis.io/apis/codag/codag-compact-api/) — The Compact API from Codag — 3 operation(s) for compact.
- [Codag Free API](https://apis.io/apis/codag/codag-free-api/) — The Free API from Codag — 1 operation(s) for free.
- [Codag Health API](https://apis.io/apis/codag/codag-health-api/) — The Health API from Codag — 1 operation(s) for health.
- [Codag Incident Memory API](https://apis.io/apis/codag/codag-incident-memory-api/) — The Incident Memory API from Codag — 3 operation(s) for incident memory.
- [Codag Install.sh API](https://apis.io/apis/codag/codag-install-sh-api/) — The Install.sh API from Codag — 1 operation(s) for install.sh.
- [Codag Internal API](https://apis.io/apis/codag/codag-internal-api/) — The Internal API from Codag — 2 operation(s) for internal.
- [Codag Onboard API](https://apis.io/apis/codag/codag-onboard-api/) — The Onboard API from Codag — 2 operation(s) for onboard.
- [Codag Org API](https://apis.io/apis/codag/codag-org-api/) — The Org API from Codag — 14 operation(s) for org.
- [Codag Orgs API](https://apis.io/apis/codag/codag-orgs-api/) — The Orgs API from Codag — 13 operation(s) for orgs.
- [Codag Parse API](https://apis.io/apis/codag/codag-parse-api/) — The Parse API from Codag — 1 operation(s) for parse.
- [Codag Whoami API](https://apis.io/apis/codag/codag-whoami-api/) — The Whoami API from Codag — 1 operation(s) for whoami.
- [Codag OAUTH API](https://apis.io/apis/codag/codag-oauth-api/) — The Oauth API from Codag — 2 operation(s) for oauth.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [codag](https://apis.io/servers/codag/codag/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Codag Agentic Access](https://apis.io/agentic-access/codag/codag-agentic-access/)

#### Collections (19)

Postman and Open Collection request collections.

- [infra-logs templater Activate API](https://apis.io/collections/codag/open-codag-activate-api/)
- [infra-logs templater Activate Admin API](https://apis.io/collections/codag/open-codag-admin-api/)
- [infra-logs templater Activate Anonymous API](https://apis.io/collections/codag/open-codag-anonymous-api/)
- [infra-logs templater Activate Auth API](https://apis.io/collections/codag/open-codag-auth-api/)
- [infra-logs templater Activate billing API](https://apis.io/collections/codag/open-codag-billing-api/)
- [infra-logs templater Activate Capsule API](https://apis.io/collections/codag/open-codag-capsule-api/)
- [infra-logs templater Activate Cli API](https://apis.io/collections/codag/open-codag-cli-api/)
- [infra-logs templater Activate Compact API](https://apis.io/collections/codag/open-codag-compact-api/)
- [infra-logs templater Activate Free API](https://apis.io/collections/codag/open-codag-free-api/)
- [infra-logs templater Activate Health API](https://apis.io/collections/codag/open-codag-health-api/)
- [infra-logs templater Activate Incident Memory API](https://apis.io/collections/codag/open-codag-incident-memory-api/)
- [infra-logs templater Activate Install.sh API](https://apis.io/collections/codag/open-codag-install-sh-api/)
- [infra-logs templater Activate Internal API](https://apis.io/collections/codag/open-codag-internal-api/)
- [infra-logs templater Activate Oauth API](https://apis.io/collections/codag/open-codag-oauth-api/)
- [infra-logs templater Activate Onboard API](https://apis.io/collections/codag/open-codag-onboard-api/)
- [infra-logs templater Activate Org API](https://apis.io/collections/codag/open-codag-org-api/)
- [infra-logs templater Activate Orgs API](https://apis.io/collections/codag/open-codag-orgs-api/)
- [infra-logs templater Activate Parse API](https://apis.io/collections/codag/open-codag-parse-api/)
- [infra-logs templater Activate Whoami API](https://apis.io/collections/codag/open-codag-whoami-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Codag Openapi Overlay](https://apis.io/overlays/codag/codag-openapi-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Codag Authentication](https://apis.io/security/codag/codag-authentication/)
- [Codag Domain Security](https://apis.io/security/codag/codag-domain-security/)
- [Codag Vulnerability Disclosure](https://apis.io/security/codag/codag-vulnerability-disclosure/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://codag.ai/)
- [Documentation](https://codag.ai/docs)
- [Getting started](https://codag.ai/docs)
- [API reference](https://codag.ai/docs/rest-api.html)
- [Pricing](https://codag.ai/pricing)
- [Sign up](https://console.codag.ai)
- [Support](https://codag.ai/support)
- [Blog](https://codag.ai/blog)
- [Security](https://codag.ai/.well-known/security.txt)
- [Terms of service](https://codag.ai/terms)
- [Privacy policy](https://codag.ai/privacy)
- [GitHub](https://github.com/codag-megalith)

## API Evangelist rating

**Kin Score 47.1** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 38.1 |
| Contract governance | 4.5 |
| Operational transparency | 23.7 |
| Developer ergonomics | 80.4 |
| Access clarity | 44.7 |

**Agent readiness 29.0** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | yes |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 30.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/codag/](https://apis.io/providers/codag/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Codag: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/codag/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
