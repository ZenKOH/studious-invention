# Contributing to CareCompass AI

CareCompass is an early-stage health-related coordination project. Contributions must protect users, preserve source fidelity and keep the product within its documented intended use.

## Before starting

1. Open or select a GitHub issue with clear acceptance criteria.
2. Confirm whether the change affects safety, privacy, security, accessibility or intended use.
3. Use synthetic data only. Never add personal health information, credentials or production exports.
4. Create a focused branch such as `feat/document-review` or `fix/care-space-isolation`.

## Pull requests

Every pull request must:

- link its issue;
- describe the problem and solution;
- include tests proportionate to risk;
- document safety, privacy and accessibility implications;
- identify migrations or operational changes;
- provide screenshots for interface changes; and
- include a rollback approach where relevant.

AI prompt, model or schema changes must include evaluation evidence. Permission changes must include negative access-control tests.

## Commit style

Use concise conventional prefixes:

```text
feat: add care space creation
fix: prevent cross-space document access
test: cover ambiguous date extraction
docs: clarify medication safety boundary
chore: configure continuous integration
```

## Definition of done

A change is done when its acceptance criteria pass, automated checks are green, documentation is current, no unresolved review conversations remain and the change is verified in the appropriate environment.

