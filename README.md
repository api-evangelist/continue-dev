# Continue (continue-dev)

Continue is the leading open-source AI code assistant for VS Code and JetBrains under Apache 2.0. The Continue CLI powers source-controlled AI checks (markdown-defined) that run in CI as GitHub status checks. The Continue Hub hosts shared assistants, blocks, models, and rules that teams can pull into their config.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/continue-dev/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=continue-dev-api-evangelist&utm_content=repo)

## Type
- **x-type:** company

## Tags
- AI, Developer Tools, Open Source, Code Completion, Customization, Apache 2.0, CLI, CI

## APIs
- **Continue VS Code & JetBrains Extensions** — Open-source autocomplete/chat/edit/agent. Bring your own LLM (OpenAI, Anthropic, Mistral, Ollama, etc.). [GitHub](https://github.com/continuedev/continue) · Apache 2.0
- **Continue CLI** — Source-controlled AI checks (`.continue/checks/`) run in CI. Surface as GitHub status checks. [Repo](https://github.com/continuedev/continue)
- **Continue Hub** — Shared assistants/blocks/models/rules. [hub.continue.dev](https://hub.continue.dev/)

## Plans, Rate Limits, FinOps
- [Plans](plans/continue-dev-plans-pricing.yml) — Open-source extensions are free; Hub has free + paid tiers; AI checks pricing per repo / org.
- [RateLimits](rate-limits/continue-dev-rate-limits.yml) — Inference rate limits depend on the user's chosen model provider.
- [FinOps](finops/continue-dev-finops.yml) — Cost lives with the user's chosen LLM provider plus Hub/checks subscription.

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## Common Properties
- [Website](https://www.continue.dev/)
- [Documentation](https://docs.continue.dev/)
- [GitHub](https://github.com/continuedev/continue)
- [Hub](https://hub.continue.dev/)

## Notes
- Continue's primary "API" surface is the open-source CLI and extensions plus the Hub. There is no public REST inference API; Continue federates to the user's chosen LLM provider.
- No public OpenAPI spec discovered.

## Maintainers
**FN:** Kin Lane

**Email:** kin@apievangelist.com
