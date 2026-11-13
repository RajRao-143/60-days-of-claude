# Day 58 — Job Discovery, Application Tracker & Calendar

## Objective
Implement the Day 8 Sprint Workbook scope: a safe job-discovery fallback, application status tracking and a date-based calendar.

## Delivered in this standalone prototype
- Manual job creation, editing and deletion.
- Job title, company, location, role, source and last-checked date.
- Exactly seven statuses: Saved, Applied, Assessment, Interview, Offer, Rejected and Withdrawn.
- Application date, deadline, notes and next action.
- Status summary, search and status filtering.
- Date-ordered agenda for application dates and deadlines.
- In-app reminders for overdue items and deadlines within seven days.
- Clearly labelled fictional sample listings; no fabricated live feed.
- Local browser persistence; no paid API, external service, SMS or WhatsApp.

## Files
- `index.html` — complete standalone application, preserving the prior Day 57 sections and adding Jobs & calendar.
- `README.md` — run instructions, scope and limitations.
- `Day58.md` — milestone record.

## Verification status
Automated static checks are performed on the delivered HTML and JavaScript. The application still requires manual browser testing by the user for form workflows, refresh persistence, date rendering and responsive behavior. No live repository integration or deployment is claimed.

## Manual test checklist
- [ ] Open `index.html` and select Jobs & calendar.
- [ ] Confirm demo records are labelled DEMO — NOT LIVE.
- [ ] Add a job with all required fields; confirm it appears in the list.
- [ ] Try submitting with a required field blank; confirm validation message appears.
- [ ] Edit the job and move it through all seven statuses.
- [ ] Refresh the page; confirm records and statuses persist.
- [ ] Add an application date and deadline; confirm both appear in the calendar.
- [ ] Add a deadline within seven days and one in the past; confirm in-app reminders.
- [ ] Filter by status and search by company/title/location.
- [ ] Delete a record and confirm it disappears from list and calendar.
- [ ] Test at mobile width.
- [ ] Revisit roadmap, resources, tutor, aptitude, coding and interview sections.

## Known limitations
This package extends the available standalone HTML prototype only. The actual GitHub working tree, live hosting configuration, production logs and deployed URL were not available for inspection. Browser-local data is not a substitute for secure multi-user storage. Live job listings are intentionally not claimed.
