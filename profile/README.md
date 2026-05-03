# Factlet Protocol

**Open-source ground truth for AI.** A portable, vendor-neutral way to ground any LLM in your team's private truth — with a built-in signal for when that grounding runs out.

## What lives here

- **[`spec`](https://github.com/factlet-ai/spec)** — the protocol RFC + v0.1 specification
- **[`registry`](https://github.com/factlet-ai/registry)** — community-contributed example factbooks
- **[`reference-sdk`](https://github.com/factlet-ai/reference-sdk)** — Python + TypeScript reference implementations

## Five primitives

- **Factlet** — one atomic truth about your private information (a decision, a constraint, an anti-pattern)
- **FactMap** — the structured collection of factlets covering one body of work
- **Factbook** — a packaged FactMap, versioned in git, portable across implementations
- **FactSignal** — how strong the grounding is at any point, measured in bars (0-5)
- **Low-FactSignal warning** — fires when a model is about to answer in a zone with no relevant factlets

## Try it in 5 minutes (no install)

The protocol is testable in any LLM today via three copy-paste prompts. Build a starter Factbook for your project, use it to answer a question with citations, score FactSignal coverage. See [factlet.ai/getting-started](https://factlet.ai/getting-started).

## Implementation reference

[Kernora's Nora](https://kernora.ai) is the maintained reference implementation. Other tools — Cursor, Claude Code, Continue.dev, Aider, Goose, OpenCode — could implement the protocol and read the same factbooks. The protocol exists with or without any one implementation.

## Status

**v0.1 draft** — the spec is open for RFC. v0.2 ships within 90 days incorporating community feedback. The protocol working group, not Kernora, owns the spec going forward.

## Contributing

See each repo's `CONTRIBUTING.md`. Spec discussions happen in [`spec/discussions`](https://github.com/factlet-ai/spec/discussions); RFC PRs land in [`spec/rfcs`](https://github.com/factlet-ai/spec).

## License

Spec, registry, and reference SDK are MIT-licensed.
