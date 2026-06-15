# wells-fargo (wells-fargo)

Wells Fargo is a diversified, community-based financial services company providing banking, investment, mortgage, and consumer and commercial finance through thousands of stores and digital channels. Wells Fargo operates a comprehensive developer portal at developer.wellsfargo.com offering open banking APIs for payments, account data, and treasury management. The Gateway API platform handles over 1.5 billion API calls annually and supports commercial banking customers with ACH, wire, RTP, FedNow, and data reporting capabilities.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/apis.yml)

## Timestamps

- **Modified:** 2026-05-19

## APIs

### Wells Fargo Gateway API

The Wells Fargo Gateway API is a comprehensive open banking platform launched in 2016, offering a growing catalog of plug-and-play APIs, SDKs, and webhooks for commercial customers and partners. The platform supports payments, real-time account information, and financial data integration across commercial banking, mortgage, credit card, and brokerage services. Built on RESTful principles with OAuth 2.0 authentication, the Gateway handles over 1.5 billion API calls annually.

- **Human URL:** [https://developer.wellsfargo.com/](https://developer.wellsfargo.com/)
- **Base URL:** `https://api.wellsfargo.com`

#### Tags

- Banking
- Financial Services
- Open Banking
- Payments
- Treasury Management
- Commercial Banking

#### Properties

- [Documentation](https://developer.wellsfargo.com/apis)
- [OpenAPI](openapi/wells-fargo-gateway-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wells-fargo-gateway-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wells-fargo-gateway-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/wells-fargo-gateway-api-listAccounts-example.json)
- [Example](examples/wells-fargo-gateway-api-createPayment-example.json)
- [Spectral Ruleset](rules/wells-fargo-rules.yml)

### Wells Fargo Account Transactions API

The Wells Fargo Account Transactions API enables treasury management customers to search and retrieve transaction data from the current day through 180 days prior. The API supports ACH, Wire, and RTP/Instant Payment transactions with unique transaction IDs, intraday and previous day reporting, and pagination for high-volume transaction retrieval.

- **Human URL:** [https://developer.wellsfargo.com/documentation/api-references/account-transactions/v3/transaction-detail-api-ref-v3](https://developer.wellsfargo.com/documentation/api-references/account-transactions/v3/transaction-detail-api-ref-v3)
- **Base URL:** `https://api.wellsfargo.com`

#### Tags

- Banking
- Financial Services
- Account Management
- Transactions
- Treasury Management

#### Properties

- [Documentation](https://developer.wellsfargo.com/documentation/api-references/account-transactions/v3/transaction-detail-api-ref-v3)
- [OpenAPI](openapi/wells-fargo-account-transactions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wells-fargo-account-transactions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wells-fargo-account-transactions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/wells-fargo-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/wells-fargo-transaction-structure.json)
- [Example](examples/wells-fargo-account-transactions-api-listAccountTransactions-example.json)
- [Spectral Ruleset](rules/wells-fargo-rules.yml)

### Wells Fargo ACH Payments API

The Wells Fargo ACH Payments API enables commercial banking customers to initiate ACH credit and debit transactions, including same-day ACH, for payroll, vendor payments, and collections. The API integrates with Wells Fargo's intelligent payment routing that automatically selects the optimal rail including RTP, FedNow, and ACH for each transaction.

- **Human URL:** [https://developer.wellsfargo.com/documentation/api-references/ach-payments/v2/ach-payments-api-ref-v2](https://developer.wellsfargo.com/documentation/api-references/ach-payments/v2/ach-payments-api-ref-v2)
- **Base URL:** `https://api.wellsfargo.com`

#### Tags

- Banking
- Financial Services
- Payments
- ACH
- Treasury Management

#### Properties

- [Documentation](https://developer.wellsfargo.com/documentation/api-references/ach-payments/v2/ach-payments-api-ref-v2)
- [OpenAPI](openapi/wells-fargo-ach-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wells-fargo-ach-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wells-fargo-ach-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/wells-fargo-ach-payment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/wells-fargo-ach-payment-structure.json)
- [Example](examples/wells-fargo-ach-payments-api-initiateAchPayment-example.json)
- [Spectral Ruleset](rules/wells-fargo-rules.yml)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/wellsfargo)
- [Website](https://www.wellsfargo.com)
- [Developer Portal](https://developer.wellsfargo.com)
- [Documentation](https://developer.wellsfargo.com/documentation)
- [Git Hub Org](https://github.com/wells-fargo)
- [J S O N L D Context](json-ld/wells-fargo-context.jsonld)
- [Vocabulary](vocabulary/wells-fargo-vocabulary.yml)
- [L L Ms Txt](https://developer.wellsfargo.com/llms.txt)
