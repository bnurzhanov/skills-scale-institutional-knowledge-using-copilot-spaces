# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

---

## UX Designer

### Role Summary
UX Designers create user interface and experience designs that meet usability standards. They bridge the gap between user needs and technical implementation.

### Responsibilities
- Design wireframes, prototypes, and high-fidelity mockups
- Collaborate with Product Managers during requirements and with Developers during implementation
- Conduct usability reviews and incorporate stakeholder feedback before handoff to development
- Participate in acceptance testing to validate that the delivered UI matches the design intent

### Goals
- Ensure the product is intuitive and accessible
- Reduce rework by aligning design and implementation early
- Champion the end user's perspective throughout the project lifecycle

### Typical Communication
- Design reviews and prototype walkthroughs
- Async feedback in GitHub Issues or design tools (e.g., Figma comments)
- Attendance at kickoff and sprint reviews

---

## Business Analyst

### Role Summary
Business Analysts gather and translate business requirements into actionable specifications for the delivery team.

### Responsibilities
- Elicit and document requirements through workshops, interviews, and research
- Map business processes and translate needs into user stories and acceptance criteria
- Act as a liaison between stakeholders and the technical team
- Update documentation as business needs evolve throughout the project

### Goals
- Ensure business goals are accurately represented in the backlog
- Reduce ambiguity and rework through clear, testable acceptance criteria
- Support a smooth handoff between requirements and development

### Typical Communication
- Requirements workshops and backlog grooming sessions
- Written user stories and acceptance criteria in GitHub Issues
- Regular check-ins with PM and Product Manager to validate alignment

---

## Release Manager

### Role Summary
Release Managers plan, coordinate, and communicate releases across teams to ensure readiness and smooth deployments.

### Responsibilities
- Maintain the release calendar and coordinate release windows with engineering, QA, and support
- Confirm that all pre-release requirements are met (code, docs, infrastructure, security)
- Lead go/no-go decisions and communicate release status to stakeholders
- Facilitate post-release retros and track follow-up items

### Goals
- Deliver reliable, low-risk releases on schedule
- Minimize release-related incidents through preparation and coordination
- Maintain clear communication with all involved teams before, during, and after each release

### Typical Communication
- Release readiness reviews and go/no-go meetings
- Release announcements and post-deploy summaries
- Coordination via the [Release & Deployment Guide](./octoacme-release-and-deployment.md)

---

## Technical Writer

### Role Summary
Technical Writers document new features, update user guides and runbooks, and ensure all documentation is accurate and up to date for internal and external audiences.

### Responsibilities
- Write and maintain user-facing documentation, release notes, and runbooks
- Collaborate with Developers, QA, and PM to gather technical context and validate accuracy
- Review PRs and issues for documentation impact; flag gaps before release
- Maintain consistent terminology and formatting across the docs set

### Goals
- Ensure users and operators can successfully use and maintain the product
- Reduce support burden through clear, accurate documentation
- Keep the docs set aligned with the Definition of Done

### Typical Communication
- Async reviews of PRs and GitHub Issues
- Collaboration during sprint reviews to gather feature context
- Participation in release sign-off to confirm docs are complete

---

## Customer Support Lead

### Role Summary
Customer Support Leads represent the support team, relay customer feedback, and coordinate responses to user-facing issues post-release.

### Responsibilities
- Communicate feature changes or known issues to customers and the support team
- Surface customer feedback and recurring issues to the Product Manager for backlog consideration
- Coordinate with the Release Manager on support readiness for each release
- Participate in post-incident retrospectives to represent the customer impact

### Goals
- Minimize customer impact from bugs and regressions
- Provide rapid, accurate responses to customer issues
- Feed customer insights back into the product roadmap

### Typical Communication
- Participation in release readiness reviews
- Escalation of customer-critical issues to PM and engineering
- Regular feedback loops with Product Manager (monthly or per release)

---

## RACI — Responsibility Assignment

Use this mini-template to clarify who is **R**esponsible, **A**ccountable, **C**onsulted, and **I**nformed for key project decisions and activities.

| Activity | PM | PdM | Dev Lead | QA | UX | BA | Release Mgr | Tech Writer | Support Lead | Sponsor |
|----------|----|-----|----------|----|----|----|-------------|-------------|--------------|---------|
| Approve project charter | I | C | C | — | — | C | — | — | — | **A/R** |
| Prioritize backlog | C | **A/R** | C | C | C | C | — | — | I | I |
| Define acceptance criteria | C | **A** | C | C | C | **R** | — | — | C | — |
| Go/No-Go release decision | **R** | C | C | C | — | — | **A** | C | C | I |
| Publish release notes | C | C | C | C | — | — | C | **A/R** | I | I |
| Update risk register | **A/R** | C | C | — | — | — | C | — | — | I |
| Log decisions | **A/R** | C | C | — | — | — | — | — | — | I |
| Close project (sign-off) | **R** | C | C | — | — | — | C | — | — | **A** |

**Key:** R = Responsible (does the work) · A = Accountable (final decision/sign-off) · C = Consulted · I = Informed · — = Not involved

> Adapt this table to your project. Not every project will involve all roles.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

