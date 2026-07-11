# ADR 0001: Initial technology stack

- Status: Proposed
- Date: 2026-07-11

## Context

CareCompass needs a phone-first application, responsive web companion, shared domain contracts, private document storage and a server-side structured AI pipeline. The initial team benefits from one primary language and a monorepo.

## Decision

Use:

- pnpm workspaces and Turborepo;
- Expo, React Native and TypeScript for mobile;
- Next.js and TypeScript for web;
- Supabase for Postgres, authentication, private storage and server functions;
- OpenAI Responses API through server-side code for file input and structured output;
- Zod and JSON Schema for validation; and
- GitHub Actions, EAS and Vercel for delivery.

## Consequences

The stack enables shared types and rapid cross-platform development. It also creates dependencies on managed services and requires deliberate work on data residency, provider contracts, native health integrations, RLS verification and server-side secret separation.

## Review triggers

Revisit this decision if clinical deployment requirements, data residency, offline operation, scale, native performance or regulated quality controls make the proposed stack unsuitable.

