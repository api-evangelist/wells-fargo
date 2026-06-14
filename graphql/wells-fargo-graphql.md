# Wells Fargo GraphQL Schema

A conceptual GraphQL schema for the Wells Fargo banking platform, derived from the public Wells Fargo Gateway API at [developer.wellsfargo.com](https://developer.wellsfargo.com). The schema translates the REST-based Open Banking, Payments, and Treasury Management surfaces into a unified GraphQL type system.

## Background

Wells Fargo operates one of the largest commercial banking API platforms in the United States. The Gateway API, launched in 2016, handles over 1.5 billion API calls annually and supports ACH, Wire, RTP, FedNow, real-time account data, and foreign exchange. This GraphQL schema models those capabilities as a single, traversable graph.

## Schema File

[wells-fargo-schema.graphql](wells-fargo-schema.graphql)

## Type Coverage

### Core Accounts (6 types)
| Type | Description |
|------|-------------|
| `Account` | Generic bank account base type |
| `CheckingAccount` | Demand deposit with overdraft and debit card linkage |
| `SavingsAccount` | Interest-bearing account with transfer limits |
| `CreditAccount` | Credit card or revolving line of credit |
| `LoanAccount` | Generic loan covering all secured/unsecured products |
| `AccountBalance` | Point-in-time ledger and available balance |

### Transaction & History (5 types)
| Type | Description |
|------|-------------|
| `AccountHistory` | Daily opening/closing balance record |
| `Transaction` | Posted or pending account transaction |
| `TransactionDetail` | Extended party and routing detail for a transaction |
| `TransactionConnection` | Paginated transaction result set |
| `TransactionEdge` | Cursor-keyed transaction wrapper |

### Payments & Transfers (8 types)
| Type | Description |
|------|-------------|
| `Transfer` | Internal fund transfer between accounts |
| `ACH` | Automated Clearing House credit or debit |
| `Wire` | Domestic or international wire transfer |
| `Check` | Physical check with image retrieval |
| `Payment` | Electronic bill payment |
| `BillPayment` | Bill payment linked to statement data |
| `Payee` | Registered bill pay recipient |
| `DirectDeposit` | Payroll direct deposit enrollment |

### Payment Controls (1 type)
| Type | Description |
|------|-------------|
| `StopPayment` | Stop payment request on a check |

### Cards (3 types)
| Type | Description |
|------|-------------|
| `Card` | Debit or credit card |
| `CardTransaction` | Transaction charged to a card |
| `CardLimit` | Spending and withdrawal limits |

### Lending Products (6 types)
| Type | Description |
|------|-------------|
| `Mortgage` | Residential first or second mortgage |
| `HomeEquity` | Home equity loan or HELOC |
| `AutoLoan` | Vehicle financing |
| `PersonalLoan` | Unsecured personal installment loan |
| `StudentLoan` | Federal or private student loan |
| `BusinessLoan` | Commercial loan or line of credit |

### Foreign Exchange (2 types)
| Type | Description |
|------|-------------|
| `FXRate` | Spot or forward exchange rate quote |
| `FXTransaction` | Completed currency conversion |

### Trade Finance (3 types)
| Type | Description |
|------|-------------|
| `TradeFinance` | Generic trade finance container |
| `LetterOfCredit` | Documentary credit (LC) |
| `BankGuarantee` | Standby LC or performance bond |

### Specialty Accounts (2 types)
| Type | Description |
|------|-------------|
| `SafeDeposit` | Safe deposit box registration |
| `TrustAccount` | Fiduciary or trust account |

### Investments (9 types)
| Type | Description |
|------|-------------|
| `Brokerage` | Self-directed brokerage account |
| `Investment` | Generic investment holding |
| `Securities` | Equity or fixed-income position |
| `Bond` | Bond holding with yield data |
| `MutualFund` | Mutual fund position |
| `CD` | Certificate of deposit |
| `Annuity` | Annuity contract |
| `Retirement` | 401(k) or employer retirement plan |
| `IRA` | Individual Retirement Account |

### Customer & Identity (6 types)
| Type | Description |
|------|-------------|
| `Customer` | Retail banking customer |
| `BusinessCustomer` | Commercial banking entity |
| `Contact` | Associated person or authorized user |
| `Address` | Physical or mailing address |
| `Organization` | Legal entity for business customers |
| `PageInfo` | GraphQL cursor pagination metadata |

### Branch & ATM (2 types)
| Type | Description |
|------|-------------|
| `Branch` | Physical bank branch with hours and services |
| `ATM` | ATM location with surcharge and deposit capabilities |

### Documents (2 types)
| Type | Description |
|------|-------------|
| `BankStatement` | Monthly or quarterly account statement |
| `TaxDocument` | IRS tax form (1099-INT, 1099-DIV, 1099-R, etc.) |

### Compliance & Regulatory (2 types)
| Type | Description |
|------|-------------|
| `Regulatory` | Regulatory filing or report |
| `ComplianceRecord` | KYC/AML/BSA compliance record |

### API Security & Access (4 types)
| Type | Description |
|------|-------------|
| `APIKey` | Machine-to-machine API key credential |
| `OAuthToken` | OAuth 2.0 authorization token |
| `AccessToken` | Bearer token returned by OAuth flow |
| `Webhook` | Event notification subscription |

### Open Banking / PSD2 (5 types)
| Type | Description |
|------|-------------|
| `TrueLayer` | TrueLayer open banking connectivity |
| `OpenBanking` | Open banking account access resource |
| `PSD2` | PSD2 payment initiation or account access entry |
| `Consent` | Customer consent for third-party data access |
| `Statement` | Statement resource for open banking APIs |

## Operations

### Query
The `Query` type exposes 50+ root fields covering accounts, balances, transactions, payments, cards, loans, FX, investments, customers, branches, ATMs, documents, compliance records, and API credentials.

### Mutation
The `Mutation` type supports initiating transfers, ACH payments, wires, stop payments, FX trades, card management, consent lifecycle, webhook management, and API key provisioning.

### Subscription
The `Subscription` type provides real-time event streams for posted transactions, payment and transfer status changes, ACH/wire status updates, FX rate ticks, consent changes, and card transactions.

## Authentication

Wells Fargo's Gateway API uses OAuth 2.0 with client credentials flow for machine-to-machine integrations and authorization code flow for customer-facing applications. The GraphQL schema models both `OAuthToken` and `AccessToken` types to reflect this dual-flow architecture.

## Source APIs

- [Wells Fargo Gateway API](https://developer.wellsfargo.com/apis)
- [Account Transactions API v3](https://developer.wellsfargo.com/documentation/api-references/account-transactions/v3/transaction-detail-api-ref-v3)
- [ACH Payments API v2](https://developer.wellsfargo.com/documentation/api-references/ach-payments/v2/ach-payments-api-ref-v2)
- [Wells Fargo Developer Portal](https://developer.wellsfargo.com)
- [Wells Fargo GitHub](https://github.com/wellsfargo)
