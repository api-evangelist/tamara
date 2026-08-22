# Tamara (tamara)

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Tamara is the Saudi Arabia–headquartered MENA shopping and Buy-Now-Pay-Later platform offering Shariah-compliant split-payment and Pay-Now solutions across Saudi Arabia, the United Arab Emirates, Kuwait, Bahrain, and Oman. Founded in 2020 and licensed by SAMA (Saudi Central Bank), Tamara provides merchants with a hosted-checkout Direct API, in-store SMS and QR payment links, mobile SDKs for iOS, Android, Flutter, and React Native, plug-and-play e-commerce extensions for Shopify, Magento, OpenCart, PrestaShop, Salesforce Commerce Cloud and WooCommerce, webhooks for order and dispute lifecycle events, and a Channel Partners onboarding API for payment service providers and platforms that white-label Tamara. The company became the first homegrown Saudi fintech unicorn in December 2023 after raising a US$340M Series C led by SNB Capital and Sanabil Investments and is backed by debt facilities from Goldman Sachs, Citi, and Apollo for its Shariah-compliant funding base.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tamara/refs/heads/main/apis.yml)

## Tags

- BNPL
- Buy Now Pay Later
- Fintech
- Payments
- Checkout
- Shariah Compliant
- MENA
- Saudi Arabia
- UAE
- Installments
- Pay Later
- Merchant Services
- Orders
- Refunds
- Captures
- Webhooks
- Disputes
- Channel Partners
- E-commerce
- POS

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Tamara Checkout API

Create online checkout sessions that send customer and order information to Tamara and receive a hosted checkout URL where the consumer completes the BNPL or Pay-Now flow. Supports SAR, AED, BHD, KWD, and OMR across Saudi Arabia, the UAE, Bahrain, Kuwait, and Oman.

- **Human URL:** [https://docs.tamara.co/reference/createcheckoutsession](https://docs.tamara.co/reference/createcheckoutsession)
- **Base URL:** `https://api.tamara.co`

#### Tags

- Checkout
- BNPL
- Payments
- Orders

#### Properties

- [Documentation](https://docs.tamara.co/reference/createcheckoutsession)
- [Quick Start](https://docs.tamara.co/docs/direct-quick-start-guide)
- [OpenAPI](openapi/tamara-checkout-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-checkout-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-checkout-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/tamara-rules.yml) — [Spectral](https://docs.stoplight.io/docs/spectral)

### Tamara Orders API

Authorize, capture, cancel, retrieve, and update orders created via Tamara checkout sessions. Mirrors the online checkout lifecycle (new → approved → authorised → captured → refunded) and is the merchant's primary post-checkout integration surface.

- **Human URL:** [https://docs.tamara.co/reference/authoriseorder](https://docs.tamara.co/reference/authoriseorder)
- **Base URL:** `https://api.tamara.co`

#### Tags

- Orders
- Authorise
- Capture
- Cancel
- BNPL

#### Properties

- [Documentation](https://docs.tamara.co/reference/authoriseorder)
- [Documentation](https://docs.tamara.co/docs/online-order-status-flow)
- [OpenAPI](openapi/tamara-orders-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-orders-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-orders-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tamara-order-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Tamara Payments API

Capture funds against an authorised order and process refunds. Includes the legacy /payments/refund endpoint and the modern /payments/simplified-refund/{order_id} surface introduced to simplify partial and full refunds against captures.

- **Human URL:** [https://docs.tamara.co/reference/captureorder](https://docs.tamara.co/reference/captureorder)
- **Base URL:** `https://api.tamara.co`

#### Tags

- Payments
- Captures
- Refunds

#### Properties

- [Documentation](https://docs.tamara.co/reference/captureorder)
- [Documentation](https://docs.tamara.co/reference/simplifiedrefund)
- [OpenAPI](openapi/tamara-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tamara-capture-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tamara-refund-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Tamara In-Store Checkout API

Generate Tamara checkout sessions for brick-and-mortar stores through SMS payment links or QR codes that customers scan with the Tamara consumer app to complete the BNPL purchase in-aisle. Includes the void operation for in-store sessions that need to be cancelled before completion.

- **Human URL:** [https://docs.tamara.co/reference/createinstorecheckoutsession](https://docs.tamara.co/reference/createinstorecheckoutsession)
- **Base URL:** `https://api.tamara.co`

#### Tags

- In-store
- POS
- SMS
- QR Code
- Checkout
- BNPL

#### Properties

- [Documentation](https://docs.tamara.co/reference/createinstorecheckoutsession)
- [Documentation](https://docs.tamara.co/reference/createinstoreqrcode)
- [Documentation](https://docs.tamara.co/docs/pos-integration)
- [OpenAPI](openapi/tamara-in-store-checkout-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-in-store-checkout-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-in-store-checkout-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tamara Webhooks API

Register and manage HTTPS webhook endpoints that receive order and dispute lifecycle events from Tamara (order_approved, order_authorised, order_captured, order_refunded, order_canceled, order_expired, dispute events, and more). Webhooks carry a JWT-encoded `tamaraToken` for verification.

- **Human URL:** [https://docs.tamara.co/reference/getting-started-with-webhooks](https://docs.tamara.co/reference/getting-started-with-webhooks)
- **Base URL:** `https://api.tamara.co`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.tamara.co/reference/getting-started-with-webhooks)
- [Documentation](https://docs.tamara.co/docs/transaction-authorisation)
- [OpenAPI](openapi/tamara-webhooks-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-webhooks-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-webhooks-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tamara Disputes API

Query, filter, and update merchant disputes raised against Tamara orders. Supports listing disputes by order id, dispute id, order status, or dispute status; and appending comments and proof attachments to an existing dispute case.

- **Human URL:** [https://docs.tamara.co/reference/get_external-merchants-orders-disputes](https://docs.tamara.co/reference/get_external-merchants-orders-disputes)
- **Base URL:** `https://api.tamara.co`

#### Tags

- Disputes
- Chargebacks
- Merchant Operations

#### Properties

- [Documentation](https://docs.tamara.co/reference/get_external-merchants-orders-disputes)
- [Documentation](https://docs.tamara.co/docs/dispute-management-best-practices)
- [OpenAPI](openapi/tamara-disputes-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-disputes-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-disputes-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tamara Pre-Checkout Eligibility API

Check whether Tamara considers a customer eligible for a BNPL purchase before exposing Tamara as a payment method on the merchant's checkout page. The endpoint accepts an order amount/currency and a customer phone number and returns a boolean eligibility indicator.

- **Human URL:** [https://docs.tamara.co/reference/pre-checkout-eligibility](https://docs.tamara.co/reference/pre-checkout-eligibility)
- **Base URL:** `https://api.tamara.co`

#### Tags

- Eligibility
- Pre-Checkout
- Risk

#### Properties

- [Documentation](https://docs.tamara.co/reference/pre-checkout-eligibility)
- [OpenAPI](openapi/tamara-eligibility-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-eligibility-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-eligibility-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Tamara Channel Partners API

Allow payment service providers, platforms, and aggregators to onboard merchants onto Tamara on their behalf. Submit merchant KYB/KYC information, retrieve onboarding status and merchant API keys, and register onboarding event webhooks. Hosted on a dedicated partner subdomain (partner-api.tamara.co).

- **Human URL:** [https://docs.tamara.co/reference/post_channel-partners-merchant-onboarding-create](https://docs.tamara.co/reference/post_channel-partners-merchant-onboarding-create)
- **Base URL:** `https://partner-api.tamara.co`

#### Tags

- Channel Partners
- Onboarding
- KYB
- KYC
- PSP

#### Properties

- [Documentation](https://docs.tamara.co/reference/post_channel-partners-merchant-onboarding-create)
- [OpenAPI](openapi/tamara-channel-partners-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tamara-channel-partners-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tamara-channel-partners-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Documentation](https://docs.tamara.co/)
- [API Reference](https://docs.tamara.co/reference/tamara-api-reference-documentation)
- [Getting Started](https://docs.tamara.co/docs/direct-quick-start-guide)
- [Status](https://status.tamara.co/)
- [Support](https://docs.tamara.co/)
- [Sign Up](https://partners.tamara.co/)
- [Terms of Service](https://tamara.co/en-SA/legal/terms-conditions)
- [Privacy Policy](https://tamara.co/en-SA/legal/privacy-policy)
- [Pricing](https://tamara.co/en-SA/business)
- [Blog](https://tamara.co/en-SA/blog)
- [Contact Form](https://tamara.co/en-SA/contact-us)
- [Github](https://github.com/Tamara-Technology)
- [LinkedIn](https://www.linkedin.com/company/tamara-co)
- [Twitter](https://twitter.com/TamaraTech)
- [Instagram](https://www.instagram.com/tamara/)
- [Plans](plans/tamara-plans-pricing.yml)
- [Rate Limits](rate-limits/tamara-rate-limits.yml)
- [Fin Ops](finops/tamara-finops.yml)
- [JSON-LD](json-ld/tamara-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/tamara-vocabulary.yml)
- [SDK](https://github.com/Tamara-Technology/php-sdk)
- [SDK](https://github.com/Tamara-Technology/dotnet-sdk)
- [SDK](https://github.com/Tamara-Technology/ios-sdk)
- [SDK](https://github.com/Tamara-Technology/android-sdk)
- [SDK](https://github.com/Tamara-Technology/flutter-sdk-example)
- [SDK](https://github.com/Tamara-Technology/react-sdk-example)
- [Plugin](https://github.com/Tamara-Technology/magento)
- [Plugin](https://github.com/Tamara-Technology/wp-plugin-tamara-checkout)
- [Plugin](https://github.com/Tamara-Technology/opencart)
- [Plugin](https://github.com/Tamara-Technology/prestashop)
- [Plugin](https://github.com/Tamara-Technology/salesforce)
- [Plugin](https://tamara.co/en-sa/plugins/shopify)
- [Integration](https://docs.tamara.co/docs/salla)
- [Integration](https://docs.tamara.co/docs/amazon-payment-services)
- [Integration](https://docs.tamara.co/docs/checkoutcom)
- [Integration](https://docs.tamara.co/docs/paytabs)
- [Integration](https://docs.tamara.co/docs/cc-avenue)
- [Integration](https://docs.tamara.co/docs/qoyod)
- [Integration](https://docs.tamara.co/docs/osarah-pro)
- [Integration](https://docs.tamara.co/docs/shahbandr)
- [Integration](https://docs.tamara.co/docs/techrar)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
