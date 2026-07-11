# Security Policy

## Project status

CareCompass AI is pre-alpha and must not be used with real patient information until its privacy and security release gates have passed.

## Reporting a vulnerability

Do not open a public GitHub issue for a suspected vulnerability or include personal data in a report. Use GitHub's private vulnerability-reporting feature when enabled, or contact the repository owner privately.

Include:

- the affected component and version;
- reproduction steps using synthetic data;
- potential impact;
- relevant logs with sensitive content removed; and
- any proposed mitigation.

## Security expectations

- Secrets remain server-side and outside Git history.
- Sensitive tables and storage objects use least-privilege access policies.
- Production data is never copied into development or test fixtures.
- Dependency and secret alerts are treated as release-blocking according to severity.
- Access-control changes require tests proving that unauthorised users are denied.

