# Engineering Decisions & Trade-offs

## Modular Monolith
Chosen to reduce operational complexity while enabling fast delivery for a small team.

## Shared Schemas (Drizzle + Zod)
- prevents frontend/backend payload mismatches
- enables consistent validation and faster refactors

## Wouter for Routing
A lightweight router choice suitable for internal apps where simplicity matters.

## React Query for Data Sync
- reduces duplicated fetching logic
- provides predictable caching/invalidation patterns
- avoids unnecessary network calls

## File Uploads via Multer
A pragmatic server-side approach to support attachments for requests and knowledge base.

## Legacy Database Integration (Firebird)
Kept behind restricted access controls due to:
- sensitivity of license operations
- risk surface of legacy systems