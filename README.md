# Proteus Architecture Map

Interactive visualization of [Proteus API](https://github.com/Newbie1337x/Proteus-API)'s module structure — generated from the real codebase (AST extraction + community detection over the dependency graph), not hand-drawn.

**[Live demo →](https://newbie1337x.github.io/proteus-architecture-map/)**

## What it shows

- **26 real business modules** (training, membership, inventory, payments, IAM, campaigns, logistics...) as bubbles sized by class count, force-separated so they never overlap.
- Click a module for its description, internal layer breakdown (API/Web, Core Services, Domain Model, Persistence, Use Cases), key domain entities and use cases — all pulled straight from the code.
- "Ver estructura interna" drills into a module's actual classes, clustered by architectural layer to show its hexagonal-architecture shape.

Framework noise (Lombok, Spring, MapStruct, Jakarta annotations), test code, and shared-kernel glue (cross-cutting exceptions, tenant context) were filtered out so the map shows production domain code only.
