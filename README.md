# AtenaDesk — Internal Platform Engineering Case Study

⚠️ **Proprietary Work Notice**

This repository is a public engineering case study describing the architecture,
technical decisions and UX strategy behind an internal management platform
built for a private software company.

Due to confidentiality and security policies, **source code, internal endpoints,
infrastructure details, and company/private data are intentionally not included**.

This documentation exists to demonstrate:
- engineering reasoning
- system design
- product ownership
- real-world problem solving in a production environment

---

## Executive Summary

AtenaDesk is a full-stack TypeScript internal platform (CRM/helpdesk/wiki + admin)
created to centralize operational workflows that were previously fragmented across
paid tools, emails, and individual notes.

It introduced:
- standardized client registration
- request/ticket management with Kanban-style flow
- a shared internal knowledge base with attachments
- role-based access control (support vs engineering vs admin)
- audit logging for accountability
- legacy database connectivity for license management workflows

---

## My Role

- Full-Stack Engineer (end-to-end ownership)
- System Designer (architecture, data model, security boundaries)
- Product & Process Contributor (requirements, UX flow, internal adoption)

---

## Engineering Highlights

- Full-stack TypeScript monolith (modular) optimized for small teams
- Shared validation/types across frontend and backend (Drizzle + Zod)
- Role-based access control + protected routes
- Audit log tracking CRUD actions across modules
- File upload pipeline (attachments) with size constraints
- Real-time communication patterns (WebSockets) where needed
- Legacy system integration (Firebird) for license workflows

---

## What’s Inside This Repo

- Architecture & system design docs (no code)
- Data model and domain modules
- UX flow diagrams (Mermaid)
- Security & compliance guidelines
- Key trade-offs and engineering decisions

---

## Quick Links

- Architecture: `ARCHITECTURE.md`
- System Design: `SYSTEM-DESIGN.md`
- Data Model: `DATA-MODEL.md`
- UX Flows: `UX-FLOWS.md`
- Security: `SECURITY-COMPLIANCE.md`
- Diagrams: `diagrams/`