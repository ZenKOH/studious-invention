# Threat Model

## Protected assets

- User identity and authentication sessions
- Uploaded care documents
- Care Space memberships and permissions
- Extracted and confirmed care information
- Privileged service and AI credentials
- Audit trails and deployment integrity

## Principal threats

| Threat | Example control |
| --- | --- |
| Cross-Care-Space access | Row-level security and negative isolation tests |
| Broken object access | Server-side authorisation on every document operation |
| Credential disclosure | Protected secrets, push protection and rotation |
| Malicious file upload | Type, size and malware validation; isolated processing |
| Prompt injection in documents | Treat document text as untrusted data; fixed tool permissions and output schemas |
| Unsupported AI output | Strict schema, source-reference validation and human confirmation |
| Excessive logging | Privacy-minimised structured logs and redaction |
| Unauthorised caregiver access | Expiring invitations, granular roles and immediate revocation |
| Supply-chain compromise | Lockfiles, dependency review and automated vulnerability alerts |
| Unsafe deployment | Protected environments, approvals and rollback procedures |

## Verification

Threat controls must have automated tests where possible and manual review where human judgement is required. The model must be revisited when new data types, processors, roles or external integrations are introduced.

