# OctoAcme — Project Closeout

## Purpose
Ensure every project ends with proper handoff, documentation, metrics readout, and captured learnings so that nothing falls through the cracks after the last release.

## When to use
After the final release has been successfully deployed and verified, and before the project team disbands or moves to the next initiative.

---

## Closeout Checklist

### 1. Handoff & Knowledge Transfer
- [ ] Runbook / operational documentation is up to date and accessible to the support/ops team
- [ ] Ownership of the service or feature is formally transferred (new owner acknowledged in writing)
- [ ] All credentials, access tokens, and secrets are rotated or transferred to the new owner
- [ ] Architecture diagram and dependency map are current
- [ ] On-call rotation updated (if applicable)

### 2. Documentation
- [ ] Project README reflects the final state of the project
- [ ] Decision Log entries are reviewed; superseded decisions are marked
- [ ] Risk Register final status updated (all risks marked Closed or transitioned to the owning team)
- [ ] Release notes for all releases published and linked from the project README
- [ ] Any temporary workarounds or technical debt items logged as GitHub Issues with label `tech-debt`

### 3. Metrics Readout
- [ ] Success metrics (from the Project One-pager) measured and documented
- [ ] Velocity and delivery metrics summarized (sprints completed, story points delivered, defect rate)
- [ ] Customer or stakeholder satisfaction signal captured (survey, NPS, support ticket trends)
- [ ] Comparison of planned vs. actual timeline and scope documented

### 4. Retrospective & Action Items
- [ ] Final retrospective held (use the [Retrospective template](./octoacme-retrospective-and-continuous-improvement.md))
- [ ] All retrospective action items created as GitHub Issues (label `retro-action`, owner and due date assigned)
- [ ] Outstanding action items from earlier retros reviewed — resolved or transitioned

### 5. Issue & Board Hygiene
- [ ] All open GitHub Issues reviewed: closed, deferred, or transferred to a new project/milestone
- [ ] Project board archived or closed
- [ ] Stale branches cleaned up (merged and deleted)
- [ ] CI/CD pipelines disabled or transferred for archived repositories

### 6. Stakeholder Communication
- [ ] Project closeout announcement sent to stakeholders (see template below)
- [ ] Final status report published (link to metrics readout and retrospective notes)
- [ ] Support team briefed on any known issues or escalation paths post-launch

---

## Project Closeout Communication Template

Use this template for the final stakeholder announcement email or Slack message.

```
Subject: [Project Name] — Project Closeout & Summary

Hi [stakeholder group],

We're pleased to announce the successful completion of [Project Name].

**What we shipped:**
- [Key feature or outcome 1]
- [Key feature or outcome 2]

**Key metrics:**
- [Success metric 1]: [Result]
- [Success metric 2]: [Result]

**Timeline:** [Planned] → [Actual]

**What's next:**
- [Owner/team] will handle ongoing support and operations.
- Outstanding items have been captured as GitHub Issues: [link]
- Retrospective notes are available here: [link]

Thank you to everyone who contributed!

[PM Name]
```

---

## Closeout Sign-off

| Role | Name | Date | Sign-off |
|------|------|------|----------|
| Project Manager | | | ☐ |
| Product Manager | | | ☐ |
| Engineering Lead | | | ☐ |
| Operations / Support Lead | | | ☐ |
| Sponsor / Stakeholder | | | ☐ |

---

## References
- [Project Initiation](./octoacme-project-initiation.md) — original One-pager and success metrics
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Risk Register Template](./octoacme-templates-risk-register.md)
- [Decision Log Template](./octoacme-templates-decision-log.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
