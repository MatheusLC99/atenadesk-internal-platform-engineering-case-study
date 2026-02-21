# Integrations

## PostgreSQL (Neon)
Primary data source for operational modules:
clients, requests, knowledge base, audit logs, custom fields, users.

## Firebird (Legacy)
Used to support license-related operational workflows.
Access is restricted to authorized roles, and actions are auditable.

## PDF Generation (jsPDF)
Used for operational exports where document output is needed.

## Real-time (WebSockets)
Used selectively when real-time updates improve internal coordination
(e.g., request status changes, notifications).