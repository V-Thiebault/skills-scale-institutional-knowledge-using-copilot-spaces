# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (DevOps Engineer verifies)
- Release notes drafted (Project Manager coordinates)
- Rollback / mitigation plan documented (DevOps Engineer prepares)
- Smoke tests prepared (QA and DevOps Engineer collaborate)
- Analytics tracking verified for new features (Data Analyst confirms)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — Project Manager coordinates
- [ ] Backup or snapshot (if applicable) — DevOps Engineer executes
- [ ] Deploy to staging and run smoke tests — DevOps Engineer and QA
- [ ] UX Designer reviews staging for design consistency and usability
- [ ] Deploy to production (automated pipeline preferred) — DevOps Engineer monitors
- [ ] Run post-deploy verifications — DevOps Engineer and Data Analyst validate metrics
- [ ] Announce release to stakeholders and support — Project Manager communicates

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (DevOps Engineer leads response)
  - Rollback to last known-good release if necessary (DevOps Engineer executes)
  - Triage root cause and capture action items (Scrum Master facilitates retrospective)
  - Data Analyst monitors impact metrics during and after incident

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
