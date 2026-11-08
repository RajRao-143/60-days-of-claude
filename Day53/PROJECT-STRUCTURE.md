# Project Structure

## Important note

The actual repository has not been inspected. The structure below is a **conceptual organization guide derived from the approved product information architecture**, not a claim about existing directories, filenames, framework conventions or implemented modules.

Preserve the repository's current stack and conventions. Do not create every folder below automatically or introduce dependencies simply to match this illustration.

## Approved product areas

The PRD's information architecture identifies:
- Dashboard
- Profile & Resume
- Roles
- Assessment
- Roadmap
- Learn/Tutor
- Practice
- Interviews
- Jobs/Tracker
- Calendar
- Reports
- Settings/Consent

The implementation blueprint also calls for responsive navigation across Dashboard, Profile, Roles, Roadmap, Practice, Interviews, Jobs and Reports, with Settings included in the fresh-conversation project shell prompt.

## Conceptual feature map

```text
LaunchPath AI
├── Dashboard
├── Profile & Resume
├── Roles
├── Assessment
├── Readiness
├── Roadmap
├── Learn & Tutor
├── Practice
│   ├── Aptitude
│   └── Coding / DSA
├── Interviews
├── Jobs & Tracker
├── Calendar
├── Reports
└── Settings & Consent
```

This is a product-level map, not a filesystem tree.

## Architecture boundaries from the approved PRD

```text
Responsive web client
        |
Application / API layer
        |
Authentication + user-scoped data store
        |
Deterministic role-fit / readiness / roadmap services
        |
Optional consent-gated AI adapter
        |
Curated content, practice bank and report export
```

Keep the optional AI provider behind an adapter interface and isolate prompts from business rules. Deterministic services and curated/manual fallbacks must keep core paths usable without paid APIs.

## Data domains identified in the PRD

The PRD names these core entities:

- User and ConsentRecord
- Profile and ResumeDocument metadata
- Skill, Role and RoleSkill
- Assessment, Question and Attempt
- ReadinessSnapshot
- Roadmap, Milestone, Task and Resource
- TutorTopicProgress
- PracticeAttempt
- InterviewSession, InterviewAnswer and RubricEvaluation
- Job, Application and Reminder
- Report

These are domain concepts, not confirmed database tables or implemented schemas.

## Repository organization: how to decide

After laptop access is restored:

1. Inspect the existing source tree and entry points.
2. Identify current feature boundaries, routes, shared components and data-access conventions.
3. Map the approved product areas onto the existing structure with the smallest coherent changes.
4. Reuse existing UI primitives and design tokens rather than duplicating them.
5. Preserve working behavior and avoid framework replacement.
6. Document the real directory tree only after it has been inspected.

## Shared UI and design direction

The implementation blueprint calls for reusable primitives such as Button, Card, Badge, Progress, EmptyState, Loading and Error. The PRD's visual direction is a deep navy/ink base, clean white surfaces, restrained teal/blue accents and warm amber for attention, with consistent typography, spacing and icon style.

These are approved design guidelines; they do not imply that the components or design tokens have already been implemented.
