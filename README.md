# Marqeta (marqeta)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Marqeta is a modern card-issuing and embedded-finance platform. The Core API is a large RESTful surface covering cards, users, businesses, GPA orders, KYC/KYB, fee transfer, transactions, real-time decisioning, MCC groups, programs, and webhooks. The Diva (Digital Wallets, Tokenization, 3DS) API extends the Core API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/apis.yml)

## Tags

- FinTech
- BaaS
- Card Issuing
- Payments
- Embedded Finance

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-08

## APIs

### Marqeta Core API

REST API for card issuing, user/business management, GPA funding, transactions, authorizations, real-time decisioning, KYC/KYB, MCC controls, programs, and webhooks. Customers operate within an isolated 'program' environment.

- **Human URL:** [https://www.marqeta.com/docs/core-api](https://www.marqeta.com/docs/core-api)
- **Base URL:** `https://sandbox-api.marqeta.com/v3`

#### Tags

- REST
- Card Issuing
- Payments

#### Properties

- [Documentation](https://www.marqeta.com/docs/core-api)
- [OpenAPI](openapi/marqeta-core-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/marqeta-core-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/marqeta-core-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Marqeta Diva API

REST API supplement for Digital Wallets (Apple Pay, Google Pay, Samsung Pay) tokenization, push provisioning, and 3-D Secure flows.

- **Human URL:** [https://www.marqeta.com/docs/diva-api](https://www.marqeta.com/docs/diva-api)
- **Base URL:** `https://sandbox-api.marqeta.com/v3`

#### Tags

- REST
- Digital Wallet
- Tokenization
- 3DS

#### Properties

- [Documentation](https://www.marqeta.com/docs/diva-api)
- [OpenAPI](openapi/marqeta-diva-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/marqeta-diva-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/marqeta-diva-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Marqeta Webhooks

Outbound HTTP webhook delivery for card events, authorization requests, advice messages, transactions, and account events.

- **Human URL:** [https://www.marqeta.com/docs/core-api/event-types](https://www.marqeta.com/docs/core-api/event-types)
- **Base URL:** `https://sandbox-api.marqeta.com/v3/webhooks`

#### Tags

- Webhooks

#### Properties

- [Documentation](https://www.marqeta.com/docs/core-api/event-types)
- [Postman Collection](collections/marqeta-core-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/marqeta-core-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/marqeta-diva-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/marqeta-diva-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Marqeta Risk Controller / Real-Time Decisioning

Synchronous webhook-style HTTP endpoint customers expose for Marqeta to call during card authorization for approve/decline decisions.

- **Human URL:** [https://www.marqeta.com/docs/core-api/real-time-decisioning](https://www.marqeta.com/docs/core-api/real-time-decisioning)
- **Base URL:** `customer-hosted`

#### Tags

- Webhooks
- RTD

#### Properties

- [Documentation](https://www.marqeta.com/docs/core-api/real-time-decisioning)
- [Postman Collection](collections/marqeta-core-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/marqeta-core-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/marqeta-diva-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/marqeta-diva-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/marqeta)
- [LinkedIn](https://www.linkedin.com/company/marqeta)
- [Website](https://www.marqeta.com/)
- [Plans](plans/marqeta-plans-pricing.yml)
- [Rate Limits](rate-limits/marqeta-rate-limits.yml)
- [Fin Ops](finops/marqeta-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
