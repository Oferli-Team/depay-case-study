# DePay Claim Evidence Matrix

This internal file maps public-facing statements to repository evidence. It should be reviewed before publication and may be omitted from the final public repository.

| Claim | Evidence | Status |
|---|---|---|
| Public pilot component of a startup | Developer clarification in the working conversation | Confirmed; startup identity remains confidential |
| Eight backend services plus shared Go module | Root directories and nine `go.mod` files | Confirmed |
| React role-based operations console | `apps/web/src/App.tsx`, `auth/personas.ts`, page components | Confirmed |
| PostgreSQL is the source of truth | `docs/architecture.md`, repositories, migrations | Confirmed |
| Transaction lifecycle and idempotency | Transaction service implementation and lifecycle tests | Confirmed |
| Confirmation updates invoice and webhook state | PostgreSQL repository path, integration test, isolated local verification | Confirmed |
| Webhook signatures, retries, delivery logs, dead-letter state | Webhook dispatcher/repositories and migrations 008–009 | Confirmed |
| Auth with refresh rotation and revocation | User service implementation and tests | Confirmed |
| Merchant API keys are scoped, hashed, revocable, and shown once | Migration 010, merchant implementation and tests | Confirmed |
| Compliance/risk/audit data model | Migrations, triggers, admin/compliance pages | Confirmed |
| Redis and RabbitMQ integrations | Wallet/gas and transaction-core services; Compose configuration | Confirmed, optional paths |
| External blockchain, balance, gas, and KYC adapters | Service provider implementations and environment switches | Confirmed as configurable adapters |
| Docker/Compose/Kubernetes/Kong/Vault configuration | Root and infrastructure files | Confirmed; production deployment not verified |
| Prometheus/Grafana observability | Shared middleware/observability, Compose, dashboard config | Confirmed |
| Multi-layer CI | `.github/workflows/ci-cd.yml` | Confirmed; no production deploy job found |
| Local end-to-end successful payment | Isolated run: invoice paid, transaction confirmed, webhook delivered successfully | Confirmed for synthetic local run only |
| Specialized-terminal payment problem | Developer clarification | Confirmed |
| Real transactions tested during pilot | Developer clarification | Confirmed for pilot testing; no production or scale claim |
| Business adoption, scale, or commercial results | Not present in repository and not supplied publicly | Do not claim |
| Exact personal contribution | Developer clarification plus 75 commits under three confirmed author-name variants | Confirmed: Backend & DevOps, database, blockchain, frontend, CI, observability |
| Startup/client name may be disclosed | Developer requested confidentiality | Do not disclose |
| Figma companion-interface design | Developer-supplied Figma file and public Figma preview | Approved design collateral; not evidence of mobile code |
