---
file: README.md
status: skeleton
last_updated: 2026-05-16
owner: TBD
---

# spec-template

> **WeAutomateHQ spec template** — the blank-slate kit that every new client project is cloned from.

## What this is

This repository is a GitHub template. When WeAutomateHQ onboards a new client, we create a fresh repo
from this template:

```bash
gh repo create --template weautomatehq1/spec-template weautomatehq1/<client-slug> --public
```

The result is a repo pre-loaded with the 17-file contract that IFleet workers and the spec decomposer
expect to find in every client project.

**Template repos are never directly edited for a client.** They evolve here and are inherited at clone time.

## The 17-file contract

Every client repo generated from this template contains these 17 spec files
(in the required reading order — see `AGENTS.md` §2):

| # | File | What it captures |
|---|------|------------------|
| 1 | `INTAKE.md` | Verbatim client interview transcript |
| 2 | `NON_GOALS.md` | Explicit out-of-scope decisions |
| 3 | `UBIQUITOUS_LANGUAGE.md` | Domain vocabulary and term definitions |
| 4 | `ARCHITECTURE.md` | System shape, C4 diagrams, invariants |
| 5 | `ROADMAP.md` | Phased milestones with `[M-NNN]` IDs |
| 6 | `SPRINT.md` | Active sprint queue |
| 7 | `FILE_STRUCTURE.md` | Annotated directory tree |
| 8 | `SECURITY.md` | Protected paths and data classification |
| 9 | `STAKEHOLDERS.md` | DACI stakeholder map |
| 10 | `INTEGRATIONS.md` | Third-party services and auth model |
| 11 | `ENV.md` | Environment variable registry |
| 12 | `KPI.md` | Success metrics |
| 13 | `RISKS.md` | Risk register |
| 14 | `RUNBOOK.md` | Operational playbook |
| 15 | `DECISIONS.md` | Index of ADRs in `docs/decisions/` |
| 16 | `CHANGELOG.md` | Release history |
| 17 | `AGENTS.md` | AI worker rulebook (reading order lives here) |

Plus `README.md` (human orientation) and `CLAUDE.md` (ADR-0001 bridge) — 19 `.md` files total.

## How to use

```bash
gh repo create --template weautomatehq1/spec-template weautomatehq1/<client-slug> --public
gh repo clone weautomatehq1/<client-slug>
```

**First file to populate:** `INTAKE.md` — paste the client interview transcript verbatim.
**For AI workers:** read `AGENTS.md` before doing any non-trivial work.

## Related repos

- `weautomatehq1/factory` — master coordination repo (roadmap, ADRs, voice-discovery)
- `weautomatehq1/IFleet` — autonomous worker fleet that reads these specs and ships code
- `weautomatehq1/voice-discovery` — voice AI that conducts client interviews and produces `INTAKE.md`
