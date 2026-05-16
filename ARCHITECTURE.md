---
file: ARCHITECTURE.md
status: skeleton
last_updated: 2026-05-16
owner: TBD
---

# Architecture

## C4 Level 1 — System Context

```mermaid
C4Context
    title System Context — [client name]
    Person(user, "User", "TODO: describe primary user")
    System(system, "[Client System]", "TODO: describe the system")
    Rel(user, system, "Uses")
```

## C4 Level 2 — Container

```mermaid
C4Container
    title Container Diagram — [client name]
    Person(user, "User")
    Container(web, "Web App", "TODO: tech stack", "TODO: responsibility")
    Container(api, "API", "TODO: tech stack", "TODO: responsibility")
    ContainerDb(db, "Database", "TODO: engine", "TODO: what it stores")
    Rel(user, web, "Uses")
    Rel(web, api, "Calls")
    Rel(api, db, "Reads/Writes")
```

## Invariants

<!-- TODO: populate for [client name] -->

## Key decisions

See `DECISIONS.md` and `docs/decisions/` for ADRs.
