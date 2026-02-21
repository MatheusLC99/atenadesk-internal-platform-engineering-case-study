# Data Model (High-Level)

This is a **conceptual model** (not the full database schema).

## Core Entities

### Users
- role: admin / user
- authentication via server-side session
- permissions gate module visibility and actions

### Clients
- standardized registration (required fields)
- supports multiple contacts
- supports optional custom fields configured by admins

### Requests (Tickets)
- linked to a client
- linked to department (support / engineering)
- status lifecycle (Kanban-style)
- supports attachments for context

### Knowledge Base Articles
- can be global or client-scoped
- supports attachments (PDF, images, etc.)
- supports structured content for internal procedures

### Custom Fields
- configured by admin
- applied dynamically to clients and articles
- types: text, checkbox, select, multiselect, date

### Audit Logs
- immutable record of changes/actions across modules
- used for compliance and accountability