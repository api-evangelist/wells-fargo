# wells-fargo (wells-fargo)

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
