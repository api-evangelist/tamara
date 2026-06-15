# Tamara (tamara)

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
