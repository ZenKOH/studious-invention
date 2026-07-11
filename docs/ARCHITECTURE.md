# Architecture

## Architectural goals

- One shared TypeScript monorepo for mobile, web and domain packages
- Server-side handling of privileged operations and AI credentials
- Care Space isolation enforced in the data layer
- Structured, versioned AI outputs validated before persistence
- Deterministic scheduling and permissions

## Proposed components

| Component | Proposed technology | Responsibility |
| --- | --- | --- |
| Mobile | Expo, React Native, TypeScript | Capture, review, Today and family interactions |
| Web | Next.js, TypeScript | Records, timeline, administration and export |
| Backend | Supabase | Authentication, Postgres, private storage and functions |
| AI pipeline | Server-side OpenAI Responses API | Document interpretation into a strict schema |
| Shared contracts | Zod and JSON Schema | Runtime validation and generated types |

## Core flow

```text
Client upload → private storage → server-side processing
→ structured extraction → validation → source-reference checks
→ draft plan → human review → confirmed plan → deterministic tasks
```

## Security boundaries

- Mobile and web clients receive only public client configuration.
- Service-role and AI credentials exist only in protected server environments.
- Every sensitive row and object belongs to a Care Space.
- Authorisation is enforced independently of interface visibility.
- Logs contain identifiers and status, not document contents by default.

## Decision records

Material architectural decisions must be documented in `docs/adr/` with context, alternatives, consequences and review triggers.

