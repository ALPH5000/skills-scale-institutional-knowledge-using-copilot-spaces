# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Project Board Columns

| Column | Definition | Who moves items here |
|---|---|---|
| **Backlog** | Accepted but not yet scheduled | PdM / PM |
| **Ready** | Refined, estimated, and ready to pull into a sprint | PM (sprint planning) |
| **In Progress** | Actively being developed | Developer (self-assigned) |
| **In Review** | PR open and awaiting code review | Developer (on PR open) |
| **QA** | Code merged; awaiting QA/test sign-off | Developer (after PR merge) |
| **Done** | Acceptance criteria verified and QA sign-off given | QA Lead |

> Items move to **QA** only after the PR is merged and CI is green. The **QA Lead** is responsible for pulling items through the QA column and moving them to Done after verification. Defects found in QA re-open the original issue or create a new linked defect issue; the item stays in QA until resolved.

## Workflows
- Use the project board (e.g., GitHub Projects) with columns defined above
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
