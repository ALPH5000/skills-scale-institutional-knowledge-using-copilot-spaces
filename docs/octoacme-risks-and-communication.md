# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication

- Identify stakeholder groups and communication needs (e.g., engineering, sales, support, Stakeholder Representative)
- **PM** is the primary owner of delivery communications (status reports, risk escalations)
- **PdM** owns product-level communications (roadmap updates, feature trade-offs)
- **Stakeholder Representative** owns business-level approvals and organisational alignment
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status

## Communication Templates
Weekly Status Template:
- Progress this week:
- Next steps:
- Risks & blockers:
- Ask / decisions needed:

Incident Communication
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled

## Escalation Paths

| Level | Trigger | Owner | Action |
|---|---|---|---|
| 1 — Team triage | Day-to-day blocker | PM | Raise in daily standup; resolve within the sprint |
| 2 — Delivery escalation | Blocker risks sprint goal or milestone | PM | PM escalates to Product Lead and dependent teams; update risk register |
| 3 — Business escalation | Blocker risks delivery date or budget | PM + PdM | PM escalates to Stakeholder Representative; schedule urgent alignment |
| 4 — Security / compliance | Security or compliance incident | PM + Security on-call | Follow security incident runbook; notify Security on-call immediately |

> **PM** owns escalation tracking and ensures each open escalation has a documented owner and target resolution date. **PdM** and **Stakeholder Representative** own business-level decisions triggered by Level 3 escalations.

