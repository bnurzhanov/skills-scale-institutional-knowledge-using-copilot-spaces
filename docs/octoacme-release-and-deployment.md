# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged (verified against [Definition of Done](./octoacme-templates-definition-of-ready-and-done.md))
- Passing CI and security scans
- Release notes drafted (Issue → PR → Release Notes traceability complete)
- Rollback / mitigation plan documented
- Smoke tests prepared

## Go / No-Go Checklist

Run this check with the Release Manager, PM, and QA lead before every release to production.

| # | Check | Owner | Status |
|---|-------|-------|--------|
| 1 | All PRs for this release are merged and CI is green | Eng Lead | ☐ |
| 2 | All acceptance criteria verified (QA sign-off) | QA | ☐ |
| 3 | Security scan passed; no critical vulnerabilities open | Security / Eng | ☐ |
| 4 | Release notes drafted and reviewed | Tech Writer / PM | ☐ |
| 5 | Staging deploy completed and smoke tests passing | Eng Lead / QA | ☐ |
| 6 | Rollback plan documented and tested | Eng Lead | ☐ |
| 7 | Support team briefed on changes and known issues | Release Mgr | ☐ |
| 8 | Deployment window confirmed and comms sent | PM / Release Mgr | ☐ |
| 9 | Monitoring and alerting in place for the new release | Eng Lead | ☐ |

**Decision:** Go ☐ / No-Go ☐  
**Decision made by:** @name  
**Date:** YYYY-MM-DD  
**Notes (if No-Go):**

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
  - **Send a rollback communication** to stakeholders and support within 30 minutes using the template below:

```
Subject: [Service Name] Rollback — [Date]

We have rolled back [Service Name] to [version] due to [brief description].

Impact: [Who/what was affected and for how long]
Status: [Current state — stable / investigating]
Next steps: [Timeline and plan to re-release with fix]
Updates: [Where stakeholders can follow progress]

[PM / On-call name]
```

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
