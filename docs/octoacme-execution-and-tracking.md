# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies (facilitated by Scrum Master)
- Weekly delivery sync — show progress, updates, and flagged risks (Project Manager coordinates)
- Demo/Review at the end of each sprint or milestone (UX Designer presents designs, Developers demo features, Data Analyst shares metrics)

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review (DevOps Engineer maintains CI pipelines)
  - Request design review from UX Designer when UI/UX changes are involved
  - Require at least one approval before merging (or team-defined policy)
  - Ensure analytics events are properly instrumented (Data Analyst reviews tracking implementation)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown (Scrum Master monitors and reports)
- Monitor success metrics identified in the Project One-pager (Data Analyst provides regular reports)
- Use dashboards for key signals (errors, latency, usage) — DevOps Engineer maintains observability
- Review usability metrics and user feedback (UX Designer analyzes and presents findings)

## Blocker Escalation
- Level 1: Team-level triage in daily standup (Scrum Master facilitates resolution)
- Level 2: PM escalates to Product Lead and dependent teams (DevOps Engineer engaged for infrastructure blockers)
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint (DevOps Engineer responsible)
- [ ] Design handoff process established (UX Designer provides specs and assets)
- [ ] Analytics instrumentation verified (Data Analyst confirms tracking completeness)
- [ ] Regular demos scheduled (Scrum Master facilitates)
- [ ] Risk register updated weekly
