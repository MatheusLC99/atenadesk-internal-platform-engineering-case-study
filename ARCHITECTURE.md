# Architecture

## Architectural Style
AtenaDesk follows a **modular monolith** approach:
frontend and backend run as a single deployable unit.

Rationale:
- simpler deployment for small teams
- reduced operational overhead
- no CORS/proxy complexity
- fast iteration cycle

## Runtime Components
- React SPA for UI
- Express API for business logic
- Storage abstraction layer (`IStorage`) for data access
- PostgreSQL as primary datastore (Neon)
- Firebird integration for legacy workflows (restricted access)
- Optional real-time communication via WebSockets

## High-Level Modules
- Auth & Access Control
- Clients
- Requests (Kanban lifecycle)
- Knowledge Base (articles + attachments)
- Admin (users, custom fields, audit logs)
- Legacy Integration (Firebird)