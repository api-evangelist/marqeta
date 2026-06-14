# Marqeta GraphQL Schema

## Overview

This conceptual GraphQL schema represents the Marqeta card-issuing and payment processing platform. Marqeta's Core API is a RESTful surface, and this schema captures an equivalent GraphQL model covering cards, cardholders, card products, funding, transactions, authorizations, KYC/KYB, sandbox simulation, webhooks, and program management.

## Source

- Platform: Marqeta Core API v3
- REST Docs: https://www.marqeta.com/docs/core-api
- Developer Guides: https://www.marqeta.com/docs/developer-guides/
- GitHub: https://github.com/marqeta
- Base URL: https://sandbox-api.marqeta.com/v3

## Schema File

[marqeta-schema.graphql](marqeta-schema.graphql)

## Key Domains

### Cards

The card domain covers virtual and physical card lifecycle: creation, state transitions (ACTIVE, SUSPENDED, TERMINATED), PAN retrieval, CVV2, PIN management, BIN details, and personalization (emboss images, text lines).

Types: `Card`, `CardDetails`, `CardState`, `CardToken`, `CardPan`, `CardExpiry`, `CardCVV`, `CardBIN`, `VirtualCard`, `PhysicalCard`, `CardPersonalization`, `EmbossImage`, `TextLine`, `CardholderAuth`, `CardPIN`, `CardControls`.

### Card Products

Card products define the behavior ruleset for a card: funding model, velocity controls, spend controls, expiration offsets, and personalization templates.

Types: `CardProduct`, `CardProductDetails`, `CardConfig`, `ExpirationOffset`, `VelocityControl`, `SpendControl`, `BusinessCard`.

### Users and Businesses

Users (cardholders) and Businesses are the account-holding entities. Both undergo KYC/KYB identity verification.

Types: `User`, `UserDetails`, `UserStatus`, `CardholderDetails`, `Business`, `BusinessDetails`, `Kyc`, `KycResult`.

### Funding

Marqeta uses a General Purpose Account (GPA) model for card funding. Funding sources back GPAs and program funding accounts.

Types: `Funding`, `FundingSource`, `GPA`, `GPABalance`, `ProgramFunding`, `MSP`, `Account`, `AccountBalance`.

### Transactions

Transactions cover the full lifecycle: authorization, clearing, refund, reversal, adjustment credits, fee assessment, and PIN-change events.

Types: `Transaction`, `TransactionDetails`, `TransactionType`, `Authorization`, `Clearing`, `Refund`, `Reversal`, `PinChange`, `AdjustmentCredit`, `TransactionFee`, `MCC`, `Merchant`, `MerchantDetails`, `Terminal`.

### Programs and Configuration

Program metadata, API keys, and tokens represent tenant-level configuration within the Marqeta multi-program environment.

Types: `Program`, `APIKey`, `Token`.

### Webhooks and Events

Webhook subscriptions and event payloads for card, transaction, and account lifecycle notifications.

Types: `Webhook`, `WebhookEvent`.

### Sandbox and Simulation

Sandbox simulation endpoints allow test-environment transaction flows without real card rails.

Types: `Sandbox`, `SimulationRequest`.

## Type Count

65 named types defined in the schema.
