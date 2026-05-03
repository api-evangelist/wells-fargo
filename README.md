# Wells Fargo

Wells Fargo is a diversified, community-based financial services company providing banking, investment, mortgage, and consumer and commercial finance through thousands of stores and digital channels. Wells Fargo operates a comprehensive developer portal at developer.wellsfargo.com offering open banking APIs for payments, account data, and treasury management. The Gateway API platform handles over 1.5 billion API calls annually.

**Website:** https://www.wellsfargo.com
**Developer Portal:** https://developer.wellsfargo.com
**Documentation:** https://developer.wellsfargo.com/documentation

## APIs

### Wells Fargo Gateway API

Comprehensive open banking platform launched in 2016 for commercial customers. Supports payments, real-time account information, and financial data integration. OAuth 2.0 authenticated.

- **Base URL:** https://api.wellsfargo.com
- **Documentation:** https://developer.wellsfargo.com/apis
- **OpenAPI:** [wells-fargo-gateway-api-openapi.yml](openapi/wells-fargo-gateway-api-openapi.yml)

**Endpoints:** List Accounts, List Payments, Create a Payment, List Transactions

### Wells Fargo Account Transactions API

Treasury management API for searching and retrieving ACH, Wire, and RTP/Instant Payment transactions with up to 180 days of history and real-time intraday reporting.

- **Base URL:** https://api.wellsfargo.com
- **Documentation:** https://developer.wellsfargo.com/documentation/api-references/account-transactions/v3/transaction-detail-api-ref-v3
- **OpenAPI:** [wells-fargo-account-transactions-api-openapi.yml](openapi/wells-fargo-account-transactions-api-openapi.yml)

**Endpoints:** List Accounts, Get Account Balances, List Account Transactions, Get Transaction Detail

### Wells Fargo ACH Payments API

ACH payment initiation API for CCD, CTX, PPD, and WEB transactions with intelligent routing across RTP, FedNow, and ACH rails. Supports individual and batch payments.

- **Base URL:** https://api.wellsfargo.com
- **Documentation:** https://developer.wellsfargo.com/documentation/api-references/ach-payments/v2/ach-payments-api-ref-v2
- **OpenAPI:** [wells-fargo-ach-payments-api-openapi.yml](openapi/wells-fargo-ach-payments-api-openapi.yml)

**Endpoints:** Initiate ACH Payment, List ACH Payments, Get ACH Payment, Cancel ACH Payment, Submit ACH Batch, List ACH Returns

## Artifacts

### OpenAPI Specifications
- [Gateway API](openapi/wells-fargo-gateway-api-openapi.yml)
- [Account Transactions API](openapi/wells-fargo-account-transactions-api-openapi.yml)
- [ACH Payments API](openapi/wells-fargo-ach-payments-api-openapi.yml)

### JSON Schema
- [Transaction Schema](json-schema/wells-fargo-transaction-schema.json)
- [ACH Payment Schema](json-schema/wells-fargo-ach-payment-schema.json)

### JSON Structure
- [Transaction Structure](json-structure/wells-fargo-transaction-structure.json)
- [ACH Payment Structure](json-structure/wells-fargo-ach-payment-structure.json)

### Examples
- [List Accounts](examples/wells-fargo-gateway-api-listAccounts-example.json)
- [Create Payment](examples/wells-fargo-gateway-api-createPayment-example.json)
- [Initiate ACH Payment](examples/wells-fargo-ach-payments-api-initiateAchPayment-example.json)
- [List Account Transactions](examples/wells-fargo-account-transactions-api-listAccountTransactions-example.json)

### Spectral Rules
- [Wells Fargo Rules](rules/wells-fargo-rules.yml)

### Capabilities (Naftiko)
- [Commercial Banking Treasury](capabilities/commercial-banking-treasury.yaml) — Unified treasury workflow combining Gateway + Transactions + ACH APIs (13 tools)
- **Shared:** [Gateway API](capabilities/shared/gateway-api.yaml)
- **Shared:** [Account Transactions API](capabilities/shared/account-transactions-api.yaml)
- **Shared:** [ACH Payments API](capabilities/shared/ach-payments-api.yaml)

### JSON-LD
- [Wells Fargo Context](json-ld/wells-fargo-context.jsonld)

### Vocabulary
- [Wells Fargo Vocabulary](vocabulary/wells-fargo-vocabulary.yml)

## Tags

Banking, Financial Services, Open Banking, Payments, ACH, Treasury Management, Commercial Banking, Fortune 500

## Maintainers
**FN:** API Evangelist
**Email:** info@apievangelist.com
