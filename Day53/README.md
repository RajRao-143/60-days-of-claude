# LaunchPath AI

**Your Intelligent Placement Readiness Companion**  
**Capstone:** India-focused, zero-budget-first MVP

LaunchPath AI is an AI-assisted placement-readiness companion for final-year students and fresher job seekers in India. It brings profile and resume review, role discovery, adaptive diagnostics, explainable readiness scoring, weekly learning plans, practice, interview simulation, job tracking and progress reporting into one responsive workflow.

## Product direction

The approved product loop is:

**Understand → Assess → Prioritize → Practice → Review → Reassess**

AI is assistive, not authoritative. Deterministic rules, curated resources and manual workflows are intended to keep core journeys usable without paid APIs.

## Approved MVP scope

- Profile and resume review, including PDF extraction preview and manual-entry fallback.
- One primary target role and up to two backup roles; explainable top-three recommendations where profile completeness permits.
- Role-based adaptive diagnostic and an explainable readiness score out of 100.
- Stable weekly milestones with adaptive tasks, curated learning resources and a beginner-first tutor.
- Aptitude, coding/DSA and text-first interview practice.
- Job discovery fallback, manual application tracking, calendar and in-app reminders.
- Progress analytics and a downloadable PDF report.
- Free public deployment only where current free-tier terms permit; otherwise a reproducible local demo.

The score is a preparation indicator, **not** a hiring probability or placement guarantee.

## Zero-budget and privacy principles

- No paid API dependency.
- External AI analysis is optional and requires explicit, purpose-specific consent.
- If AI is unavailable or consent is declined, use rule-based matching, templates and curated resources.
- Do not place API secrets in client-side code.
- Minimize collected data and apply user-scoped access controls.
- Clearly distinguish fictional demo data from real user data.

## Documentation status — Day 53

This folder contains project documentation prepared from the approved PRD and Implementation Blueprint. It does **not** establish that the application has been implemented or verified.

**Completed in this Day 53 package:** project overview, setup guidance, environment guidance, conceptual project structure, status summary and challenge submission.

**Pending:** repository inspection, stack/package-manager identification, local setup, application implementation, tests, build, deployment and end-to-end verification. Local setup and application verification are pending because the laptop is unavailable.

No framework, language, database, hosting provider, package manager, environment-variable name or executable command is asserted as the current project configuration. The implementation blueprint explicitly says to inspect the existing repository and preserve its stack and conventions.

## Getting started

1. Obtain access to the project repository and inspect its existing files.
2. Identify the framework, runtime, package manager, scripts, routes, styles and environment configuration from the repository itself.
3. Follow the repository's existing install, development, test and build instructions.
4. Complete the verification checklist in [SETUP.md](SETUP.md) before claiming the application runs.

See:
- [SETUP.md](SETUP.md) — repository inspection, setup sequence and verification checklist.
- [ENVIRONMENT.md](ENVIRONMENT.md) — environment and secret-handling guidance.
- [PROJECT-STRUCTURE.md](PROJECT-STRUCTURE.md) — conceptual product and documentation structure.
- [DAY53-SUMMARY.md](DAY53-SUMMARY.md) — what is documented and what remains pending.
- [day53.md](day53.md) — concise challenge submission.

## Source of truth

This documentation follows only:
1. `LaunchPath_AI_PRD.pdf` — Product Requirements Document, Version 1.0, approved scope baseline.
2. `LaunchPath_AI_Implementation_Blueprint.pdf` — implementation blueprint, Days 2–10 and execution/release gates.

If repository evidence later conflicts with an assumed setup detail, inspect first and preserve the existing working implementation. Do not silently expand or redesign the approved product scope.
