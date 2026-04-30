# Release & Deployment Checklist

Use this checklist for every release to ensure consistent, low-risk deployments. See [Release & Deployment Guide](../octoacme-release-and-deployment.md) for full guidance.

---

## Pre-Release Requirements

- [ ] All acceptance criteria for the release are met
- [ ] All PRs are merged to the release branch
- [ ] CI pipeline is passing (tests, lint, security scans)
- [ ] Release notes drafted and reviewed
- [ ] Rollback / mitigation plan documented and communicated
- [ ] Smoke test scripts prepared and ready to run
- [ ] Deployment window scheduled (if change-window policy applies)
- [ ] Dependent teams and support notified of upcoming release
- [ ] Database migrations or data changes reviewed and tested

## Staging Deployment & Verification

- [ ] Backup or snapshot taken (if applicable)
- [ ] Deployed to staging environment
- [ ] Smoke tests executed on staging and all passed
- [ ] Key user flows manually verified on staging
- [ ] Performance and error baselines checked on staging

## Production Deployment

- [ ] Deployed to production via automated pipeline (preferred) or manual runbook
- [ ] Deployment log recorded with timestamp and version

## Post-Release Verification

- [ ] Post-deploy smoke tests executed in production
- [ ] Key dashboards and alerts checked (errors, latency, usage)
- [ ] Release announced to stakeholders and support team
- [ ] Release notes published to the appropriate channel
- [ ] Rollback plan confirmed as no longer needed (or triggered if required)
- [ ] Incident log updated if any issues were encountered

---

**Owner:** DevOps Engineer (deployment steps) and Project Manager (coordination and announcements)  
**Related:** [Project Initiation Checklist](project-initiation-checklist.md) | [Weekly Status Template](../templates/weekly-status-template.md)
