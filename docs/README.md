# OctoAcme Project Management Docs

## Overview

OctoAcme's project management approach follows a lightweight, repeatable lifecycle that emphasizes iterative delivery, clear ownership, and measurable outcomes. Work typically starts with an **initiation** step to validate the business need and align stakeholders, using a simple one-pager that captures the problem, SMART objective, success metrics, timeline, risks, and resourcing. Once approved, the team moves into **planning**, where work is broken into shippable increments with clear acceptance criteria, estimates, dependencies, and a documented Definition of Done. From there, delivery proceeds through **execution**, **release**, and **close/retrospective**, ensuring the team captures learnings and continuously improves.

Roles and responsibilities are explicitly defined to prevent ambiguity and single-owner bottlenecks. A named **Project Manager (PM)** coordinates schedules, delivery rituals, risks, and communications; a **Product Manager (PdM)** owns outcomes, prioritization, and success measurement; **Developers** implement and test features while collaborating on design and estimates; **QA/Testing** validates quality and acceptance criteria; and **Stakeholders** provide input and approvals. These personas reinforce clear decision-making, ownership of artifacts (like the one-pager, backlog, and risk register), and shared expectations for what "done" means.

Execution is organized around predictable team rhythms and transparent workflow tracking. Teams use daily standups for progress and blockers, weekly delivery syncs to surface risks and dependencies, and sprint-end demos/reviews to validate increments. Day-to-day work is managed via a project board with standard columns (Backlog → Ready → In Progress → In Review → QA → Done). Communication is structured around stakeholder needs, using a consistent weekly status template (progress, next steps, risks/blockers, asks/decisions), plus clear escalation paths from team triage to PM/Product Lead to sponsor-level escalation when business impact warrants it.

Quality assurance and release practices are treated as first-class parts of delivery. OctoAcme expects unit tests for new logic, integration tests where appropriate, and end-to-end smoke tests for critical flows, supported by CI that runs tests, linting, and security scanning before review/merge. PRs are kept small when possible, include linked issues and acceptance criteria, and require at least one approval per team policy. Releases follow a standardized checklist (CI/security green, release notes drafted, rollback plan documented, staging verification, post-deploy checks, and stakeholder announcements), and any incidents trigger rollback/triage plus a blameless retrospective with tracked action items.

---

## How to Use These Docs

Each document below covers a specific phase or aspect of OctoAcme's project management process. Start with the **Overview** for a high-level orientation, then explore the phase-specific guides relevant to where your project currently stands. The **Roles and Personas** doc is a useful reference throughout all phases.

---

## Documentation Index

| Document | Description |
|----------|-------------|
| [Project Management Overview](octoacme-project-management-overview.md) | High-level summary of the full project lifecycle and guiding principles |
| [Project Initiation Guide](octoacme-project-initiation.md) | How to validate a business need, align stakeholders, and create a project one-pager |
| [Project Planning](octoacme-project-planning.md) | Breaking work into shippable increments, estimates, Definition of Done, and backlog setup |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Daily standups, sprint rhythms, project board columns, and delivery rituals |
| [Risk Management & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, weekly status templates, and stakeholder communication cadences |
| [Release & Deployment Guide](octoacme-release-and-deployment.md) | Release checklist, staging verification, rollback plans, and post-deploy practices |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Sprint retrospectives, blameless post-mortems, and tracking improvement action items |
| [Roles and Personas](octoacme-roles-and-personas.md) | Definitions and responsibilities for PM, PdM, Developers, QA Lead, UX/UI Designer, Release Manager, and Stakeholder Representative |
| [RACI & Responsibility Matrix](octoacme-raci-and-responsibility-matrix.md) | Who owns what, RACI matrix, and lifecycle handoff checklists |
