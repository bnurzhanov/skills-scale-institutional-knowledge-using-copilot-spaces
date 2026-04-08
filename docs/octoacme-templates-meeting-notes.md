# OctoAcme — Meeting Notes Templates

## Purpose
Reduce meeting overhead and ensure consistent, actionable records for the recurring meetings in OctoAcme's project lifecycle.

## When to use
Use the appropriate template before each meeting to prepare an agenda and during (or immediately after) the meeting to capture notes and action items.

---

## Template 1: Project Kickoff Meeting

**Meeting type:** Project Kickoff  
**Date:** YYYY-MM-DD  
**Facilitator:** @name  
**Attendees:** @name, @name, …  
**Duration:** (actual)

### Agenda
1. Welcome & introductions (5 min)
2. Project overview — problem, goals, success metrics (10 min)
3. Roles & responsibilities (5 min)
4. Scope, timeline, and milestones (10 min)
5. Risks and dependencies (10 min)
6. Ways of working — standups, demos, communication channels (5 min)
7. Q&A and next steps (5 min)

### Notes
*(Capture key discussion points per agenda item)*

### Decisions Made
*(Copy rows into the [Decision Log](./octoacme-templates-decision-log.md))*

| Decision | Made By | Rationale |
|----------|---------|-----------|
|          |         |           |

### Action Items
*(Create as GitHub Issues and label `action-item`)*

| # | Action | Owner | Due Date | Issue Link |
|---|--------|-------|----------|------------|
| 1 |        |       |          |            |

---

## Template 2: Weekly Sync / Status Update

**Meeting type:** Weekly Sync  
**Date:** YYYY-MM-DD  
**Facilitator:** @name  
**Attendees:** @name, @name, …

### Status Summary
- **Overall health:** 🟢 On Track / 🟡 At Risk / 🔴 Off Track
- **Sprint / Iteration:** #N — Week N of N

### Progress This Week
*(List completed items, merged PRs, or milestones hit)*

- 

### Planned for Next Week
*(Key items expected to be completed or advanced)*

- 

### Risks & Blockers
*(Reference or update the [Risk Register](./octoacme-templates-risk-register.md))*

| Risk / Blocker | Owner | Status / Action |
|----------------|-------|-----------------|
|                |       |                 |

### Decisions Made
*(Log in [Decision Log](./octoacme-templates-decision-log.md) if significant)*

| Decision | Made By |
|----------|---------|
|          |         |

### Action Items
| # | Action | Owner | Due Date | Issue Link |
|---|--------|-------|----------|------------|
| 1 |        |       |          |            |

---

## Template 3: Sprint / Iteration Retrospective

**Meeting type:** Retrospective  
**Date:** YYYY-MM-DD  
**Facilitator:** @name  
**Attendees:** @name, @name, …  
**Sprint / Iteration:** #N

### What Went Well
*(Celebrate successes — keep these practices)*

- 

### What Could Be Improved
*(Honest observations — no blame, focus on process)*

- 

### Prioritized Action Items
*(Top 2–3 items; create as GitHub Issues labeled `retro-action` with an owner and due date)*

| # | Action Item | Owner | Due Date | GitHub Issue |
|---|-------------|-------|----------|--------------|
| 1 |             |       |          |              |
| 2 |             |       |          |              |
| 3 |             |       |          |              |

### Follow-up on Previous Action Items
| Issue | Action | Owner | Status |
|-------|--------|-------|--------|
|       |        |       | ✅ Done / 🔄 In Progress / ⏳ Overdue |

---

## Template 4: Ad-hoc / Stakeholder Update Meeting

**Meeting type:** Stakeholder Update / Ad-hoc  
**Date:** YYYY-MM-DD  
**Facilitator:** @name  
**Attendees:** @name, @name, …

### Purpose of this meeting
*(Why was this called? What needs to be communicated or decided?)*

### Key Updates
- 

### Risks Surfaced
- 

### Asks / Decisions Needed
*(Be explicit about what you need from attendees)*

| Ask | Owner | Deadline |
|-----|-------|----------|
|     |       |          |

### Action Items
| # | Action | Owner | Due Date |
|---|--------|-------|----------|
| 1 |        |       |          |

---

## Guidance for All Meeting Notes
- **Before:** Share the template/agenda at least 24 hours in advance for planned meetings.
- **During:** Assign a note-taker (rotate this role) and a timekeeper.
- **After:** Publish notes to the project's `docs/` folder or GitHub Discussions within 24 hours.
- **Action items:** Every action item must have an **owner** and a **due date**. Open as a GitHub Issue when appropriate (use label `action-item` or `retro-action`).

---

## References
- [Project Planning](./octoacme-project-planning.md) — kickoff guidance
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — weekly sync cadence
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — retro structure
- [Decision Log Template](./octoacme-templates-decision-log.md)
