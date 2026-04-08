# OctoAcme — Decision Log Template

## Purpose
Track significant project decisions in a lightweight, searchable log so that context is never lost, new team members can understand the "why," and audits are easy.

## When to use
Capture a decision when it meets **any** of the following criteria:
- It affects scope, architecture, or timeline
- Two or more options were seriously considered
- It was made by a group (meeting, async discussion) rather than one person alone
- It may need to be revisited or reversed in the future
- A stakeholder or auditor might ask "why did we choose this?"

> **Tip:** Decisions do NOT need to be perfect. Capture the decision made at the time with the information available. Update the status if it is later revised.

---

## Decision Log Table

Copy and paste the table below into your project's `docs/` folder or project README. Add a new row for each decision.

| ID | Date | Decision | Context / Problem | Options Considered | Decision Made By | Rationale | Status | Link |
|----|------|----------|--------------------|-------------------|-----------------|-----------|--------|------|
| DEC-001 | YYYY-MM-DD | Short title of the decision | Why did this need to be decided? | Option A, Option B, Option C | @person or meeting | Why this option was chosen over alternatives | Accepted / Superseded / Under Review | Issue or PR link |

---

## Field Definitions

| Field | Description |
|-------|-------------|
| **ID** | Sequential identifier (DEC-001, DEC-002, …). Prefix with project code if managing multiple projects. |
| **Date** | Date the decision was made (not when it was logged). |
| **Decision** | One-line title that clearly names what was decided. |
| **Context / Problem** | 1–3 sentences on the problem or question that prompted the decision. |
| **Options Considered** | List of the realistic alternatives that were evaluated. |
| **Decision Made By** | GitHub username(s) or meeting name (e.g., "Kickoff meeting 2025-01-10"). |
| **Rationale** | Key reason(s) the chosen option was selected. Be concise; link to a design doc for detail. |
| **Status** | `Accepted` (active), `Superseded` (replaced by another decision — link to it), or `Under Review`. |
| **Link** | Optional link to the GitHub Issue, PR, or discussion thread where the decision was recorded. |

---

## Example

| ID | Date | Decision | Context / Problem | Options Considered | Decision Made By | Rationale | Status | Link |
|----|------|----------|--------------------|-------------------|-----------------|-----------|--------|------|
| DEC-001 | 2025-01-15 | Use GitHub Actions for CI/CD | We needed an automated pipeline before the first release. | GitHub Actions, Jenkins, CircleCI | @pm-lead, @eng-lead | Native GitHub integration reduces setup overhead; team already familiar. | Accepted | #42 |
| DEC-002 | 2025-02-01 | Adopt feature flags for rollout | Needed to release incrementally without multiple branches. | Feature flags (LaunchDarkly), long-lived branches, per-region deploy | Architecture Review | Reduces branch complexity; allows instant rollback per user segment. | Accepted | #67 |

---

## Maintenance Guidance
- **Who updates it:** The PM or facilitator logs the decision within 24 hours of it being made.
- **Where it lives:** `docs/decision-log.md` in the project repository, or as a table in the project's main README.
- **Review cadence:** Skim the log at each retrospective to mark superseded entries and capture any undocumented decisions.

---

## References
- [Project Initiation](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)
