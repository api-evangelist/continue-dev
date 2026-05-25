# Continue (continue-dev)

Continue is the open-source AI code assistant for VS Code and JetBrains, distributed under Apache 2.0. The IDE extensions and the Continue CLI federate to any LLM provider (Anthropic, OpenAI, Mistral, OpenRouter, Ollama, AWS Bedrock, Google, and more) and load their configuration from Continue Hub. Continue Hub (api.continue.dev) is the registry and IDE API serving assistants, blocks, models, rules, prompts, docs, and MCP servers. Continue has also pivoted into "continuous AI" — source-controlled markdown checks that run as full AI agents on every pull request and surface as GitHub status checks.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=continue-dev-api-evangelist&utm_content=repo)

## Type
- **x-type:** opensource

## Tags
- AI, Artificial Intelligence, Developer Tools, Code Assistant, Open Source, VS Code, JetBrains, CLI, MCP, Apache 2.0

## APIs
- **Continue Hub IDE API** — 8 REST operations at `api.continue.dev/ide/*` for listing/fetching assistants, listing organizations, organization policy, free-trial status, secrets sync, and the Stripe checkout URL for the Models Add-On. Bearer auth with `con_`-prefixed API keys. [OpenAPI](openapi/continue-dev-hub-ide-api-openapi.yml) · [Source spec](https://github.com/continuedev/continue/blob/main/packages/continue-sdk/openapi.yaml)
- **Continue IDE Extensions** — Open-source VS Code and JetBrains plugins providing chat, edit, apply, autocomplete, and agent modes. Apache 2.0. [GitHub](https://github.com/continuedev/continue) · [Docs](https://docs.continue.dev/)
- **Continue CLI** — Open-source CLI powering source-controlled AI checks (`.continue/checks/*.md`) that run locally and in CI. [Quickstart](https://docs.continue.dev/checks/quickstart) · [Run in CI](https://docs.continue.dev/checks/running-in-ci)
- **Continue Hub** — Hosted registry for assistants, blocks (models, rules, prompts, docs, MCP servers, context providers), and policy. [hub.continue.dev](https://hub.continue.dev/)
- **Continue Mission Control** — Metrics and observability for check outcomes and agent runs across repos. [Docs](https://docs.continue.dev/mission-control/metrics)

## Artifacts
- [OpenAPI — Continue Hub IDE API](openapi/continue-dev-hub-ide-api-openapi.yml)
- JSON Schema — [Assistant](json-schema/continue-dev-assistant-schema.json), [Organization](json-schema/continue-dev-organization-schema.json), [Free Trial Status](json-schema/continue-dev-free-trial-status-schema.json)
- [JSON Structure — Assistant](json-structure/continue-dev-assistant-structure.json)
- [JSON-LD context](json-ld/continue-dev-context.jsonld)
- Examples — [List Assistants](examples/continue-dev-list-assistants-example.json), [List Organizations](examples/continue-dev-list-organizations-example.json), [Free Trial Status](examples/continue-dev-free-trial-status-example.json)
- [Spectral ruleset](rules/continue-dev-rules.yml)
- [Naftiko Capability — Hub IDE](capabilities/hub-ide.yaml)
- [Vocabulary](vocabulary/continue-dev-vocabulary.yml)

## Plans, Rate Limits, FinOps
- [Plans](plans/continue-dev-plans-pricing.yml) — Open Source (free, Apache 2.0), Starter ($3/M tokens, pay-as-you-go), Team ($20/seat/month, $10/seat credits), Company (custom enterprise with BYO API keys, SSO, SLA).
- [Rate Limits](rate-limits/continue-dev-rate-limits.yml) — `/ide/*` endpoints return 429 on per-user quota exhaustion; free trial enforces per-user chat and autocomplete caps; BYO LLM passes through to the underlying provider.
- [FinOps](finops/continue-dev-finops.yml) — Cost splits across Continue Hub subscription, Continue-managed proxy tokens, and the user's chosen LLM provider; tag spend by Continue Hub organization (SubAccountId).

## SDKs
- TypeScript — auto-generated from the OpenAPI in `packages/continue-sdk/typescript`.
- Python — auto-generated from the OpenAPI in `packages/continue-sdk/python`.

## Anthropic
Continue federates to Claude (Opus, Sonnet, Haiku) as a first-class chat/edit/apply/autocomplete model. The [`anthropic-continue-hub`](https://github.com/continuedev/anthropic-continue-hub) repo publishes ready-to-use Continue Hub blocks for the Anthropic Messages API.

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-05-25

## Notes
- Continue's primary "API" surface is the Continue Hub IDE API at `api.continue.dev` (8 documented endpoints under `/ide`) — discovered via `packages/continue-sdk/openapi.yaml` in the monorepo. There is no public inference API; model traffic is federated to whichever LLM provider the user configures, optionally via the Continue-managed proxy.
- API keys are bearer tokens prefixed `con_`, generated in the Continue Hub web interface under account settings.
- The local Swagger UI for the Hub IDE API can be launched with `npm run swagger-ui` from `packages/continue-sdk`.

## Maintainers
**FN:** Kin Lane
**Email:** info@apievangelist.com
