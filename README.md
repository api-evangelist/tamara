# Tamara

Tamara is the Saudi Arabia–headquartered MENA shopping and Buy-Now-Pay-Later platform offering Shariah-compliant split-payment and Pay-Now solutions across Saudi Arabia, the United Arab Emirates, Kuwait, Bahrain, and Oman. Founded in 2020 and licensed by the Saudi Central Bank (SAMA, license No. 95/A Sh/202502), Tamara became the first homegrown Saudi fintech unicorn in December 2023 after raising a US$340M Series C co-led by SNB Capital and Sanabil Investments, and operates on a Shariah-compliant funding base anchored by Goldman Sachs, Citi, and Apollo debt facilities.

This repository profiles Tamara's developer surface — eight APIs (Checkout, Orders, Payments, In-Store Checkout, Webhooks, Disputes, Pre-Checkout Eligibility, and Channel Partners), six SDKs (PHP, .NET, iOS, Android, Flutter examples, React Native example), six e-commerce plugins (Magento, WooCommerce, OpenCart, PrestaShop, Salesforce Commerce Cloud, Shopify), and the ecosystem of regional integration partners (Salla, Amazon Payment Services, Checkout.com, PayTabs, CCAvenue, Qoyod, Osarah Pro, Shahbandr, Techrar).

## APIs

| API | Description |
|---|---|
| [Tamara Checkout API](openapi/tamara-checkout-api-openapi.yml) | Create hosted checkout sessions; return a `checkout_url` for the consumer to complete BNPL or Pay-Now. |
| [Tamara Orders API](openapi/tamara-orders-api-openapi.yml) | Authorise, retrieve, update, and cancel orders through Tamara's online lifecycle. |
| [Tamara Payments API](openapi/tamara-payments-api-openapi.yml) | Capture funds and process simplified or legacy refunds. |
| [Tamara In-Store Checkout API](openapi/tamara-in-store-checkout-api-openapi.yml) | Generate SMS or QR-code payment links for brick-and-mortar BNPL. |
| [Tamara Webhooks API](openapi/tamara-webhooks-api-openapi.yml) | Register and manage HTTPS webhooks for order and dispute events. |
| [Tamara Disputes API](openapi/tamara-disputes-api-openapi.yml) | List, filter, and update merchant disputes. |
| [Tamara Pre-Checkout Eligibility API](openapi/tamara-eligibility-api-openapi.yml) | Decide whether to render Tamara as a payment option before checkout. |
| [Tamara Channel Partners API](openapi/tamara-channel-partners-api-openapi.yml) | PSP/platform surface to onboard merchants onto Tamara and listen for onboarding events. |

## Naftiko Capabilities

Per-API Naftiko capabilities are published in [`capabilities/`](capabilities/) — each capability exposes REST and MCP adapters routed through a self-contained HTTP `consumes` block.

- `capabilities/checkout-sessions.yaml`
- `capabilities/orders.yaml`
- `capabilities/payments.yaml`
- `capabilities/in-store-checkout.yaml`
- `capabilities/webhooks.yaml`
- `capabilities/disputes.yaml`
- `capabilities/eligibility.yaml`
- `capabilities/channel-partners.yaml`

## JSON Schemas

- [`json-schema/tamara-order-schema.json`](json-schema/tamara-order-schema.json)
- [`json-schema/tamara-checkout-session-schema.json`](json-schema/tamara-checkout-session-schema.json)
- [`json-schema/tamara-capture-schema.json`](json-schema/tamara-capture-schema.json)
- [`json-schema/tamara-refund-schema.json`](json-schema/tamara-refund-schema.json)
- [`json-schema/tamara-dispute-schema.json`](json-schema/tamara-dispute-schema.json)

## Examples

End-to-end request/response payloads for the core merchant lifecycle live in [`examples/`](examples/):

- Create Checkout Session
- Authorise Order
- Capture Order
- Simplified Refund
- Pre-Checkout Eligibility
- Register Webhook

## Spectral Rules

[`rules/tamara-rules.yml`](rules/tamara-rules.yml) enforces Tamara's API conventions: bearer auth, Title Case summaries, camelCase `operationId`s, the `https://api.tamara.co` (and `partner-api.tamara.co`) server entry, and the supported GCC currency enum (SAR, AED, BHD, KWD, OMR).

## Commercial Profile

- [`plans/tamara-plans-pricing.yml`](plans/tamara-plans-pricing.yml) — Merchant and Channel Partner plans (free onboarding/API; per-transaction MDR negotiated per merchant).
- [`rate-limits/tamara-rate-limits.yml`](rate-limits/tamara-rate-limits.yml) — Tamara does not publish numeric rate limits; policies cover idempotency, webhook retries, and backoff.
- [`finops/tamara-finops.yml`](finops/tamara-finops.yml) — FOCUS 1.3-aligned mapping of Tamara's weekly settlement cycle, MDR, refund-adjustment, and dispute-chargeback meters.

## Semantics

- [`json-ld/tamara-context.jsonld`](json-ld/tamara-context.jsonld) — JSON-LD vocabulary mapping Tamara order, checkout session, capture, refund, dispute, webhook, and Money to schema.org and XSD types.
- [`json-structure/tamara-order-structure.json`](json-structure/tamara-order-structure.json) — JSON Structure representation of a Tamara Order for code generation.
- [`vocabulary/tamara-vocabulary.yml`](vocabulary/tamara-vocabulary.yml) — Domain vocabulary covering products, lifecycle states, regulators, supported countries/currencies/locales, order/dispute statuses, payment types, and webhook events.

## SDKs and Plugins

Official source on GitHub at [Tamara-Technology](https://github.com/Tamara-Technology):

- **SDKs:** [PHP](https://github.com/Tamara-Technology/php-sdk), [.NET](https://github.com/Tamara-Technology/dotnet-sdk), [iOS](https://github.com/Tamara-Technology/ios-sdk), [Android](https://github.com/Tamara-Technology/android-sdk), Flutter ([example](https://github.com/Tamara-Technology/flutter-sdk-example)), React Native ([example](https://github.com/Tamara-Technology/react-sdk-example))
- **Plugins:** [Magento](https://github.com/Tamara-Technology/magento), [WooCommerce](https://github.com/Tamara-Technology/wp-plugin-tamara-checkout), [OpenCart](https://github.com/Tamara-Technology/opencart), [PrestaShop](https://github.com/Tamara-Technology/prestashop), [Salesforce Commerce Cloud](https://github.com/Tamara-Technology/salesforce), [Shopify](https://tamara.co/en-sa/plugins/shopify)
- **Regional integrations:** Salla, Amazon Payment Services, Checkout.com, PayTabs, CCAvenue, Qoyod, Osarah Pro, Shahbandr, Techrar.

## Useful Links

- **Documentation:** https://docs.tamara.co/
- **API Reference:** https://docs.tamara.co/reference/tamara-api-reference-documentation
- **LLM-Friendly Index:** https://docs.tamara.co/llms.txt
- **Quick Start (Direct API):** https://docs.tamara.co/docs/direct-quick-start-guide
- **Partners Portal:** https://partners.tamara.co/
- **Status:** https://status.tamara.co/
- **GitHub:** https://github.com/Tamara-Technology
