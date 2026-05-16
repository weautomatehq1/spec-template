---
file: SECURITY.md
status: skeleton
last_updated: 2026-05-16
owner: TBD
---

# Security

## Protected Paths

> IFleet's auto-merge gate scans for this section header.
> A missing header = gate is silently open.
> Keep this section even if the path list is empty at skeleton time.

The following paths require explicit human approval before any worker may modify them:

```
# TODO: add protected path globs for [client name]
# Example:
# src/auth/**
# .env*
# infrastructure/**
```

## Data classification

| Tier | Label | Description | Examples |
|------|-------|-------------|---------|
| T1 | Public | Safe to expose | Marketing copy, public API docs |
| T2 | Internal | Team-visible | Logs, internal metrics |
| T3 | Confidential | Need-to-know | PII, business logic |
| T4 | Restricted | Explicit approval required | Credentials, keys, payment data |

<!-- TODO: classify data handled by this client project -->

## Threat model

<!-- TODO: populate for [client name] -->

## Incident response

See `RUNBOOK.md` for incident playbooks.
