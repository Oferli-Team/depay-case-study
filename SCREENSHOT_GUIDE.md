# DePay Screenshot Guide

## Prepared public gallery

All prepared images are 2560×1440 PNG files in a compact dark browser frame. The underlying application was deployed locally from a clean repository clone, backed by an isolated PostgreSQL instance, and populated only with repository seed data that was further sanitized to reserved `.test` domains and clearly synthetic user names.

| Priority | File | Recommended use |
|---:|---|---|
| 1 | `assets/screenshots/public/depay-merchant-dashboard.png` | README hero and portfolio preview; shows the paid invoice and successful webhook summary. |
| 2 | `assets/screenshots/public/depay-payment-confirmed.png` | Core workflow proof; shows invoice, transaction, and confirmed status together. |
| 3 | `assets/screenshots/public/depay-webhook-delivery.png` | Integration proof; shows a delivered terminal event, one attempt, and successful response. |
| 4 | `assets/screenshots/public/depay-merchant-analytics.png` | Merchant reporting; shows paid revenue and post-payment invoice/transaction charts. |
| 5 | `assets/screenshots/public/depay-compliance-risk.png` | Compliance workflow; shows risk types, levels, and linked synthetic transactions. |
| 6 | `assets/screenshots/public/depay-admin-analytics.png` | Platform operations; shows turnover, transaction status, failure, and RPC-latency charts. |
| 7 | `assets/screenshots/public/depay-user-transactions.png` | Customer view; shows sanitized history and the confirmed local transaction. |
| 8 | `assets/screenshots/public/depay-sql-function.png` | Technical depth; shows an allowlisted analytics function and sanitized results. |
| 9 | `assets/screenshots/public/depay-role-selection.png` | Optional overview; shows the product's four operational personas. |
| 10 | `assets/screenshots/public/depay-figma-wallet-rate.png` | Approved Figma collateral; use only with a caption clarifying that it is a companion-interface design, not a mobile implementation found in the public source. |

## Recommended README sequence

1. Merchant dashboard as the hero image
2. Confirmed payment flow
3. Merchant analytics
4. Webhook delivery
5. Compliance risk review
6. Admin analytics
7. User transaction history

Use the SQL function screenshot in the longer case study rather than the first screenful of the README.

## Do not use

- Raw system-health captures: they expose internal container endpoint names.
- Raw database/browser captures: connection information and records are too easy to disclose accidentally.
- Terminal output: it can contain local paths, internal ports, or configuration values.
- Original seed screenshots captured before sanitization.
- Mobile full-page capture: the repository's current narrow-screen layout produced excessive whitespace and is not a strong portfolio visual.
- Any future screenshot containing real wallet addresses, transaction hashes, emails, webhook URLs, or provider responses.

## Publication notes

- Keep the prepared screenshots unchanged unless a new sanitization review is performed.
- The operational screenshots include two display-only CSS corrections made in the disposable local clone: radio control sizing and brand-mark alignment. No product content or workflow was altered, and the fixes were not written to the user's source checkout.
- Add alt text that describes the workflow rather than claiming business impact.
- Do not label the product as a production processor or attach performance/scale claims without developer confirmation.
- No video assets were prepared, per the request to create screenshots only.
- The Figma-derived asset comes from the developer-approved public project file and must remain labeled as design collateral.
