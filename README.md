# Continue (continue-dev)

Continue is the open-source AI code assistant for VS Code and JetBrains, distributed under Apache 2.0. The Continue IDE extensions and the Continue CLI federate to any LLM provider — Anthropic, OpenAI, Mistral, OpenRouter, Ollama, and a Continue-managed proxy — and load their configuration from Continue Hub. Continue Hub (api.continue.dev) is the registry and IDE API that serves assistants, blocks, models, rules, prompts, docs, and MCP servers to the extensions, along with free-trial status, organization policy, secrets sync, and the Stripe checkout URL for the Models Add-On. Continue has also pivoted into "continuous AI" — source- controlled checks that live as markdown files under .continue/checks/ and run in CI as GitHub status checks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI
- Artificial Intelligence
- Developer Tools
- Code Assistant
- Open Source
- VS Code
- JetBrains
- CLI
- MCP
- Apache 2.0

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-25

## APIs

### Continue Hub IDE API

REST API exposed by api.continue.dev that the Continue VS Code and JetBrains extensions and the Continue CLI use to list and refresh assistants, list organizations, fetch organization policy, sync user secrets, check free-trial chat/autocomplete quota, and obtain a Stripe checkout URL for the Models Add-On. Bearer auth with API keys prefixed con_, generated in the Continue Hub web interface. Auto-generated TypeScript and Python clients ship in packages/continue-sdk in the open-source continuedev/continue monorepo.

- **Human URL:** [https://github.com/continuedev/continue/blob/main/packages/continue-sdk/openapi.yaml](https://github.com/continuedev/continue/blob/main/packages/continue-sdk/openapi.yaml)
- **Base URL:** `https://api.continue.dev`

#### Tags

- Hub
- IDE
- Assistants
- Organizations
- AI

#### Properties

- [Documentation](https://github.com/continuedev/continue/tree/main/packages/continue-sdk)
- [OpenAPI](openapi/continue-dev-hub-ide-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/continue-dev-hub-ide-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/continue-dev-hub-ide-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/continue-dev-assistant-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/continue-dev-organization-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/continue-dev-free-trial-status-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/continue-dev-assistant-structure.json)
- [JSON-LD](json-ld/continue-dev-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/continue-dev-list-assistants-example.json)
- [Example](examples/continue-dev-list-organizations-example.json)
- [Example](examples/continue-dev-free-trial-status-example.json)
- [SDK](https://www.npmjs.com/package/@continuedev/sdk)
- [SDK](https://pypi.org/project/continuedev-sdk/)

### Continue IDE Extensions

Open-source IDE plugins shipping for VS Code and JetBrains. Provide chat, edit, apply, autocomplete, and agent modes. Bring your own LLM (Anthropic, OpenAI, Mistral, OpenRouter, Ollama) or use the Continue-managed proxy on the Hub Starter/Team tiers. Configured via YAML assistants pulled from Continue Hub.

- **Human URL:** [https://docs.continue.dev/](https://docs.continue.dev/)
- **Base URL:** `https://www.continue.dev`

#### Tags

- VS Code
- JetBrains
- Open Source
- Apache 2.0
- AI

#### Properties

- [GitHub Repository](https://github.com/continuedev/continue)
- [Documentation](https://docs.continue.dev/)
- [License](https://github.com/continuedev/continue/blob/main/LICENSE)
- [Postman Collection](collections/continue-dev-hub-ide-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/continue-dev-hub-ide-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Continue CLI

Open-source command-line interface powering Continue's source-controlled AI checks. Checks are markdown files in .continue/checks/ that run as full AI agents against pull requests and surface results as GitHub status checks. Also runs assistants locally and headlessly.

- **Human URL:** [https://docs.continue.dev/checks/quickstart](https://docs.continue.dev/checks/quickstart)
- **Base URL:** `https://continue.dev/check`

#### Tags

- CLI
- CI
- Checks
- Open Source
- AI

#### Properties

- [GitHub Repository](https://github.com/continuedev/continue)
- [Documentation](https://docs.continue.dev/checks/quickstart)
- [Documentation](https://docs.continue.dev/checks/running-locally)
- [Documentation](https://docs.continue.dev/checks/running-in-ci)
- [Postman Collection](collections/continue-dev-hub-ide-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/continue-dev-hub-ide-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Continue Hub

Hosted registry where teams publish and share assistants, blocks (models, rules, prompts, docs, MCP servers, context providers), and policy. Powers the Continue Hub IDE API and is the primary commercial surface alongside the open-source extensions and CLI.

- **Human URL:** [https://hub.continue.dev/](https://hub.continue.dev/)
- **Base URL:** `https://hub.continue.dev`

#### Tags

- Hub
- Registry
- Assistants
- Blocks
- MCP

#### Properties

- [Portal](https://hub.continue.dev/)
- [Documentation](https://docs.continue.dev/)
- [Sign Up](https://continue.dev/login)
- [Postman Collection](collections/continue-dev-hub-ide-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/continue-dev-hub-ide-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Continue Mission Control

Observability surface for tracking check outcomes, agent runs, and adoption metrics across an organization's repositories. Part of the Team and Company tiers.

- **Human URL:** [https://docs.continue.dev/mission-control/metrics](https://docs.continue.dev/mission-control/metrics)
- **Base URL:** `https://continue.dev`

#### Tags

- Mission Control
- Metrics
- Observability
- Checks

#### Properties

- [Documentation](https://docs.continue.dev/mission-control/beyond-checks)
- [Documentation](https://docs.continue.dev/mission-control/metrics)
- [Postman Collection](collections/continue-dev-hub-ide-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/continue-dev-hub-ide-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.continue.dev/)
- [Portal](https://www.continue.dev/)
- [Documentation](https://docs.continue.dev/)
- [GitHub Organization](https://github.com/continuedev)
- [GitHub Repository](https://github.com/continuedev/continue)
- [LinkedIn](https://www.linkedin.com/company/continuedev)
- [Blog](https://blog.continue.dev/)
- [Sign Up](https://continue.dev/login)
- [Pricing](https://www.continue.dev/pricing)
- [Getting Started](https://docs.continue.dev/)
- [Documentation](https://docs.continue.dev/checks/quickstart)
- [Documentation](https://docs.continue.dev/checks/reference)
- [Checks Docs](https://continue.dev/check)
- [Hub](https://hub.continue.dev/)
- [License](https://github.com/continuedev/continue/blob/main/LICENSE)
- [SDK](https://github.com/continuedev/continue/tree/main/packages/continue-sdk/typescript)
- [SDK](https://github.com/continuedev/continue/tree/main/packages/continue-sdk/python)
- [Tool](https://github.com/continuedev/rules)
- [Tool](https://github.com/continuedev/create-software-factory)
- [Tool](https://github.com/continuedev/pollhook)
- [Tool](https://github.com/continuedev/instinct)
- [Code Examples](https://github.com/continuedev/awesome-rules)
- [Code Examples](https://github.com/continuedev/checks)
- [Plugins](https://github.com/continuedev/anthropic-continue-hub)
- [Plugins](https://github.com/continuedev/openai-continue-hub)
- [Plugins](https://github.com/continuedev/mistral-continue-hub)
- [Plugins](https://github.com/continuedev/openrouter-continue-hub)
- [Plugins](https://github.com/continuedev/ollama-continue-hub)
- [Plugins](https://github.com/continuedev/google-continue-hub)
- [Spectral Rules](rules/continue-dev-rules.yml)
- [Vocabulary](vocabulary/continue-dev-vocabulary.yml)
- [Plans](plans/continue-dev-plans-pricing.yml)
- [Rate Limits](rate-limits/continue-dev-rate-limits.yml)
- [Fin Ops](finops/continue-dev-finops.yml)
- [L L Ms Txt](https://docs.continue.dev/llms.txt)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
