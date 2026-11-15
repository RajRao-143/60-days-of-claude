# Challenge Retrospective — LaunchPath AI

**Participant:** Raj Rao  
**Challenge:** AB Talks 60-Day Claude AI Challenge  
**Capstone:** LaunchPath AI — Your Intelligent Placement Readiness Companion  
**Review date:** 15 November 2026

## Evidence note
This retrospective uses the available project conversation, the current GitHub repository and the deployed Day58 application source. The uploaded text available during this review was a Day 42 social post, not a complete 60-day tracker. This document therefore does not invent a day-by-day record for Days 1–55 or claim that every daily challenge task has been independently verified.

## Confirmed capstone journey
- The challenge repository contains day folders and project artefacts, showing a build-in-public workflow. Gaps in folder numbering are not interpreted as proof that work was or was not completed.
- The capstone evolved into LaunchPath AI, a placement-readiness companion for students.
- Day 56 focused on aptitude practice and coding/DSA learning.
- Day 57 added a text-first mock interview experience with role/type selection, question presets and a transparent practice rubric.
- Day 58 brought together the weekly roadmap, learning library, beginner-first tutor, aptitude practice, coding & DSA, interview simulator, jobs & calendar, and analytics.
- The application is deployed through GitHub Pages: https://rajrao-143.github.io/60-days-of-claude/Day58/index.html
- The inspected build is a standalone HTML application using CSS, JavaScript and browser localStorage. No paid API or backend is required for this reviewed build.

## Important technical decisions
- **Local-first storage:** learning and application records are stored in the user's browser. This avoids a backend dependency but does not sync across devices.
- **Manual-first job tracking:** users enter opportunities themselves. Sample opportunities are labelled fictional, not live vacancies.
- **Honest analytics:** metrics are derived from saved activity; demo jobs are excluded from genuine application totals.
- **Text-first interviews:** the simulator works without voice features or paid APIs.
- **Transparent scoring:** interview feedback is a heuristic practice indicator, not a factual assessment of correctness or a hiring decision.
- **Print-to-PDF:** the analytics report uses the browser print flow; it is not a separate PDF service.
- **Mobile follow-up:** responsive CSS exists in source, but actual device verification remains outstanding.

## Skills demonstrated by the capstone
- Structuring a multi-section web application with HTML, CSS and JavaScript.
- Building interactive forms, filters, status workflows and browser-persisted state.
- Connecting learning and job-search workflows around a student problem.
- Designing transparent metrics and communicating product limitations.
- Using GitHub for versioned documentation and GitHub Pages deployment.
- Reviewing a product through engineering, user experience, product and recruiter perspectives.

## What remains to verify
Source inspection confirms that the eight navigation sections exist. It does not prove every interaction works in every browser. Independently verify all module interactions, localStorage persistence, mobile layouts, analytics refresh behaviour, print-to-PDF output and keyboard/accessibility basics. Capture screenshots or test notes as evidence.

## Lessons learned
A useful student product is not just a collection of features. It needs a clear workflow, understandable feedback, honest data, sensible limitations and documentation that helps another person run and evaluate it. A deployed link is an important milestone, but deployment alone is not complete quality assurance.

## Closing reflection
This capstone represents the shift from experimenting with AI-assisted building to shaping a coherent product around a real student need. LaunchPath AI brings preparation, practice, reflection and application tracking into one place. The next step is not feature accumulation; it is careful testing, feedback and steady improvement.
