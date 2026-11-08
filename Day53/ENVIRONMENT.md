# Environment Configuration

## Status and scope

This document defines configuration-handling principles, not a fabricated environment-variable list. The approved PRD and Implementation Blueprint do not identify a concrete framework, runtime, database, authentication vendor, AI provider, hosting platform or variable names.

The actual environment schema must be derived from the repository and approved integrations after inspection. Local configuration and verification are pending because the laptop is unavailable.

## Configuration principles

- Use environment-based configuration where supported by the existing stack.
- Keep private credentials out of source control and client-side bundles.
- Use host-side secret settings for deployed environments.
- Provide a safe local example/template only after the real variable names and purposes have been confirmed.
- Do not commit populated local environment files.
- Do not invent credentials, endpoints, database names or provider settings.
- Avoid adding paid services or dependencies. Check current free-tier limits, terms, data retention and regional availability before using any provider.

## Potential configuration categories to inspect

These are categories to look for in the existing repository, **not confirmed variables or required services**:

| Category | What to establish | Handling |
|---|---|---|
| Application mode | How development, demo and production modes are selected | Use existing configuration conventions |
| Data store | Whether a data store is configured and how connections are supplied | Keep credentials private; enforce user-scoped access |
| Authentication | Whether email/password or an eligible free identity provider is configured | Never expose secrets in client code |
| Optional AI adapter | Whether an external provider is configured | Optional; explicit purpose-specific consent required before each analysis |
| File/PDF handling | Any parser or upload limits already configured | Validate type and size; retain manual-entry fallback |
| Deployment | Host-specific settings and build configuration | Verify current free-tier terms; configure secrets on the host |
| Logging/diagnostics | Existing error and diagnostic settings | Avoid logging unnecessary resume, contact or interview data |

## AI and integration controls

- External AI analysis must show purpose, data categories and provider/destination before explicit opt-in.
- Consent must be specific to the analysis, recorded with purpose/provider/data categories/timestamp/policy version, and revocable.
- AI unavailable or consent declined: use deterministic rules, templates and curated resources.
- Job feed unavailable: use clearly labelled curated/demo listings and manual entries.
- Voice unsupported: use text interview.
- Cloud unavailable: disclose local demo mode and persistence limitations.

## Security checklist

- [ ] No secrets committed to the repository.
- [ ] No private API key included in browser/client code.
- [ ] HTTPS used for deployed traffic.
- [ ] Input and upload type/size validation is present.
- [ ] Rendered content is sanitized.
- [ ] User-scoped ownership checks protect records.
- [ ] External AI requests are blocked until purpose-specific consent.
- [ ] Data collection and retention are minimized and documented.
- [ ] Current provider free-tier terms and data-retention terms are reviewed.

All checks remain **pending verification** until performed against the actual repository and runtime.
