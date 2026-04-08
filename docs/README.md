# OctoAcme Project Management Docs

This README provides a concise overview of OctoAcme's project management processes and quick links to all standardized process documents for project delivery, execution, and improvement.

---

## Overview of OctoAcme Project Management Processes

OctoAcme's project management approach follows a lightweight, end-to-end lifecycle designed to keep ownership clear and delivery iterative. Work moves through five phases: **Initiation** (confirm the problem, stakeholders, success metrics, and a high-level timeline), **Planning** (turn the approved initiative into a prioritized backlog with acceptance criteria, estimates, dependencies, and a Definition of Done), **Execution** (build, test, and review in small increments using a project board with a Backlog → Ready → In Progress → In Review → QA → Done flow), **Release** (deploy with safeguards and clear release notes), and **Retrospective/Continuous Improvement** (capture learnings and feed improvements back into the backlog). This structure is consistent across cross-functional projects while allowing teams to adapt cadence and artifacts to project size.

Roles are explicitly defined to avoid ambiguity. **Project Managers (PM)** coordinate timelines, risks, dependencies, and communications. **Product Managers (PdM)** define outcomes, prioritize the backlog, and measure success. **Developers** implement features with testability and maintainability in mind. **QA/Testing** validates acceptance criteria and overall quality. **Stakeholders** contribute inputs and approvals. Each project has a named PM and Product Lead to ensure clear ownership and data-informed decisions via success metrics established early in the Project Charter/One-pager.

Communication and execution are driven by a predictable team rhythm: daily standups for blocker and dependency surfacing, a weekly PM + PdM sync, and monthly stakeholder updates. Risks are tracked in a simple risk register (impact/likelihood/owner/mitigation/status) and reviewed at weekly syncs. Escalation follows a defined path—team triage → PM → Product Lead → Sponsor—with a separate security incident runbook for security issues. Status updates use a consistent template highlighting progress, next steps, risks/blockers, and explicit asks/decisions needed.

Quality assurance is built into both development and release practices. OctoAcme encourages **small pull requests** linked to issues and acceptance criteria, with CI (tests, lint, security scanning) required to pass before review and at least one approval per team policy. Testing is layered—unit tests for new logic, integration tests where needed, and end-to-end smoke tests for critical flows prior to release. Releases are standardized with pre-release requirements (acceptance criteria met, scans passing, release notes drafted, rollback plan documented), a deployment checklist (staging verification, production deploy, post-deploy checks), and an incident/rollback playbook followed by blameless retrospectives with owned action items and due dates.

---

## Docs Index

| Document | Description |
|---|---|
| [Overview](./octoacme-project-management-overview.md) | Principles, core roles, lifecycle, key artifacts, and communication cadence |
| [Project Initiation Guide](./octoacme-project-initiation.md) | How to kick off a project: charter, stakeholders, success metrics |
| [Project Planning](./octoacme-project-planning.md) | Backlog, milestones, dependencies, Definition of Done |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Project boards, PR workflow, standups, status reporting |
| [Risk Management & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation paths, communication templates |
| [Release & Deployment Guide](./octoacme-release-and-deployment.md) | Release types, deployment checklist, rollback playbook |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retrospective format, action items, improvement tracking |
| [Roles & Personas](./octoacme-roles-and-personas.md) | Detailed responsibilities for PM, PdM, Developers, and QA |

---

See each document for detailed checklists, templates, and actionable guidance.
