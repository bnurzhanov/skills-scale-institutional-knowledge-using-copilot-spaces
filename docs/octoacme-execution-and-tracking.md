# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
  - **WIP limits (recommended):** In Progress ≤ 2 per developer; In Review ≤ 3 per team. Adjust per sprint planning.
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
- **Issue hygiene:**
  - Every issue must have acceptance criteria before it can be moved to "In Progress" (see [Definition of Ready](./octoacme-templates-definition-of-ready-and-done.md))
  - Issues must be linked to the implementing PR and to the release milestone for traceability: Issue → PR → Release Notes
  - All issues must be labeled (e.g., `feature`, `bug`, `tech-debt`, `action-item`) and assigned an owner
- **Traceability:** Ensure that every user-facing change has a corresponding issue, a merged PR that references the issue (`Closes #N`), and a release notes entry. Use this chain to audit what shipped in each release.

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
- [ ] [Risk Register](./octoacme-templates-risk-register.md) updated weekly
- [ ] All issues have acceptance criteria before moving to "In Progress"
- [ ] Issue → PR → Release Notes traceability enforced
- [ ] WIP limits agreed and visible on the project board
- [ ] [Weekly sync notes](./octoacme-templates-meeting-notes.md) published within 24 hours
