# Authentication & Authorization

## Authentication
- Passport.js local strategy
- server-side sessions via express-session
- passwords hashed using bcrypt

Why sessions (instead of JWT)?
- simpler for a monolithic app
- login state maintained on the server
- reduced token handling complexity for internal environments

## Authorization
Role-based access control:
- **admin**: user management, custom fields, audit logs, legacy integration
- **standard user**: clients, requests, knowledge base (scoped by rules)

## Route Protection
- unauthenticated users are redirected to login
- admin-only routes hidden and protected server-side