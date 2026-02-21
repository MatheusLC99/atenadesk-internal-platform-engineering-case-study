# System Design

## 1) Storage Abstraction
A data access interface (`IStorage`) isolates database logic from routes/services.
This improves testability and makes future migrations safer.

## 2) API Organization
REST-style endpoints protected by middleware:
- `requireAuth` for authenticated access
- `requireAdmin` for administrative actions

## 3) Validation Strategy
Schemas and types are shared across layers using:
- Drizzle (schema/types)
- Zod (validation)

This prevents mismatches between frontend payloads and backend expectations.

## 4) Attachments
File uploads are handled server-side with size constraints (up to ~200MB),
supporting knowledge base and request context.

## 5) Audit Logging
Every major CRUD interaction is recorded:
- user identity
- timestamp
- action type (create/update/delete)
- entity/module affected
This increases accountability and traceability.