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

## Scrum Master

### Role Summary
The Scrum Master facilitates agile ceremonies, removes blockers, and coaches the team on continuous process improvement. They act as a neutral process guide and servant-leader for the delivery team.

### Responsibilities
- Facilitate sprint planning, daily standups, sprint reviews, and retrospectives
- Identify and remove impediments blocking the team
- Coach team members on agile principles and practices
- Shield the team from external interruptions during a sprint
- Track and communicate team velocity and process health

### Goals
- Maintain a healthy, predictable delivery cadence
- Foster a culture of continuous improvement
- Ensure ceremonies are effective and time-boxed

### Interactions with Other Roles
- **PM**: Coordinates on schedule, risks, and cross-team dependencies; Scrum Master owns the ceremony rhythm while PM owns the overall timeline
- **PdM**: Ensures the backlog is groomed and prioritized before sprint planning
- **Developers**: Directly supports daily unblocking and sprint focus
- **QA**: Ensures QA capacity is factored into sprint commitments
- **Stakeholders**: Invites stakeholders to sprint reviews; escalates blockers that require sponsor involvement through PM

### Artifact Ownership
- Retrospective notes and action item log (owns facilitation and follow-up)
- Sprint velocity tracking

---

## UX Designer

### Role Summary
The UX Designer owns the user experience and visual design of the product, ensures usability feedback loops with real users, and validates that delivered features meet human-centered design standards.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, prototypes, and design specifications
- Define and maintain design system components and standards
- Review implemented features against design acceptance criteria
- Advocate for accessibility and inclusive design

### Goals
- Ensure delivered features are intuitive and meet user needs
- Reduce rework caused by late-stage usability issues
- Maintain visual and interaction consistency across the product

### Interactions with Other Roles
- **PdM**: Collaborates on problem framing, user research synthesis, and feature trade-offs
- **Developers**: Provides annotated specs and is available to answer design questions during implementation; reviews PRs for UX fidelity
- **QA**: Shares design acceptance criteria; participates in UX-specific test scenarios
- **PM**: Flags design dependencies and timeline risks (e.g., research cycles)
- **Stakeholders**: Presents research findings and design proposals for feedback and sign-off

### Artifact Ownership
- UX research summaries and usability test reports
- Design files and prototypes (linked from backlog items)

---

## DevOps Engineer

### Role Summary
The DevOps Engineer manages CI/CD pipelines, deployment operations, and infrastructure as code. They partner with developers and QA to enable reliable, repeatable releases and maintain a healthy production environment.

### Responsibilities
- Build, maintain, and improve CI/CD pipelines
- Manage infrastructure provisioning and configuration (IaC)
- Monitor production health (uptime, latency, error rates) and respond to incidents
- Coordinate deployment windows and rollback procedures with PM
- Enforce security scanning and compliance gates in the pipeline
- Document runbooks and incident playbooks

### Goals
- Minimize deployment risk and mean time to recovery (MTTR)
- Increase deployment frequency through automation
- Maintain high environment stability and observability

### Interactions with Other Roles
- **PM**: Aligns on release readiness and deployment scheduling; owns the CI/CD sections of the release checklist
- **Developers**: Reviews infrastructure requirements in design docs; approves IaC changes
- **QA**: Provides staging environments and automated test integration hooks
- **Support Lead**: Escalates production incidents and ensures runbooks are current
- **Stakeholders**: Reports on environment health and release readiness

### Artifact Ownership
- CI/CD pipeline configuration and runbooks
- Infrastructure-as-code repository and deployment logs
- See [docs/checklists/release-and-deployment-checklist.md](checklists/release-and-deployment-checklist.md) for pre/post-release steps owned by this role

---

## Support Lead

### Role Summary
The Support Lead is the primary contact for customer feedback, support escalations, and post-release incident management. They bridge the gap between users, the product team, and engineering to ensure issues are triaged and resolved quickly.

### Responsibilities
- Triage and prioritize incoming support tickets and customer escalations
- Reproduce and document bugs for the development team
- Communicate status updates and workarounds to affected customers
- Collaborate with DevOps and developers on incident response and root-cause analysis
- Track recurring issues and surface them as product improvement requests to PdM

### Goals
- Minimize customer impact and resolution time for production issues
- Provide timely, accurate communication to stakeholders during incidents
- Convert support insights into actionable product feedback

### Interactions with Other Roles
- **PM**: Reports on open incidents and escalates high-severity issues; co-owns post-release verification
- **PdM**: Surfaces recurring pain points as prioritization inputs for the backlog
- **Developers**: Works directly with engineers during incident triage and hotfix cycles
- **DevOps Engineer**: Coordinates on incident response runbooks and rollback decisions
- **QA**: Shares reproduction steps; collaborates on regression test coverage for fixed bugs
- **Stakeholders**: Sends incident communications and post-mortems

### Artifact Ownership
- Incident log and post-mortem reports
- Customer-facing status communications

---

## Product Designer

### Role Summary
The Product Designer bridges strategy and execution by translating product requirements into end-to-end product experiences. They work alongside the UX Designer (or may encompass UX in smaller teams) with a focus on interaction design, information architecture, and design system consistency.

### Responsibilities
- Define information architecture and user flows for new features
- Produce high-fidelity mockups and interactive prototypes
- Maintain the product design system and component library
- Run design critique sessions and incorporate feedback
- Partner with PdM to shape feature requirements from a user perspective

### Goals
- Deliver cohesive, high-quality product experiences
- Reduce design debt through a maintained design system
- Accelerate development velocity by providing clear, complete design specifications

### Interactions with Other Roles
- **PdM**: Co-develops feature definitions; translates user stories into design requirements
- **UX Designer**: Divides research and visual execution (in larger teams); shares findings and prototypes
- **Developers**: Hands off annotated specs; participates in implementation reviews
- **QA**: Provides visual acceptance criteria for automated and manual testing
- **PM**: Communicates design milestones and flags timeline risks

### Artifact Ownership
- Product design system documentation
- Feature-level design specs and prototype links (attached to backlog items)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

