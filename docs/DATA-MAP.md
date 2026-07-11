# Data Map

This inventory must be completed before real user data is accepted.

| Data category | Purpose | System of record | Access | Retention | External processor |
| --- | --- | --- | --- | --- | --- |
| Account identity | Authentication and account recovery | Auth service | User and authorised operations | To be defined | Supabase |
| Care Space membership | Authorisation and collaboration | Postgres | Authorised members by role | To be defined | Supabase |
| Uploaded documents | Build user-requested draft plans | Private object storage | Explicitly authorised members and server pipeline | To be defined | Supabase; approved AI provider during processing |
| Structured extraction | Review and provenance | Postgres | Authorised members | To be defined | Supabase |
| Confirmed care-plan items | Daily coordination | Postgres | Authorised members | To be defined | Supabase |
| Check-ins | User-entered recovery context | Postgres | Role-dependent | To be defined | Supabase |
| Audit events | Security and change history | Postgres | Restricted operations access | To be defined | Supabase |
| Operational telemetry | Reliability and debugging | Observability service | Restricted engineering access | Short and defined | To be selected |

## Required decisions

- Production region and data residency
- Maximum document retention
- Whether deletion is immediate or subject to a short recovery window
- Audit-event retention
- Backup expiration and deletion propagation
- Data export format
- Processor contracts and permitted subprocessors

