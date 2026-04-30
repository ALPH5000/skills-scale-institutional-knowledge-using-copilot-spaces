# OctoAcme — RACI & Responsibility Matrix

## Purpose
Define who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for key activities across the project lifecycle, and provide a clear handoff checklist for each phase.

> **RACI key**
> - **R** — Responsible: does the work
> - **A** — Accountable: owns the outcome; one person per activity
> - **C** — Consulted: provides input before/during; two-way communication
> - **I** — Informed: kept up to date; one-way communication

---

## RACI Matrix

| Activity | PM | PdM | Developer | QA Lead | UX/UI Designer | Release Manager | Stakeholder Rep |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Define project one-pager / charter | A | C | I | I | I | I | C |
| Stakeholder alignment & approvals | R | C | I | I | I | I | A |
| Backlog prioritisation | C | A | C | C | C | I | C |
| Acceptance criteria authoring | C | A | C | C | R | I | C |
| UX research & wireframes | I | C | C | I | A | I | C |
| Design specification handoff | I | C | R | C | A | I | I |
| Sprint planning | A | C | R | C | C | I | I |
| Feature implementation | I | C | A | C | C | I | I |
| Test planning & execution | C | C | C | A | C | I | I |
| Defect triage | C | C | R | A | I | I | I |
| QA sign-off | I | I | I | A | I | R | I |
| Release readiness check | A | C | C | R | I | R | I |
| Production deployment | I | I | C | C | I | A | I |
| Release communication | C | C | I | I | I | R | I |
| Risk register maintenance | A | C | C | C | I | I | I |
| Escalation (team-level blocker) | A | C | C | I | I | I | I |
| Escalation (business-level blocker) | R | C | I | I | I | I | A |
| Sprint retrospective facilitation | A | C | R | C | C | C | I |
| Retrospective action item tracking | A | I | C | C | C | C | I |

---

## Lifecycle Handoff Checklist

Use this checklist to confirm readiness before moving to the next phase. The accountable role for each gate is noted in parentheses.

### Phase 1 → Phase 2: Initiation → Planning

- [ ] Project one-pager drafted and reviewed by PdM and Stakeholder Rep (PM)
- [ ] Problem statement, success metrics, and high-level timeline agreed (PM + PdM)
- [ ] Key stakeholders identified and communication cadence agreed (PM)
- [ ] Initial risk register created with at least a first pass on High-impact items (PM)
- [ ] Stakeholder Representative sign-off obtained to proceed (Stakeholder Rep)

### Phase 2 → Phase 3: Planning → Execution

- [ ] Backlog items broken into shippable increments with acceptance criteria (PdM)
- [ ] Definition of Done documented and agreed by team (PM + Developers)
- [ ] UX/UI designs for first sprint ready and handed off to Developers (UX/UI Designer)
- [ ] Test plan drafted, covering unit, integration, and UAT scope (QA Lead)
- [ ] CI pipeline configured: automated tests, linting, and security scanning (Developers)
- [ ] Sprint 1 kick-off completed (PM)

### Phase 3 → Phase 4: Execution → Release

- [ ] All in-scope acceptance criteria met and verified by QA Lead (QA Lead)
- [ ] QA sign-off report produced and shared with Release Manager and PM (QA Lead)
- [ ] All PRs merged; CI/CD pipeline green (Developers)
- [ ] Release notes drafted and reviewed by PM and PdM (Release Manager)
- [ ] Rollback plan documented and communicated to the team (Release Manager)
- [ ] Deployment window confirmed with Stakeholder Rep (PM + Release Manager)
- [ ] Staging deployment completed and smoke tests passed (Release Manager + QA Lead)

### Phase 4 → Phase 5: Release → Retrospective

- [ ] Production deployment completed and post-deploy verifications passed (Release Manager)
- [ ] Release announcement sent to stakeholders and support (Release Manager)
- [ ] Any post-release incidents logged and triaged (PM)
- [ ] Sprint / release metrics captured (velocity, defect rate, cycle time) (PM)
- [ ] Retrospective scheduled within one week of release (PM)

### Phase 5: Retrospective → Closed

- [ ] Retrospective facilitated; outcomes documented (PM)
- [ ] Action items assigned with owners and target dates (PM)
- [ ] Action items added to next sprint/planning cycle backlog (PdM + PM)
- [ ] Project charter / one-pager updated with learnings (PM)
- [ ] Final status report shared with Stakeholder Rep (PM)

---

## Who Owns What — Quick Reference

| Artifact / Decision | Owner |
|---|---|
| Project charter / one-pager | PM (accountable), PdM (consulted) |
| Product roadmap & backlog | PdM |
| Sprint plan & timeline | PM |
| Acceptance criteria | PdM (with UX/UI Designer input) |
| UX/UI specifications | UX/UI Designer |
| Test plan & QA sign-off | QA Lead |
| Risk register | PM |
| Release calendar & deployment | Release Manager |
| Release notes | Release Manager (drafted), PM (approved) |
| Escalation decisions (business) | Stakeholder Representative |
| Escalation decisions (delivery) | PM |
| Retrospective action items | PM (tracking), whole team (ownership) |
