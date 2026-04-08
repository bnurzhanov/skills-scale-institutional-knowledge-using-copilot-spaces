# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with the fields below. Use the copy/paste-ready [Risk Register Template](./octoacme-templates-risk-register.md) for a full template with examples and a scoring matrix.
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Risk Score (Impact × Likelihood)
- Owner
- Mitigation plan
- Contingency plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates on a defined cadence:
  - **Weekly:** PM sends a status update to the delivery team and key stakeholders using the Weekly Status Template below
  - **Milestone-based:** Broader stakeholder update at each milestone or release
  - **Incident-based:** Immediate communication when a critical risk materializes (see Incident Communication template)
- **Single source of truth:** The project README or a `docs/status-updates/` folder is the canonical location for status updates. Do not maintain parallel status threads in chat — link to the source of truth from Slack/Teams.
- Use the [Meeting Notes template](./octoacme-templates-meeting-notes.md) for weekly sync notes to reduce duplication.

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
- Team-level -> PM -> Product Lead -> Sponsor
- For security incidents, follow the security incident runbook and notify Security on-call
