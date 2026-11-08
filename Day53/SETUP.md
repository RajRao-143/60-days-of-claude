# Setup Guide

## Current status

**Local setup has not been performed.** The laptop is unavailable, so repository inspection, dependency installation, application launch and verification remain pending. This guide documents the safe sequence to follow when access is restored; it is not evidence that the app currently runs.

## 1. Prerequisites to confirm

Do not install a new framework or replace the existing stack based on this document. First identify the project's actual requirements from its repository and official project files.

Inspect:
- Repository root and existing README/setup notes.
- Runtime and framework indicators.
- Lockfiles and package manager.
- Existing scripts for development, build, lint, typecheck and tests.
- Route structure, entry points, styles and current environment files.
- Existing deployment configuration, if any.

Useful read-only inspection commands (run from the repository root):

```bash
git status --short
git branch --show-current
ls -la
find . -maxdepth 2 -type f | sort
```

These commands inspect repository state; they do not install dependencies or prove that the application works. On systems without `find` or a compatible shell, use the file browser or equivalent listing command.

## 2. Clone or open the repository

If the repository is hosted remotely, use its actual clone URL:

```bash
git clone <repository-url>
cd <repository-directory>
```

If the repository is already present locally, open its root directory instead. Do not invent a repository URL or directory name.

## 3. Identify the correct install and run commands

Read the existing manifest, lockfile and scripts before running commands. Use the package manager already selected by the repository.

Examples below are **conditional patterns only**, not a declaration that LaunchPath AI uses Node.js or any particular package manager:

```bash
# Only if the repository contains package.json and an npm lockfile:
npm ci
npm run
```

Then run only the development, test, lint, typecheck and build scripts that are actually defined in the repository. If the project uses another runtime or package manager, follow its checked-in instructions and lockfile instead. Do not create scripts or add dependencies merely to make these examples work.

Record the exact commands and observed outcomes after local verification.

## 4. Configure environment

1. Inspect existing environment templates and configuration references.
2. Document each required variable, purpose and whether it is public or secret.
3. Obtain values only from approved providers/accounts and current free-tier terms.
4. Keep secrets in local environment files or host-side secret settings as appropriate.
5. Ensure secret files are excluded from version control.
6. Never place private API keys or service credentials in browser/client code.
7. Do not add an external AI provider or live job feed unless it is within the approved scope, permitted on a free tier and properly consent-gated.

See [ENVIRONMENT.md](ENVIRONMENT.md). No variable names or values are prescribed here because neither source document specifies a concrete stack-specific environment schema.

## 5. Run and verify

After setup, follow the actual repository scripts and verify:

- Application starts using the repository's documented command.
- Primary navigation and responsive layout behave as intended.
- Sample/fictional data is explicitly labelled.
- No secrets appear in source files or client bundles.
- Optional AI paths are blocked until purpose-specific consent; fallback paths remain available.
- Manual profile entry remains available if PDF parsing fails.
- Text interview remains available if voice is unsupported.
- Curated/demo jobs and manual job entry remain clear if a live feed is unavailable.
- Local-mode persistence limitations are disclosed.

Do not mark any item as passed until it has been checked in the target environment.

## 6. Release sequence

The approved blueprint places integration, analytics, PDF reporting and QA on Day 9, then hardening, clean install, tests, production build, deployment checks and demo preparation on Day 10. Preserve these release gates. Do not claim deployment succeeded until the deployed URL has been opened and verified.

## Verification record

| Check | Status |
|---|---|
| Repository inspected | Pending — laptop unavailable |
| Stack and package manager identified | Pending |
| Dependencies installed | Pending |
| Local application launched | Pending |
| Responsive navigation checked | Pending |
| Tests / lint / typecheck (if configured) | Pending |
| Production build | Pending |
| Environment and secret review | Pending |
| End-to-end journey | Pending |
| Deployment or reproducible local demo | Pending |
