# Source: https://hub.ozow.com/docs/one-api/u9dgo2smpkkz3-overview

Overview

# Overview

Introducing Ozow's **OneAPI (Beta)**, a single modern API for handling all payment-related services, including but not limited to:

- Payment processing (Instant EFT, Cards, Capitec Pay, Bank Deposits, Vouchers, etc.)
- Bank account verification (Check Digit Verification, Bank Account Verification)
- Refunds
- Settlements
- Webhooks for asynchronous notifications

It is a [REST](https://en.wikipedia.org/wiki/REST) based API with predictable resource-oriented URLs, accepts JSON and returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.

## [Why OneAPI?](https://hub.ozow.com/#why-oneapi)

1. **Unified API**: OneAPI combines all Ozow integrations into a single endpoint.
2. **Modern standards**:
 - **OAuth 2.0**: for secure, standards-based authentication.
 - **Idempotency**: preventing duplicate requests for transactions, refunds, etc.
 - **RESTful design**: simpler integration, predictable endpoint structures.
 - **Future-proof**: As Ozow adds payment methods or new features, your integration automatically gains access to them with minimal changes on your side.
 - **Direct payments**: advanced flows that allow merchants to handle user input (e.g., card details) without always needing to redirect to Ozow.

> Important
> 
> The old Ozow APIs will eventually be deprecated. All new features will be introduced in the OneAPI only. For longevity and the broadest feature set, migrating or integrating to OneAPI is strongly recommended.

## [Key Benefits Over Old APIs](https://hub.ozow.com/#key-benefits-over-old-apis)

**Standardized Security & Auth**

Uses OAuth2 Client Credentials flow with well-defined scopes (e.g., payment, refund, settlements). This removes the need for older, ad-hoc credential solutions.

**Idempotency**

Prevents accidental double charges or double refunds. Simply include an Idempotency-Key header to ensure that your requests (e.g., refunds or payments) are processed once only.

**Broader Payment Methods**

Integrate with multiple payment types (Bank Deposits, Capitec Pay, Nedbank Direct EFT, Card, Voucher, etc.) via a single unified approach.

**Direct Payment Flows**

Optionally process payments without redirecting the user away from your site or app for certain payment methods (e.g., card, ABSA Pay, Nedbank Direct EFT).

**Better Developer Experience**

- Uniform naming and data structures across endpoints.
- Clear, descriptive error responses.
- Thorough documentation and built-in support for webhooks in a standard format.

**Automatic Access to New Features**

- As Ozow introduces new payment methods or features, you gain immediate or near-immediate access. No re-integration is required—just pass the correct parameters.

## [Pre-requisities](https://hub.ozow.com/#pre-requisities)

Before beginning to use the One API a merchant has to be a registered Ozow merchant with a valid login for the [Ozow Dashboard](https://dash.ozow.com/MerchantAdmin/Dashboard) (Production) or [Ozow Staging Dashboard](https://stagingdash.ozow.com/MerchantAdmin/Dashboard) (Test). If any assistance is required with this please contact the Ozow support team via [support@ozow.com](mailto:support@ozow.com).

## [Environments](https://hub.ozow.com/#environments)

While using the API, the following environments are available and should be noted:

| Environment | URL |
| --- | --- |
| One API - Production | [https://one.ozow.com](https://one.ozow.com) |
| One API - Staging | [https://stagingone.ozow.com](https://stagingone.ozow.com) |
| Ozow Dashboard - Production | [https://dash.ozow.com](https://dash.ozow.com) |
| Ozow Dashboard - Staging | [https://stagingdash.ozow.com](https://stagingdash.ozow.com) |

[Overview](https://hub.ozow.com/#overview 'Overview') [Why OneAPI?](https://hub.ozow.com/#why-oneapi 'Why OneAPI?') [Key Benefits Over Old APIs](https://hub.ozow.com/#key-benefits-over-old-apis 'Key Benefits Over Old APIs') [Pre-requisities](https://hub.ozow.com/#pre-requisities 'Pre-requisities') [Environments](https://hub.ozow.com/#environments 'Environments')