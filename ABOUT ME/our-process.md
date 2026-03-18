# Webapper Agile Guide (WAG) - Process Overview

**Last Updated:** 2026-03-18
**Source:** WAG v3.0 (March 4, 2024)

## What This Is

The WAG is Webapper's internal guide to how we build and deliver software. It defines our scrum process, sprint structure, ticket standards, roles, and ceremonies. Every project at Webapper follows this process unless a specific deviation is noted in the project's context file.

## Core Philosophy

High quality software comes from strong process and clarity. Clarity requires effort and discipline. Requirements must be described before programming, and with enough detail to prevent blockers. Tickets are the "one source of truth" (OSOT) for all work.

## Sprint Structure

- **Sprint Length:** 2 weeks, synchronized across all Webapper projects
- **Sprint Naming:** "{SPRINT END DATE} {Customer}" (e.g., "03-28-26 VisionAST")
- **Cadence Goal:** Everything happens during a sprint: planning, standups, review, retrospective

## Ceremonies Schedule

- **Daily Standup (USTeam):** Tuesday through Thursday weekly. Each person answers: What did I do yesterday? What will I do today? Any blockers?
- **Daily Standup (VTeam):** Internal daily scrum during Vietnam business hours
- **Sprint Touchpoint (VTeam + USTeam):** Once per sprint (every 2 weeks)
- **Sprint Planning & Backlog Refinement:** USTeam has weekly meetings per project. Only scrum masters add/remove tickets from sprints.
- **Sprint Review / Demo:** Once per sprint with all available stakeholders including the customer. Can be replaced with a written summary or email report.
- **Retrospective:** Once per month during one of the bi-weekly VTeam-USTeam meetings. Everyone should speak openly and honestly about what went well and what didn't.

## Ticket Workflow (Standard Statuses)

1. **New** - New requirement (bug, feature, or enhancement)
2. **Discovery** - Scrum master works with clients on requirements. Dev team asks questions and provides estimates.
3. **Confirmed** - Ticket is understood, estimation complete
4. **In Progress** - Developer is actively working, updates ticket daily
5. **Ready to Test** - Deployed to QA server, scrum master tests. Failure goes back to In Progress.
6. **Testing Complete - Ready to Deploy** - QA passed, ready for production
7. **Ready for Production Testing** - Deployed to prod, developer verifies, then scrum master and/or client performs UAT. Failure goes back to In Progress.
8. **Done!** - Requirements fully delivered

Additional statuses: Waiting on Customer (blocked on external party), On Hold (paused for any reason), Closed/Stale (no longer relevant), Invalid (duplicate or false report)

## Plan Levels (Ticket Hierarchy)

- **Epic** - Large-scale objective spanning multiple sprints. Should consist of multiple stories. Should not remain open indefinitely. More than 40 hours of discovery alone suggests an epic.
- **Story** - Medium scale, under an epic. Details specific functionality focusing on user value. Should contain subtasks or a checklist if complex.
- **Task** - Smallest unit. Specific, well-defined, achievable in a short timeframe. Should typically take 8 hours or less.

## Estimation

- Every ticket must be estimated before being added to a sprint
- An educated guess is better than no estimate
- **Estimate Confidence** levels:
  - No Earthly Idea: only a guess, ticket not well understood
  - Low: ~25% accurate (could take up to 3x longer)
  - Medium: ~50% accurate (could take up to 2x longer)
  - High: ~75%+ accurate (could take up to 25% longer)

## Sprint Capacity Planning

- Weekly swimlane capacity planning meetings (Fridays)
- Sprint Planning Spreadsheet tracks estimates vs. actual hours, planned vs. unplanned work
- All effort counts: Discovery, Testing, Regression Test Building, Studying, Cross-Training, Documentation, and Development
- No ticket should be added to a sprint if it isn't assigned

## Roles

### Scrum Masters (USTeam)
- Only people who add/remove tickets from sprints
- Groom/curate backlogs consistently (daily/weekly)
- Plan sprints and respond to all questions within 24 hours
- Oversee Estimate Confidence and Estimate fields
- Work with clients to fill the Product Owner role

### Developers
- Update tickets daily (comments, status, hours)
- Keep ticket list matching weekly swim lane
- Communicate blockers immediately, tag USTeam members in tickets
- Do not self-assign tickets without discussing with scrum master
- Goal: finish the work defined for each sprint

## Ticket Rules

- **Comments:** Always add comments as you work, even incremental updates
- **Scope Creep:** If scope is added to an in-progress estimated ticket, new work goes in a new ticket
- **Time Tracking:** Keep Total Time Worked up-to-date. Hours must match Harvest.
- **Git Commits:** Use format `re #123 - this is my commit message` to link commits to tickets
- **Bug Format:** Developer output must include Root Cause and Solution
- **Tags:** Tag tickets with helpful meta information (Bug, Bad Data, Next Sprint, etc.)
- **Followers:** Add followers and use @mentions for notifications

## Key Ticket Metrics

- **Velocity:** Move tickets toward closure as quickly as possible while maintaining quality
- **Accuracy:** All ticket fields as accurate as possible
- **Recency:** Tickets as up-to-date as possible
- **Formula:** High Velocity + High Quality = Great Customer Experience

## Tools

- **Project Management:** Jira (migrated from Assembla). Ticket rules and workflow remain the same.
- **Roadmap/Prioritization:** Productboard (ICE scoring for CloudSee Drive)
- **Time Tracking:** Harvest
- **Standups:** What's Up @ Webapper Miro board
- **Sprints:** Google Sheets Sprint Planning Spreadsheet
- **Process Visualization:** Miro board
