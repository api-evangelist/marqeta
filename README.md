# Marqeta (marqeta)

Marqeta is a modern card-issuing and embedded-finance platform. The Core API is a large RESTful surface covering cards, users, businesses, GPA orders, KYC/KYB, fee transfer, transactions, real-time decisioning, MCC groups, programs, and webhooks. The Diva (Digital Wallets, Tokenization, 3DS) API extends the Core API.

OpenAPI specs for the Marqeta Core API and Diva API are tracked in [`openapi/`](openapi/). Latest Core API YAML pulled from https://github.com/marqeta/marqeta-openapi.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=marqeta-api-evangelist&utm_content=repo)

## Type
- **x-type:** company

## APIs
- **Marqeta Core API** - REST API for card issuing, user/business management, GPA funding, transactions, authorizations, real-time decisioning, KYC/KYB, MCC controls, programs, and webhooks.
- **Marqeta Diva API** - REST API supplement for Digital Wallets (Apple Pay, Google Pay, Samsung Pay) tokenization, push provisioning, and 3-D Secure flows.
- **Marqeta Webhooks** - Outbound HTTP webhook delivery for card events, authorization requests, advice messages, transactions, and account events.
- **Marqeta Risk Controller / Real-Time Decisioning** - Synchronous webhook-style HTTP endpoint customers expose for Marqeta to call during card authorization for approve/decline decisions.

## Tags
 - FinTech, BaaS, Card Issuing, Payments, Embedded Finance

## Timestamps
- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## Common Properties
- [Website](https://www.marqeta.com/)
- [Plans](plans/marqeta-plans-pricing.yml)
- [RateLimits](rate-limits/marqeta-rate-limits.yml)
- [FinOps](finops/marqeta-finops.yml)

## Maintainers
**FN:** Kin Lane

**Email:** kin@apievangelist.com
