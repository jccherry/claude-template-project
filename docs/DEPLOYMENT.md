# Deployment

## Overview

<!-- Describe the deployment targets and strategy: cloud provider, containerized, serverless, etc. -->

## Environments

| Environment | URL | Branch | Auto-deploy |
|-------------|-----|--------|-------------|
| Dev | <!-- https://dev.example.com --> | <!-- develop --> | <!-- Yes --> |
| Staging | <!-- https://staging.example.com --> | <!-- main --> | <!-- Yes --> |
| Production | <!-- https://example.com --> | <!-- release tags --> | <!-- No --> |

## Dev Deployment

```bash
# Deploy to dev
# npm run deploy:dev
```

<!-- Describe any manual steps, required env vars, or prerequisites. -->

## Staging Deployment

```bash
# Deploy to staging
# npm run deploy:staging
```

<!-- Describe the staging deployment process, approval gates, and verification steps. -->

## Production Deployment

```bash
# Deploy to production
# npm run deploy:prod
```

<!-- Describe the production deployment process, rollback procedure, and post-deploy verification. -->

## Infrastructure

<!-- Describe the infrastructure: servers, containers, load balancers, CDN, DNS. -->
<!-- Link to IaC (Terraform, Pulumi, CloudFormation) if applicable. -->

## Versioning

This project uses [Semantic Versioning](https://semver.org/). Tags are created automatically when PRs are merged to `main`.

| Label | Bump | Example |
|-------|------|---------|
| `semver:major` | Breaking change | `1.2.3` → `2.0.0` |
| `semver:minor` | New feature | `1.2.3` → `1.3.0` |
| `semver:patch` | Bug fix / chore | `1.2.3` → `1.2.4` |
| No label | Defaults to patch | `1.2.3` → `1.2.4` |

The auto-tagging workflow lives at `.github/workflows/auto-tag.yml`.

## CI/CD Pipeline

<!-- Describe the CI/CD flow from commit to production. -->

```
push → lint → test → build → merge → auto-tag → deploy
```

## Environment Variables

<!-- List all env vars needed for deployment, separated by environment if they differ. -->

| Variable | Dev | Staging | Production |
|----------|-----|---------|------------|
| <!-- API_URL --> | <!-- http://localhost:3000 --> | <!-- https://staging-api.example.com --> | <!-- https://api.example.com --> |

## Rollback

<!-- Describe how to rollback a bad deployment for each environment. -->

## Monitoring & Alerts

<!-- Describe monitoring tools, dashboards, and alerting setup. -->

## Notes

<!-- DNS, SSL certificates, scaling considerations, cost estimates. -->
