# Privacy Policy — Milani Cart

**Last updated:** October 18, 2026

This policy explains how Milani Cart processes information when a merchant installs and uses the app.

## 1. Who we are

Milani Cart is a Shopify application operated by **Caziel** (CVR: **40544097**), Denmark.

For privacy questions, contact **milaniapps@outlook.com**.

## 2. What information Milani Cart processes

Milani Cart processes only the information needed to operate the app, provide storefront functionality, and show merchant analytics.

- Shopify store and authentication information.
- Cart and app settings configured by the merchant.
- Product and variant information used for cart, gift, and upsell functionality.
- Store-scoped storefront events such as cart views and upsell additions.
- Minimized paid-order analytics for orders attributed to Milani Cart.
- Privacy requests received from Shopify: Shopify's request ID, the customer ID, the requested order IDs, the time received, the status, and when the request was marked as handled.
- The store's Milani Cart plan status (active, inactive or unknown) and when it was last checked.

For attributed paid orders, Milani Cart may store the Shopify order ID, order total, paid timestamp, reward attribution, and limited line-item data such as product ID, title, quantity, price, and upsell attribution.

Milani Cart does **not** intentionally store customer names, email addresses, phone numbers, shipping addresses, billing addresses, or payment details for merchant analytics.

## 3. Technical and security data

For security, rate limiting, and event deduplication, Milani Cart may temporarily process technical request information such as:

- IP address.
- Browser user-agent.
- Browser language.

This information is used to generate short-lived identifiers and is not stored as part of persistent shopper profiles.

## 4. Why we process information

- Operate the cart drawer and embedded Shopify app.
- Save merchant configuration.
- Provide rewards, gifts, discounts, and upsells.
- Provide aggregate cart and order analytics.
- Protect storefront endpoints from abuse.
- Handle support, uninstall, and privacy requests.
- Maintain the security and reliability of the service.

Milani Cart does not sell customer or merchant data and does not use retained analytics for third-party advertising.

## 5. Data retention and deletion

Storefront analytics and minimized paid-order analytics may be retained for up to **366 days** for merchant reporting.

When the app is uninstalled, or when Shopify sends an applicable shop-redaction request, Milani Cart deletes locally stored data associated with that store, including sessions, app settings, upsell rules, analytics events, stored paid-order analytics, stored privacy requests, and the store's Milani Cart plan status.

## 6. Shopify privacy requests

Milani Cart receives Shopify's mandatory privacy webhooks. Every webhook is authenticated before any action is taken.

- `customers/redact`: retained order analytics for the Shopify order IDs in the request, and stored privacy requests for that customer, are deleted automatically.
- `shop/redact`: all locally stored data for the store is deleted automatically.
- `customers/data_request`: the request is authenticated and stored in Milani Cart's database with Shopify's request ID, the customer ID, the requested order IDs, the time it was received, and its status. No other customer data from the request is stored. The request is shown to the merchant in the Milani Cart app together with the data Milani Cart stores about the requested orders, which the merchant can download and provide to the customer, and then mark the request as handled. Stored requests are deleted when the app is uninstalled, and when Shopify sends a `shop/redact` request or a `customers/redact` request for that customer.

Privacy requests can also be sent directly to milaniapps@outlook.com.

## 7. Service providers

Milani Cart relies on the following providers to operate the service:

- **Shopify** — app platform, authentication, APIs, Checkout, Theme App Extensions, App Pricing, and privacy webhooks.
- **Railway** — application hosting.
- **Neon** — PostgreSQL database hosting.

Optional merchant-enabled storefront features may also connect the shopper's browser to third-party services such as Trustpilot or Google-hosted typography.

## 8. Security

Milani Cart uses measures including HTTPS/TLS, Shopify authentication, signed Shopify app-proxy requests, authenticated webhooks, scoped API permissions, rate limiting, request validation, and data minimization.

## 9. Your rights

Depending on applicable law, including the GDPR, individuals may have rights to request access, correction, deletion, restriction of processing, objection, and data portability.

Complaints may also be submitted to the relevant data-protection authority. In Denmark, this is **Datatilsynet**.

To make a privacy request, contact **milaniapps@outlook.com**.

## 10. Changes to this policy

This Privacy Policy may be updated when Milani Cart's functionality, providers, or legal requirements change.

The date at the top shows the latest revision.
