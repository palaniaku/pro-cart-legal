# Privacy Policy — Pro Cart

**Last updated:** 18 September 2026

## 1. Who we are

Pro Cart is a Shopify application developed and operated by **Caziel** (CVR: **40544097**), a sole proprietorship registered in Denmark.

For questions about this policy or how we handle data, contact **contactcaziel@gmail.com**.

We are the data controller for the information described below.

## 2. What this policy covers

This policy explains what data Pro Cart processes when a merchant installs the app on a Shopify store, why the data is processed, how it is stored, and how privacy requests are handled.

Pro Cart adds a customizable side cart to Shopify storefronts, with features such as reward tiers, upsells, display/selection of existing Shopify selling plans, discount codes, notes, payment icons, and trust content.

## 3. Information we process

### 3.1 Merchant and Shopify session information

When Pro Cart is installed, Shopify provides the information required to authenticate the store and operate the embedded app. Pro Cart's Shopify session storage can contain:

- The store's `.myshopify.com` domain
- The Shopify access token and granted scopes
- Shopify user/session identifiers
- For online sessions, account information supplied by Shopify such as first name, last name, email address, locale, account-owner status, and related session metadata

This information is used only to authenticate the merchant, maintain the embedded app session, and communicate with Shopify on the merchant's behalf.

### 3.2 App configuration

Pro Cart stores settings by shop, including cart design and behavior settings, reward configuration, selected gift and upsell products, storefront text, and trust/presentation settings.

The app also stores identifiers for Shopify resources that Pro Cart itself manages, such as app-owned automatic discounts.

### 3.3 Product information

Pro Cart requests the `read_products` scope so merchants can select products and the app can display product titles, images, variants, prices, and related product information needed by cart features.

Pro Cart does not store a copy of the merchant's full product catalogue. Product references selected for app features can be stored as part of the merchant's configuration.

The app requests `write_files` so a merchant can upload a trust badge image to the merchant's own Shopify Files.

### 3.4 Storefront analytics

To provide merchant-facing cart analytics, the current Pro Cart storefront records only the store-scoped events needed by the analytics UI:

- Cart views
- Upsell additions

An upsell event contains the relevant product ID and timestamp. A cart-view event records only the event and timestamp. New storefront analytics events don't store product titles or event amounts.

Existing installations can contain historical checkout, legacy add-on, or selling-plan event categories created by older Pro Cart builds. The current storefront endpoint no longer accepts those legacy event types, and those records are removed with the rest of the shop-scoped analytics data on uninstall or applicable redaction.

These records are associated with the Shopify store, not with a shopper profile. Pro Cart does not intentionally attach shopper names, email addresses, phone numbers, postal addresses, IP addresses, browser fingerprints, or payment details to these storefront analytics events.

### 3.5 Paid-order analytics

Pro Cart requests `read_orders` and subscribes to Shopify's `orders/paid` webhook so merchant analytics can reflect completed paid orders rather than only cart activity.

The webhook is configured to request only the fields needed for this purpose. Pro Cart stores:

- Shopify order ID
- The time used for paid-order analytics
- Order total
- A minimized line-item projection containing product ID, title, quantity, price, and whether a line was attributed to a Pro Cart upsell, legacy add-on, or free gift
- The Pro Cart reward-tier cart attribute used for aggregate reward analytics

Pro Cart does **not** persist customer name, customer email, customer phone number, shipping address, billing address, or payment details from the order webhook.

A Shopify order ID can still relate to an identifiable customer. For that reason, Pro Cart treats retained order records as protected customer data and supports Shopify's mandatory privacy webhooks.

## 4. Why we process this data

We process the data above to:

- Authenticate merchants and operate the embedded Shopify app
- Render and configure Pro Cart on the storefront
- Save and restore merchant configuration
- Synchronize app-owned Shopify discounts and other required Shopify resources
- Provide cart, reward, upsell, and paid-order analytics to the merchant
- Respond to support and privacy requests
- Comply with legal obligations

We limit processing to these purposes and do not sell merchant or customer data or use it for third-party advertising.

## 5. Where data is stored

Pro Cart uses third-party infrastructure providers to operate the service, including:

- **Neon** for PostgreSQL database infrastructure
- **Railway** for application hosting

These providers process data on our behalf under their applicable security and data-protection terms. We do not state a specific data-residency region in this policy unless it is confirmed by the active production configuration.

## 6. Who we share data with

We do not sell data and do not share it for advertising.

Data is shared as needed with Shopify and the infrastructure providers used to operate Pro Cart, or where disclosure is required by law.

If a merchant enables optional storefront presentation features, the shopper's browser can also connect directly to the relevant third-party service:

- **Google Fonts** — only when the merchant selects an optional Google-hosted font in Pro Cart typography settings. The browser requests the selected font stylesheet and font resources from Google.
- **Trustpilot** — only when the merchant enables the Trustpilot integration and provides the required Trustpilot configuration. Pro Cart then loads Trustpilot's official TrustBox resources so Trustpilot can render the merchant's review content.

Those optional services process browser/network information under their own terms and privacy notices. Merchants can avoid those connections by leaving the corresponding optional feature disabled.

## 7. Retention and deletion

Merchant configuration, session data, storefront analytics, and paid-order analytics are retained for the period that Pro Cart remains installed so the merchant can use the app and its analytics history. Pro Cart does not currently apply a separate time-based retention period after uninstall.

When a merchant uninstalls Pro Cart, the app processes Shopify's `app/uninstalled` webhook and deletes shop-scoped local app data, including sessions, app configuration, upsell rules, analytics events, and stored order analytics. Shopify-side resource cleanup is attempted where Shopify still provides the access required to do so.

Pro Cart also supports Shopify's mandatory privacy webhooks:

- `customers/data_request` — authenticated requests concerning data associated with a customer
- `customers/redact` — deletes stored order-analytics records for the order IDs Shopify identifies for redaction
- `shop/redact` — deletes shop-scoped sessions, settings, rules, analytics events, and stored order analytics

These handlers are authenticated through Shopify's webhook verification flow.

## 8. Security

Pro Cart uses Shopify's authentication and webhook-verification mechanisms. Application secrets and database credentials are supplied to the application through protected production environment configuration rather than exposed to the storefront.

Shopify access tokens are stored in the app's server-side session storage and are not returned to storefront clients. Communications between the application, Shopify, and infrastructure providers use encrypted HTTPS/TLS connections where supported by those services. Infrastructure providers also apply their own storage and security controls.

## 9. Your rights

Depending on applicable data-protection law, merchants and their customers may have rights including:

- Requesting access to personal data
- Requesting correction of inaccurate data
- Requesting deletion of data
- Objecting to or restricting certain processing
- Requesting data portability
- Lodging a complaint with the relevant supervisory authority

In Denmark, the supervisory authority is Datatilsynet.

To make a privacy request, contact **contactcaziel@gmail.com**. We will respond in accordance with applicable legal requirements.

## 10. Children

Pro Cart is a business application for Shopify merchants and is not directed at children. We do not knowingly collect data from children through the Pro Cart merchant application.

## 11. Changes to this policy

We may update this policy as the service develops or as legal and platform requirements change. The date at the top reflects the most recent revision.

## 12. Contact

**Caziel**  
CVR: 40544097  
Denmark

Email: **contactcaziel@gmail.com**
