# code-review-standard

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
[![Agent Skill](https://img.shields.io/badge/Agent%20Skill-SKILL.md-blue.svg)](SKILL.md)
[![Code Review](https://img.shields.io/badge/code-review-checklist-brightgreen.svg)](SKILL.md)

SynomosAI four-pillar system: **Identity · Traceability · Governance · Symbiosis** — when AI enters business, trust is the only hard currency.

> This repo is part of the [SynomosAI](https://github.com/SynomosAI) skill ecosystem. See [`synomosai-skills`](https://github.com/SynomosAI/synomosai-skills) for the full catalog.

**Keywords**: code review · PR review · quality gate · checklist · Blocker / Suggestion / Nit · engineering standards

## Quick Start

This repo is an **Agent Skill** (SKILL.md spec), not a runnable SDK.

```bash
git clone https://github.com/SynomosAI/code-review-standard.git
cd code-review-standard
cat SKILL.md
```

```bash
head -15 SKILL.md
# cp -r . ~/.workbuddy/skills/code-review-standard/
```

## What this skill covers

A complete code review standard for WorkBuddy full-stack and WeChat ecosystem projects:

- Three iron rules: education-first, specific and actionable, priority-graded
- Three-tier checklist: 🔴 Blockers (security, data loss, API contracts, tests, permissions), 🟡 Suggestions (validation, naming, DRY, performance, error handling), 💭 Nits (comments, format, magic numbers, function length)
- Standard review flow: self-review → PR → 24h response → graded feedback → fixes → Approve
- Hotfix fast track: senior engineer reviews within 30 min; tests/docs within 24h
- Tooling: ESLint, Prettier, Jest/Vitest, SonarQube
- Metrics: response <24h, rounds ≤2, coverage ≥80%, zero security issues
- Comment templates: Blocker / Suggestion / Nit / praise

## Metadata

- **Skill**: `code-review-standard`
- **Version**: 1.0.0
- **License**: MIT (see LICENSE.md)

## License

MIT License. © 2026 注册老炮@MedXpert.

## Disclaimer

This repo is a theoretical-positioning and tooling exploration; it does not represent certified, commercially delivered, or client-specific work. External standards (ISO/IEC 42001, NIST AI RMF, GB/Z 185) are paraphrased from public sources; verify independently before formal citation.
