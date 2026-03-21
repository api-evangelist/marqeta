# Marqeta (marqeta)
Marqeta is a modern card issuing platform that enables businesses to create, issue, and manage payment cards with granular spend controls and real-time transaction processing. Their developer platform provides RESTful APIs for building card programs, including prepaid, expense management, earned wage access, and buy now pay later use cases, along with analytics and webhook-based event notifications.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/apis.yml)

## Scope
- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - Card Issuing, Payment Processing, Fintech, Payments, Analytics

## Timestamps

- **Created:** 2026-03-21
- **Modified:** 2026-03-21

## APIs

### Marqeta Core API
The Marqeta Core API is a RESTful interface that enables developers to build and manage card payment programs programmatically. It provides endpoints for creating and managing cardholders, issuing physical and virtual cards, defining spending controls, and retrieving transaction data. The API supports use cases including prepaid cards, expense management, earned wage access, and buy now pay later programs. Authentication uses HTTP Basic Auth, and the API communicates using JSON over HTTPS. Webhooks are available to receive real-time event notifications for card activity and transaction events.

**Human URL:** [https://www.marqeta.com/docs/core-api/introduction](https://www.marqeta.com/docs/core-api/introduction)

#### Tags:

 - Card Issuing, Payment Processing, Fintech, REST, Payments

#### Properties

- [Documentation](https://www.marqeta.com/docs/core-api/introduction)
- [OpenAPI](openapi/marqeta-core-api-openapi.yml)

### Marqeta DiVA API
The Marqeta DiVA (Data insights, Visualization, and Analytics) API is a RESTful interface that provides programmatic access to production data from a Marqeta card program. It surfaces the data behind Marqeta's reporting and analytics tools, enabling developers to retrieve large datasets in JSON or CSV format. The API supports filtering, sorting, aggregation, and pagination for customized responses. Use cases include financial reconciliation, program balance reporting, transaction analysis, and settlement data retrieval.

**Human URL:** [https://www.marqeta.com/docs/diva-api/introduction](https://www.marqeta.com/docs/diva-api/introduction)

#### Tags:

 - Analytics, Reporting, Data, Fintech, REST

#### Properties

- [Documentation](https://www.marqeta.com/docs/diva-api/introduction)
- [OpenAPI](openapi/marqeta-diva-api-openapi.yml)

### Marqeta Webhooks
Marqeta Webhooks deliver real-time event notifications to a developer-configured endpoint when specific events occur within a card program. Each program supports up to five active webhook configurations, and events cover card transactions, authorizations, declines, and other platform activity. Webhook payloads are delivered as HTTP POST requests in JSON format to the receiving endpoint. This allows applications to respond immediately to card activity without polling the Core API for updates.

**Human URL:** [https://www.marqeta.com/docs/developer-guides/webhooks-landing-page](https://www.marqeta.com/docs/developer-guides/webhooks-landing-page)

#### Tags:

 - Webhooks, Events, Real-Time, Notifications, Fintech

#### Properties

- [Documentation](https://www.marqeta.com/docs/developer-guides/webhooks-landing-page)
- [AsyncAPI](asyncapi/marqeta-webhooks-asyncapi.yml)

## Common Properties

- [Portal](https://www.marqeta.com/docs)
- [Documentation](https://www.marqeta.com/docs)
- [Website](https://www.marqeta.com/)
- [Blog](https://www.marqeta.com/blog)
- [Login](https://app.marqeta.com/login)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
