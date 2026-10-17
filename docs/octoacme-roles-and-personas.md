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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Suggested Personas (proposed additions)

The following personas are proposed to improve clarity and accountability for cross-cutting and operational responsibilities. For each persona below: responsibilities, when they should be consulted, typical meetings or touchpoints, and example acceptance criteria are indicated.

### Program Director
- Responsibilities
  - Own program-level outcomes across multiple projects.
  - Prioritize inter-project dependencies and allocate program resources.
  - Coordinate with Product Leads and Sponsors on strategy and roadmap trade-offs.
- When to consult
  - When initiatives span multiple projects or teams, or when prioritization conflicts arise across projects.
- Typical touchpoints
  - Weekly syncs with PMs, monthly sponsor reviews, quarterly roadmap planning.
- Interactions with existing roles
  - PMs: align on delivery timelines and resolve cross-project conflicts.
  - PdMs: coordinate prioritization across product lines.
  - Sponsors: update strategic progress and solicit guidance.
- Example acceptance criteria
  - Program roadmap published and approved by sponsors.
  - Cross-project dependencies documented and owned.

### Technical Lead (Tech Lead)
- Responsibilities
  - Own architecture and technical direction for a project or large feature.
  - Mentor developers and ensure code quality and maintainability.
  - Drive non-functional requirement decisions (scalability, security, performance).
- When to consult
  - During design, architecture reviews, and when resolving complex technical trade-offs.
- Typical touchpoints
  - Architecture reviews, sprint planning, design docs, code review cycles.
- Interactions with existing roles
  - Developers: provide technical guidance and review designs.
  - PM/PdM: advise on technical trade-offs and effort estimates.
  - QA: coordinate on test strategies for non-functional requirements.
- Example acceptance criteria
  - Architecture review completed with documented decisions and trade-offs.
  - Implementation meets agreed non-functional benchmarks.

### Release / Platform Engineer
- Responsibilities
  - Own release pipelines, deployment automation, rollback procedures, and observability setup.
  - Ensure deployment safety and validate release readiness checklists.
- When to consult
  - Prior to any release, when changing deployment pipelines, or when improving observability/monitoring.
- Typical touchpoints
  - Release readiness meetings, CI/CD pipeline reviews, post-deploy verifications.
- Interactions with existing roles
  - Developers: coordinate for release automation hooks and instrumentation.
  - QA: ensure release steps align with test/verification plans.
  - On-call/Support: validate runbooks and rollback procedures.
- Example acceptance criteria
  - Release pipeline validated in staging and rollback tested.
  - Monitoring and alerting configured for new features.

### UX Researcher / Designer
- Responsibilities
  - Lead user research, synthesize findings, and inform acceptance criteria with UX signals.
  - Produce design artifacts and ensure usability goals are met.
- When to consult
  - During discovery, before defining acceptance criteria for user-facing features, and during pre-release validations.
- Typical touchpoints
  - Discovery sessions with PdM, design reviews, usability testing, handoffs to engineering.
- Interactions with existing roles
  - PdM: define user needs and acceptance criteria.
  - Developers: clarify design intent and implementation constraints.
  - QA: help define UX acceptance tests and criteria.
- Example acceptance criteria
  - Usability test results meet target success rates.
  - Design artifacts and accessibility checks documented.

### Data Analyst / Measurement Lead
- Responsibilities
  - Define metrics, dashboards, and instrumentation needed to validate success criteria.
  - Support experiments, A/B testing, and post-release analysis.
- When to consult
  - When defining success metrics, planning experiments, or interpreting release impact.
- Typical touchpoints
  - Metrics review sessions, launch analysis meetings, instrumentation planning.
- Interactions with existing roles
  - PdM: align on success metrics and analysis plans.
  - PM: report on outcome metrics and status.
  - Engineers: coordinate instrumentation and data collection.
- Example acceptance criteria
  - Dashboards for key metrics are in place before release.
  - Instrumentation implemented and validated in staging.

### Security / Compliance Liaison
- Responsibilities
  - Act as the primary point of contact for security reviews, threat modeling, and compliance assessments.
  - Ensure security requirements and mitigations are tracked and implemented.
- When to consult
  - At design time for sensitive features, before production release for compliance checks, and during incident response.
- Typical touchpoints
  - Security review meetings, threat modeling sessions, compliance audits.
- Interactions with existing roles
  - Security team: escalate complex issues and request formal reviews.
  - Tech Lead: implement mitigations and architecture changes.
  - PM: inform risk and mitigation plans.
- Example acceptance criteria
  - Security review completed with no blocking issues or documented mitigations.
  - Compliance requirements captured and addressed.

### Support / Customer Success Lead
- Responsibilities
  - Provide customer-impact insights, coordinate support handoffs, and validate operational runbooks.
  - Triage and prioritize customer-reported issues and feedback to product/engineering.
- When to consult
  - During release planning for customer-impacting features, and after release for support readiness.
- Typical touchpoints
  - Release readiness reviews, weekly feedback syncs, incident post-mortems.
- Interactions with existing roles
  - PM: prioritize customer issues and feedback.
  - PdM: feed user insights and suggest product adjustments.
  - On-call/Support teams: ensure runbooks and escalation paths are adequate.
- Example acceptance criteria
  - Support runbooks created and validated.
  - Known customer-impact queries documented and assigned.

---

## How to integrate these personas into existing docs & process

- For each new persona add:
  - A concise Role Summary and Responsibilities section.
  - Clear guidance on typical consultation points (when to involve them).
  - Touchpoints and meeting cadence (e.g., Release Engineer attends release readiness).
  - Example acceptance criteria or sign-off requirements (e.g., Security Liaison sign-off).
- Update project templates (e.g., release checklists, PR templates, runbooks) to include relevant sign-offs or contact fields for the new personas.
- Suggested rollout:
  1. Draft the new persona entries into docs/octoacme-roles-and-personas.md.
  2. Review with PMs, PdMs, Tech Leads, Security, and Support for alignment.
  3. Publish updated doc and communicate changes in the weekly PM sync.

