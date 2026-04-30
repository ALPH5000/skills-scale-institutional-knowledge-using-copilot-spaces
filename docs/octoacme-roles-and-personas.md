# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA Lead

### Role Summary
The QA Lead owns the quality strategy for a project. They plan and oversee test execution across all phases, act as the quality gate before releases, and partner closely with Developers and the Release Manager to ensure readiness.

### Responsibilities
- Define and maintain the test plan, test cases, and acceptance criteria verification
- Coordinate manual and automated testing (unit, integration, regression, UAT)
- Track and report defects; triage severity with PM and Developers
- Confirm all acceptance criteria are met before sign-off
- Maintain CI quality gates and contribute to test automation strategy

### Goals
- Prevent defects from reaching production
- Reduce regression risk at each release
- Provide clear, timely quality signals to the team

### Typical Communication
- Sprint ceremonies and daily standups (blocker/defect status)
- QA sign-off reports shared with PM and Release Manager
- Defect triage discussions with Developers and PM

### Interactions & Hand-offs
- **← Developers**: receives feature branches and build artefacts for testing; returns defect reports
- **← Product Manager (PdM)**: receives acceptance criteria and user stories to derive test cases
- **→ Release Manager**: provides QA sign-off as a release gate; shares test summary reports
- **↔ Project Manager (PM)**: reports quality metrics, risks, and blocking defects; PM adjusts schedule as needed
- **← UX/UI Designer**: receives UX specifications to validate UI acceptance and accessibility

---

## UX/UI Designer

### Role Summary
The UX/UI Designer shapes the user experience and interface of features. They translate product requirements into wireframes, prototypes, and design specifications, ensuring that what is built is usable, accessible, and aligned with user needs.

### Responsibilities
- Conduct user research, create personas, and define user journeys
- Produce wireframes, mockups, and interactive prototypes
- Define and document UI/UX specifications and design tokens
- Collaborate in design reviews and provide feedback on implemented UI
- Ensure accessibility (WCAG) compliance in designs

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce rework by providing clear, developer-ready specifications
- Validate designs with real users before full implementation

### Typical Communication
- Design reviews with Developers and Product Manager
- Prototype walkthroughs with Stakeholder Representative
- Handoff notes and annotated designs shared in the project repo or design tool

### Interactions & Hand-offs
- **← Product Manager (PdM)**: receives feature requirements and user research insights; collaborates on problem framing
- **→ Developers**: delivers design specifications, assets, and interaction guidelines for implementation
- **→ QA Lead**: provides design specs and accessibility requirements to inform acceptance testing
- **↔ Stakeholder Representative**: presents prototypes for feedback and validation before development begins
- **↔ Project Manager (PM)**: aligns on design milestones and flags scope or timeline risks

---

## Release Manager

### Role Summary
The Release Manager coordinates and owns the end-to-end release process. They ensure releases are planned, communicated, and executed safely, with clear rollback plans and stakeholder notifications.

### Responsibilities
- Own the release calendar and deployment windows
- Coordinate release readiness checks across PM, QA Lead, and Developers
- Ensure rollback and incident plans are documented and understood
- Orchestrate staging deployments and production go/no-go decisions
- Communicate release status to stakeholders and support teams

### Goals
- Reduce release risk through clear gates and checklists
- Maintain a reliable, predictable release cadence
- Ensure every release has a documented rollback path

### Typical Communication
- Pre-release readiness meetings with PM, QA Lead, and Developers
- Release notes and deployment announcements to stakeholders
- Incident communications and post-release summaries

### Interactions & Hand-offs
- **← QA Lead**: receives QA sign-off report before go/no-go decision
- **← Developers**: confirms all PRs merged, CI green, and migration scripts ready
- **← Product Manager (PdM)**: receives feature descriptions for release notes; confirms scope
- **↔ Project Manager (PM)**: aligns on deployment window and communicates release status
- **→ Stakeholder Representative**: delivers release announcements and known issues summary

---

## Stakeholder Representative

### Role Summary
The Stakeholder Representative acts as the voice of the business or customer. They validate that the project is delivering real value, provide timely approvals, and ensure organisational alignment throughout the project lifecycle.

### Responsibilities
- Articulate business needs, constraints, and success criteria
- Review and approve project one-pagers, scope changes, and key deliverables
- Participate in sprint reviews and provide acceptance feedback
- Escalate business-level blockers and budget/resource decisions
- Champion the project within their organisation or business unit

### Goals
- Ensure the delivered solution meets business and customer needs
- Maintain executive visibility and support for the project
- Provide timely decisions to unblock the team

### Typical Communication
- Monthly (or milestone-based) status briefings from PM
- Sprint review demos and feedback sessions
- Ad-hoc escalation requests from PM when sponsor decisions are required

### Interactions & Hand-offs
- **← Project Manager (PM)**: receives weekly/milestone status reports; provides go/no-go decisions on scope changes
- **← Product Manager (PdM)**: receives roadmap updates and trade-off recommendations for approval
- **← Release Manager**: receives release announcements and post-release summaries
- **↔ UX/UI Designer**: reviews prototypes and provides business/customer feedback before development
- **→ PM / PdM**: surfaces new requirements, priorities, or constraints from the business

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [`octoacme-raci-and-responsibility-matrix.md`](octoacme-raci-and-responsibility-matrix.md) for a full RACI matrix and lifecycle handoff checklist.

