# DePay Publication Checklist

## Content accuracy

- [x] Described as the public pilot component of a startup, based on the developer's clarification
- [x] Described as previous work by an Oferli technical team member
- [x] No claim that Oferli originally built the project
- [x] No invented client name, dates, scale, revenue, adoption, or performance metrics
- [x] Remaining unknowns are omitted or clearly described as not publicly confirmed
- [x] Original problem confirmed as cryptocurrency payment through specialized terminals
- [x] Backend & DevOps role and technical contribution confirmed by the developer
- [x] Real transactions described only as pilot testing, without scale or commercial claims
- [x] Provider adapters described as configurable/local rather than proof of live production processing
- [x] No source-code excerpts included

## Repository evidence checked

- [x] README, documentation, specifications, and implementation report
- [x] All Go modules and service structure
- [x] React/TypeScript console and role-specific routes
- [x] API controllers, service, repository, and shared middleware layers
- [x] Database migrations, functions, triggers, views, roles, seed, and SQL tests
- [x] Authentication, refresh tokens, merchant API keys, and role structures
- [x] Blockchain, balance, gas, KYC, webhook, Redis, and RabbitMQ paths
- [x] Dockerfiles, Docker Compose profiles, Kubernetes, Kong, Vault, Prometheus, and Grafana configuration
- [x] GitHub Actions workflow
- [x] Git history and author-name variants
- [x] Current and historical sensitive-file paths

## Verification performed

- [x] Go test commands passed across all nine modules
- [x] PostgreSQL-backed transaction lifecycle integration test passed
- [x] 14 frontend tests passed
- [x] Frontend production build completed
- [x] Ten database migrations applied to an isolated local database
- [x] Three SQL verification scripts completed
- [x] Eight backend health endpoints returned ready
- [x] Local invoice reached `paid`
- [x] Local transaction reached `confirmed`
- [x] Corresponding webhook delivery reached `delivered` with a successful response
- [x] Screenshot records sanitized to `.test` domains and synthetic user names

## Security and privacy blockers

- [ ] Remove/rotate tracked private key material before any source redistribution
- [ ] Review historical `.env` files and confirm any credentials are revoked
- [ ] Review development secret fallbacks and all default local credentials/tokens
- [ ] Correct or explicitly accept the current credentialed wildcard CORS policy before production reuse
- [ ] Resolve or accept the four high-severity frontend dependency audit findings before deployable reuse
- [ ] Confirm the public repository's missing license and ownership rights
- [x] Keep startup/client identity confidential
- [x] DePay name and prepared screenshots approved for publication by Oferli
- [x] Selected Figma-derived design preview approved as project collateral
- [ ] Confirm no third-party copyrighted assets require separate permission
- [ ] Keep internal endpoint, database, log, wallet, transaction-hash, and provider details out of public assets

## Files allowed in a future portfolio repository

- [x] `README.md`
- [x] `CASE_STUDY.md`
- [x] `SALES_SUMMARY.md`
- [x] `SCREENSHOT_GUIDE.md`
- [x] `PUBLICATION_CHECKLIST.md`
- [x] `EVIDENCE_MATRIX.md`
- [x] `assets/screenshots/public/*.png`

Do not copy the original application source or Git history into the portfolio repository.

## Confirmed by Mikhail

- [x] Role: Backend & DevOps Engineer
- [x] Contribution: backend, database, blockchain integrations, frontend, infrastructure, CI, and observability
- [x] All three Git author-name variants belong to him
- [x] Startup/client identity remains confidential
- [x] DePay name, prepared screenshots, approved Figma collateral, and high-level architecture may be published
- [x] The project remained at pilot stage and tested real transactions
- [x] No separate code or design owner identified
- [x] Create the Oferli repository privately first, following the previous case-study pattern
