# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Release Readiness Checklist

Complete this checklist before the go/no-go decision. Ownership is noted for each item.

| # | Item | Owner |
|---|---|---|
| 1 | All in-scope acceptance criteria verified and QA sign-off report produced | QA Lead |
| 2 | All PRs merged and CI/CD pipeline green (tests, lint, security scans) | Developers |
| 3 | Release notes drafted and reviewed | Release Manager + PM |
| 4 | Rollback / mitigation plan documented and communicated to the team | Release Manager |
| 5 | Smoke tests executed against staging environment | QA Lead + Release Manager |
| 6 | Deployment window confirmed and stakeholders notified | PM + Release Manager |
| 7 | Support team briefed on new features and known issues | PM |
| 8 | Go/no-go decision recorded | PM (decision), Release Manager (execution) |

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
