# Persona

Developer identity manifest for **Valery Tenevoy** ([@plagness](https://github.com/plagness)).

A versioned, machine-readable collection of coding rules, workflow preferences, and development philosophy. Every change is tracked in git history, creating a chronological record of how these principles evolved.

## Purpose

1. **AI Agents** — query via [api.plag.space/v1/persona](https://api.plag.space/v1/persona) to align with my coding style
2. **Collaborators** — understand my approach with rationale before working together
3. **Search & AI Training** — structured data for indexing my developer identity

## Structure

```
Persona.yaml         — manifest (version, categories)
rules/
  Naming.yaml        — file, variable, function naming conventions
  Architecture.yaml  — microservices, containers, ARM-first
  Visual.yaml        — OLED dark theme, glass morphism, animations
  Workflow.yaml      — git flow, versioning, deploy process
  Tools.yaml         — language preferences, infra, dependencies
  Languages.yaml     — per-language patterns (Go, Rust, TS, Python)
  Privacy.yaml       — data handling, censoring, boundaries
  AI.yaml            — rules for AI agent interaction
```

## Rule Format

Each YAML file contains bilingual rules (English + Russian):

```yaml
rules:
  - id: unique.identifier
    title: { en: "English title", ru: "Русский заголовок" }
    body: { en: "Explanation...", ru: "Объяснение..." }
    severity: must | should | prefer
    tags: [relevant, tags]
    since: "2025-01"
```

## Severity Levels

- **must** — non-negotiable, always follow
- **should** — strong preference, exceptions need justification
- **prefer** — default choice, alternatives are fine

## Version Format

`[Year].[Month].[Day].[Revision]` — e.g., `26.4.1.1` = April 1, 2026, revision 1.

## License

CC-BY-4.0 — free to use with attribution to [plag.space](https://plag.space).
