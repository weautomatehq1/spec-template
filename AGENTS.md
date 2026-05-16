---
file: AGENTS.md
status: skeleton
last_updated: 2026-05-16
owner: TBD
---

# AGENTS.md

> Primary rulebook for every AI worker in this repo. Follows the cross-vendor agents.md convention
> (https://agents.md). Claude Code reads it via the `@AGENTS.md` import in `CLAUDE.md`.

## 1. Project overview

<!-- TODO: populate for [client name] -->

## 2. Required reading order

Before doing any non-trivial work in this repo, read these in order:

1. `INTAKE.md` — verbatim client interview (the source of truth — never invent)
2. `NON_GOALS.md` — explicit out-of-scope (kills gold-plating)
3. `UBIQUITOUS_LANGUAGE.md` — domain vocab; client's word always wins
4. `ARCHITECTURE.md` — system shape + invariants
5. `ROADMAP.md` — phased milestones with `[M-NNN]` IDs
6. `SPRINT.md` — active sprint (your work queue)
7. `FILE_STRUCTURE.md` — where files go
8. `SECURITY.md` — protected paths (auto-merge gates)
9. `STAKEHOLDERS.md` — who decides what
10. `INTEGRATIONS.md` — third-party services + auth model
11. `ENV.md` — env var registry
12. `KPI.md` — success metrics (when populated)
13. `RISKS.md` — known risks + mitigations
14. `RUNBOOK.md` — operational playbook (when populated)
15. `DECISIONS.md` -> `docs/decisions/*.md` — why we picked what we picked
16. `CHANGELOG.md` — release history
17. `AGENTS.md` — this file

**If a spec file contradicts code, the spec wins.** Open an issue; do not silently drift.

## 3. Repo structure

<!-- TODO: populate for [client name] -->

## 4. Worker rules

### Naming
<!-- TODO: populate for [client name] -->

### Branching
<!-- TODO: populate for [client name] -->

### Commit format
<!-- TODO: populate for [client name] -->

### PR size
<!-- TODO: populate for [client name] -->

### Reviewer requirement
<!-- TODO: populate for [client name] -->

## 5. Verification checklist

<!-- TODO: populate for [client name] -->

Before marking any task complete, confirm:

- [ ] All spec files consulted (reading order §2 above)
- [ ] No invented facts — only what INTAKE.md says
- [ ] SECURITY.md protected paths not modified without approval
- [ ] Tests pass
- [ ] No secrets committed

## 6. Forbidden actions

<!-- TODO: populate for [client name] -->

- Do NOT invent client requirements not present in `INTAKE.md`
- Do NOT modify `SECURITY.md` protected paths without explicit approval
- Do NOT commit secrets, API keys, or `.env` files
- Do NOT push directly to `main`

## 7. Cost controls

<!-- TODO: populate for [client name] -->
