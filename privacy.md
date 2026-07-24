# Privacy Policy — Pro Cart

**Last updated:** 22 July 2026

## 1. Who we are

Pro Cart is a Shopify application developed and operated by **Milani** (CVR: **40544097**), a sole proprietorship registered in Denmark.

For any questions about this policy or about how we handle data, contact us at **contactcaziel@gmail.com**.

We are the data controller for the information described below.

## 2. What this policy covers

This policy explains what data Pro Cart collects when a merchant installs the app on their Shopify store, why we collect it, how we store it, and what rights merchants and their customers have.

Pro Cart adds a customizable side cart to Shopify storefronts, with features such as rewards, upsells, add-ons, discount codes, and trust badges.

## 3. Information we collect

### 3.1 From the merchant's store

When you install Pro Cart, we receive and store:

- **Store identity**: your `.myshopify.com` domain and Shopify store ID
- **Access credentials**: an access token that lets the app communicate with your store, plus the scopes you have granted
- **Account details** supplied by Shopify during installation, which may include the store owner's name, email address, and locale
- **App configuration**: every setting you choose inside Pro Cart, including colours, text, reward thresholds, selected upsell and add-on products, and typography

### 3.2 Product information

Pro Cart requests the `read_products` scope so it can display product titles, images, variants, and prices inside the cart. We read this data when the cart is rendered. We do not store a copy of your full product catalogue.

The app also requests `write_files` so merchants can upload a trust badge image, which is stored in the merchant's own Shopify Files.

### 3.3 Usage and analytics data

To show merchants how the cart performs, Pro Cart records events such as:

- Cart views
- Checkout button clicks
- Upsell and add-on additions, including the product involved and the amount

These records are tied to the store, not to individual shoppers. We do **not** collect shopper names, email addresses, payment details, or IP addresses.

### 3.4 Order data

When an order is completed, Pro Cart may store the Shopify order ID, total value, and line items in order to attribute revenue to the cart. This data contains no customer identifiers.

## 4. Why we process this data

We process the data above in order to:

- Operate the app and render the cart correctly on your storefront
- Save and restore your configuration
- Provide analytics on cart performance
- Respond to support requests
- Comply with legal obligations

Our legal basis is the performance of our contract with the merchant, and our legitimate interest in operating and improving the service.

## 5. Where data is stored

- **Database**: PostgreSQL hosted by Neon (servers in the EU, eu-west-2)
- **Application hosting**: Railway

Both providers act as data processors on our behalf and are bound by their own security and data protection commitments.

## 6. Who we share data with

We do not sell data, and we do not share it for advertising.

Data is shared only with the infrastructure providers listed above, and with Shopify itself as part of normal app operation.

If a merchant enables the Trustpilot widget, Trustpilot's own script is loaded on the storefront and is subject to Trustpilot's privacy policy. This is optional and disabled unless the merchant turns it on.

## 7. How long we keep data

We keep configuration and analytics data for as long as the app remains installed.

When a merchant uninstalls Pro Cart, we receive Shopify's `app/uninstalled` webhook and immediately delete all data associated with that store: session and access credentials, app configuration, upsell rules, analytics events, and order records. Nothing is retained after uninstallation.

We also support Shopify's mandatory GDPR webhooks:

- `customers/data_request` — requests for a customer's stored data
- `customers/redact` — requests to delete a customer's data
- `shop/redact` — requests to delete all data for a store

Because Pro Cart does not store personal customer data, responses to customer-level requests will normally confirm that no such data is held.

## 8. Security

Access tokens and database credentials are stored as encrypted environment variables and are never exposed to the storefront. All communication between the app, Shopify, and our database uses HTTPS/TLS.

## 9. Your rights

Under the GDPR, merchants and their customers have the right to:

- Request access to personal data we hold
- Request correction of inaccurate data
- Request deletion of data
- Object to or restrict processing
- Request data portability
- Lodge a complaint with a supervisory authority. In Denmark this is Datatilsynet (datatilsynet.dk)

To exercise any of these rights, contact **contactcaziel@gmail.com**. We respond within 30 days.

## 10. Children

Pro Cart is a business tool for merchants and is not directed at children. We do not knowingly collect data from anyone under 16.

## 11. Changes to this policy

We may update this policy as the app develops. The date at the top reflects the most recent revision. Material changes will be communicated to merchants through the app or by email.

## 12. Contact

**Caziel**
CVR: 40544097
Denmark

Email: contactcaziel@gmail.com
