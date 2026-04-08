# OctoAcme — Definition of Ready & Definition of Done

## Purpose
Provide a single, authoritative reference for what "ready" and "done" mean at OctoAcme so that planning and execution use consistent quality gates.

## When to use
- **Definition of Ready (DoR):** Before pulling a backlog item into a sprint or iteration. Use during sprint planning to gate which items can be worked on.
- **Definition of Done (DoD):** Before closing an issue or merging a PR. Use during code review, QA, and release validation to confirm the work is truly complete.

---

## Definition of Ready (DoR)

A backlog item is **Ready** when all of the following are true:

- [ ] Title is clear and concise
- [ ] Problem statement or user story is written (`As a <role>, I want <goal> so that <reason>`)
- [ ] Acceptance criteria are defined and testable
- [ ] Dependencies are identified and either resolved or explicitly tracked
- [ ] Rough estimate (T-shirt or story points) has been applied
- [ ] Design or UX assets attached (if UI work)
- [ ] No blocking unknowns — open questions are documented and assigned

> **Tip:** If an item doesn't meet DoR, move it back to the backlog with a note on what's missing rather than pulling it into the sprint.

---

## Definition of Done (DoD)

A work item is **Done** when all of the following are true:

### Code & Tests
- [ ] Code implemented and peer-reviewed (at least one approval)
- [ ] All acceptance criteria verified by developer or QA
- [ ] Unit tests written and passing
- [ ] Integration or end-to-end tests passing (where applicable)
- [ ] No new linting or security scan failures introduced

### Documentation
- [ ] Inline code comments updated for complex logic
- [ ] User-facing docs or runbooks updated (if behavior changes)
- [ ] Release notes entry drafted (if customer-facing change)

### Tracking
- [ ] GitHub issue updated and linked to the merged PR
- [ ] Issue labeled and closed (or moved to "Done" column)
- [ ] Risk register updated if this item resolved or introduced a risk

### Release
- [ ] Deployed to staging and smoke-tested
- [ ] Stakeholder sign-off received (if required by acceptance criteria)

---

## References
- [Project Planning](./octoacme-project-planning.md) — references DoR/DoD during sprint planning
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — uses DoD to close issues and PRs
- [Risk Register Template](./octoacme-templates-risk-register.md)
