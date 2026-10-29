# Continue

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

Continue is the open-source AI code assistant for VS Code and JetBrains, distributed under Apache 2.0. The Continue IDE extensions and the Continue CLI federate to any LLM provider — Anthropic, OpenAI, Mistral, OpenRouter, Ollama, and a Continue-managed proxy — and load their configuration from Continue Hub. Continue Hub (api.continue.dev) is the registry and IDE API that serves assistants, blocks, models, rules, prompts, docs, and MCP servers to the extensions, along with free-trial status, organization policy, secrets sync, and the Stripe checkout URL for the Models Add-On. Continue has also pivoted into "continuous AI" — source- controlled checks that live as markdown files under .continue/checks/ and run in CI as GitHub status checks.

**Areas:** Artificial Intelligence · Developer Tools · Code Assistant · Open Source · VS Code · JetBrains · CLI · MCP · Apache 2.0

## Continue on APIs.io

Everything profiled for Continue is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/continue-dev/](https://apis.io/providers/continue-dev/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [Continue IDE Extensions](https://apis.io/apis/continue-dev/ide-extensions/) — Open-source IDE plugins shipping for VS Code and JetBrains. Provide chat, edit, apply, autocomplete, and agent modes. Bring your own LLM (Anthropic, OpenAI,…
- [Continue CLI](https://apis.io/apis/continue-dev/continue-cli/) — Open-source command-line interface powering Continue's source-controlled AI checks. Checks are markdown files in .continue/checks/ that run as full AI…
- [Continue Hub](https://apis.io/apis/continue-dev/continue-hub/) — Hosted registry where teams publish and share assistants, blocks (models, rules, prompts, docs, MCP servers, context providers), and policy. Powers the…
- [Continue Mission Control](https://apis.io/apis/continue-dev/mission-control/) — Observability surface for tracking check outcomes, agent runs, and adoption metrics across an organization's repositories. Part of the Team and Company tiers.
- [Continue Ide API](https://apis.io/apis/continue-dev/continue-dev-ide-api/) — The Ide API from Continue — 8 operation(s) for ide.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Continue Dev Agentic Access](https://apis.io/agentic-access/continue-dev/continue-dev-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Continue Hub Assistant](https://apis.io/schemas/continue-dev/continue-dev-assistant/)
- [Continue Free Trial Status](https://apis.io/schemas/continue-dev/continue-dev-free-trial-status/)
- [Continue Hub Organization](https://apis.io/schemas/continue-dev/continue-dev-organization/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Continue Dev Assistant Structure](https://apis.io/json-structure/continue-dev/continue-dev-assistant-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Continue Dev Context](https://apis.io/jsonld/continue-dev/continue-dev-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Continue Vocabulary](https://apis.io/vocabularies/continue-dev/continue-dev-vocabulary/)

#### Examples (2)

Example requests and responses.

- [Continue Dev Free Trial Status Example](https://apis.io/examples/continue-dev/continue-dev-free-trial-status-example/)
- [Continue Dev List Organizations Example](https://apis.io/examples/continue-dev/continue-dev-list-organizations-example/)

#### Collections (3)

Postman and Open Collection request collections.

- [Continue Hub IDE API](https://apis.io/collections/continue-dev/open-continue-dev-hub-ide-api/)
- [Continue Hub Ide API](https://apis.io/collections/continue-dev/open-continue-dev-ide-api/)
- [Continue Hub Ide API](https://apis.io/collections/continue-dev/postman-continue-dev-ide-api/)

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Continue — jsonschema rules](https://apis.io/rules/continue-dev/continue-dev-jsonschema-spectral-rules/)
- [Continue API Rules](https://apis.io/rules/continue-dev/continue-dev-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Continue Dev Authentication](https://apis.io/security/continue-dev/continue-dev-authentication/)
- [Continue Dev Domain Security](https://apis.io/security/continue-dev/continue-dev-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Continue Dev Plans Pricing](https://apis.io/plans/continue-dev/continue-dev-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Continue Dev Rate Limits](https://apis.io/rate-limits/continue-dev/continue-dev-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Continue Dev Finops](https://apis.io/finops/continue-dev/continue-dev-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.continue.dev/)
- [Documentation](https://docs.continue.dev/)
- [Getting started](https://docs.continue.dev/)
- [Pricing](https://www.continue.dev/pricing)
- [Blog](https://blog.continue.dev/)
- [GitHub](https://github.com/continuedev)

## API Evangelist rating

**Kin Score 45.7** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 64.3 |
| Contract quality | 60.0 |
| Contract governance | 27.3 |
| Operational transparency | 36.8 |
| Developer ergonomics | 63.1 |
| Access clarity | 21.1 |

**Agent readiness 23.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 15.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/continue-dev/](https://apis.io/providers/continue-dev/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Continue: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/continue-dev/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
