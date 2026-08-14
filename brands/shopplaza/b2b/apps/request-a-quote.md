# SP Request a Quote (RFQ)

> Source-of-truth file for RFQ product knowledge. Brand-level, portfolio-level and competitor knowledge live elsewhere.
> Labels used below: `VERIFIED PRODUCT FACT` = confirmed on an official Shopplaza/Shopify source. `MARKETING RECOMMENDATION` = our judgement, not product truth.

## Identity

`VERIFIED PRODUCT FACT` (listing facts verified 2026-08-14)

- Official name: **SP Request a Quote (RFQ)**
- Developer / publisher: **Shopplaza B2B** (Ha Noi, VN)
- Product line: B2B
- Status: Live on the Shopify App Store
- Shopify App Store URL: https://apps.shopify.com/mp-request-a-quote-rfq
- Shopplaza landing page: https://shopplaza.io/b2b-apps/request-a-quote/
- Documentation: https://shopplaza.io/docs/request-a-quote-rfq/
  (note: the docs path is `request-a-quote-rfq`, **not** `mp-request-a-quote-rfq` — the `mp-` form 404s)
- Launched: 14 November 2025
- App Store categories: Pricing quotes; Wholesale
- Built for Shopify badge: Yes — *verification date: 2026-08-14*
- Rating: 5.0 — *verification date: 2026-08-14*
- Review count: 17 — *verification date: 2026-08-14*
- Pricing: listed as **Free** on the App Store; the landing page states "100% Free" / "Free to Use" — *verification date: 2026-08-14*
- Languages: English — *verification date: 2026-08-14*
- Works with: Shopify Admin — *verification date: 2026-08-14*
- Install / merchant count: not published on the listing — do not cite a number
- Last verified: 2026-08-14

## Product Summary

`VERIFIED PRODUCT FACT` — SP Request a Quote (RFQ) adds a complete quotation workflow to a Shopify store. Buyers request custom pricing from the storefront (product, collection, cart pages or a floating widget), propose their own prices, attach files and track quote status. Merchants manage every request from a central quote dashboard, negotiate inside the quote, and convert agreed quotes into Shopify Draft Orders so the buyer can check out through a normal Shopify checkout link.

Official positioning line from the Shopplaza landing page: *"A Complete Quote Workflow for Shopify — Let buyers request custom pricing, negotiate offers, and accept quotes online."* The stated core problem is *"Quote Requests Shouldn't Live in Emails and Spreadsheets."*

App Store tagline: *"B2B quote requests, negotiate pricing & convert to orders."*

## Target Users

`VERIFIED PRODUCT FACT` (from official positioning)
- B2B and wholesale merchants on Shopify who sell at negotiated rather than fixed prices
- Growing B2B businesses and established sales teams that manage custom pricing workflows
- Merchants who want quote workflows without code, on any Shopify plan

`MARKETING RECOMMENDATION` — highest-intent segments to target in content and ads: wholesale/distribution, made-to-order and configurable goods, industrial/MRO supply, and merchants already hiding prices behind a login.

## Problems Solved

`VERIFIED PRODUCT FACT` (framed by official docs and landing page)
- Quote requests scattered across email threads and spreadsheets, with no single record
- No storefront path for a buyer who needs custom pricing instead of a fixed add-to-cart price
- Price negotiation happening outside the store, disconnected from the order that results
- Manual re-keying of an agreed price into an order — the app creates the Draft Order automatically
- No visibility into quote volume, acceptance and response speed

## Core Use Cases

`VERIFIED PRODUCT FACT`
- Buyer requests custom pricing on eligible products from the storefront
- Bulk / high-quantity order quoting with minimum quantity or minimum value thresholds
- Merchant-initiated quotes created from the admin for a known customer
- Back-and-forth price negotiation with attached documents (specs, POs, artwork)
- Converting an agreed quote into a Shopify Draft Order and checkout link
- Hiding prices for some customers and offering "request a quote" instead (with SP Hide Price & Access Control)

## Buyer Quote Journey

`VERIFIED PRODUCT FACT`
1. **Entry point** — buyer clicks an *Add to Quote* button on a product page, collection page, cart page or cart drawer, or opens the **floating quote widget**.
2. **Quote cart modal** — buyer reviews line items (name, image, variant, quantity, original price, proposed quote price, subtotal), adjusts quantities, edits the proposed price, and selects/removes items. An empty quote cart shows a search bar (first 20 eligible variants, A–Z); a populated cart shows a search icon.
3. **Details form** — first/last name, email, phone, company, country/region, address, city, region, postcode; required fields are marked. A comment box captures special instructions, target pricing or delivery preferences.
4. **Attachments** — buyer can attach files (PNG, PDF, JPG, JPEG, DOC on the storefront form) where the merchant has enabled attachments.
5. **Summary & submit** — buyer sees original vs. proposed totals before submitting. Submission can be blocked if minimum quote requirements are not met; an optional message explains why.
6. **Response** — merchant sends a quote; buyer receives it by email and can accept, decline, or negotiate.
7. **Acceptance** — a Shopify Draft Order is created and the buyer receives a checkout link by email.
8. **Manage Quotes portal** — logged-in buyers see Quote ID, creation time, status, expiry, value, and status-dependent actions (View/Download for active quotes; view-only for declined/expired).

`VERIFIED PRODUCT FACT` — Guests and logged-in buyers can both submit quotes; logged-in buyers get persistent quote history and chat. The Manage Quotes portal requires login.

## Merchant Quote Workflow

`VERIFIED PRODUCT FACT` — Merchants work in **Apps → SP Request a Quote (RFQ) → Manage Quotation**.

- **Create Quote** — select or add a customer, browse and add products/variants (out-of-stock variants are disabled), set quantities and custom prices. Prices auto-adjust if a minimum quote value is configured. On save, the merchant chooses *"Yes, Send now"* (status becomes **Sent**) or *"No, keep Draft."*
- **Edit** — allowed on **Draft**, **Requested by customer** and **Under Negotiation**. On **Under Negotiation**, the *Send quote* button stays disabled until something changes. **Sent**, **Accepted**, **Declined** and **Expired** quotes cannot be edited, but Declined / Expired / Accepted quotes can be **duplicated** into a new draft.
- **Negotiate** — messages are exchanged inside the quote; a **Quote Timeline** records activity, and merchants can add team-only internal notes ("Leave an internal note…") and pin up to three. System logs record detail updates and status changes automatically.
- **Shipping & tax** — merchants choose a shipping method when items and a shipping address exist; estimated tax is calculated from the buyer address and the store's Shopify tax settings. A read-only **Final total** = Subtotal + Shipping + Estimated tax.
- **List management** — search by customer name/email; filter by Status, Customer, Created date; sort by Requested time or Total value; **bulk convert** quotes (with a confirmation step).
- **PDF export** — quotes in **Sent**, **Under Negotiation** or **Accepted** can be downloaded as PDF from the detail page or the Actions column.

## Quote Lifecycle and Statuses

`VERIFIED PRODUCT FACT` — seven statuses, documented with these exact labels:

| Status | Official meaning |
|---|---|
| **Draft** | Created by the merchant, not yet sent |
| **Requested by customer** | Buyer submitted a request, waiting for the merchant to send |
| **Sent** | Merchant sent the quote to the buyer |
| **Under Negotiation** | Messages exchanged; price discussion ongoing |
| **Accepted** | Buyer accepted → Draft Order auto-created |
| **Declined** | Buyer declined |
| **Expired** | Buyer did not respond before the expiry date |

Naming note: use **"Requested by customer"**. The older internal label *"Need Send Quote"* is not used in current official documentation — treat it as legacy and do not present it as a product status. `[NEEDS VERIFICATION]` whether "Need Send Quote" still appears anywhere in the current admin UI.

**Convert quote** — `VERIFIED PRODUCT FACT`
- Available on **Draft**, **Requested by customer** and **Under Negotiation** — i.e. the merchant can skip the send/accept round trip.
- Effect: status changes to **Accepted**, a Shopify Draft Order is created, and an acceptance email is sent.
- Documented caveat: *"If Margin Protection is enabled, this action may be disabled until approval is granted."*
- Bulk conversion is supported from the quote list with a confirmation step.

**Draft Order on acceptance** — `VERIFIED PRODUCT FACT` — the generated Shopify Draft Order carries final items, quantities, negotiated prices, shipping fees and estimated tax; the buyer gets a checkout link by email.

**Expiry** — `VERIFIED PRODUCT FACT` — Settings → General → Quote Expiration sets *"Quote expire after"* (days) and *"Quote reminders send before"* (days). Expiry date = last send time + expire days; resending recalculates expiry from the most recent send. If neither accepted nor declined by expiry, status becomes **Expired** and an expiry warning email is triggered.

## Core Features

`VERIFIED PRODUCT FACT`
- Storefront quote entry points: floating quote widget + *Add to Quote* on product, collection and cart pages / cart drawer
- Buyer-proposed pricing per line item, plus a free-text comment
- Quote cart modal with variant search
- File attachments both on the request and during negotiation
- Central quote dashboard with search, filters, sorting and bulk actions
- Built-in messaging/chat per quote, plus Quote Timeline and pinned internal notes
- Merchant-created quotes and quote duplication
- Shipping method selection, estimated tax and final total on the quote
- One-click **Convert quote** → Shopify Draft Order + checkout link
- Branded quote PDF (logo, fonts, colours, field visibility, filename variables) and product info display (SKU, barcode, custom metafields)
- 8 lifecycle email notifications with template customisation, variables, live preview and test sends
- Optional custom SMTP
- Quote Analytics dashboard
- Multi-currency via Shopify Markets
- No-code setup; works across Shopify plans (per official landing page)

## Quote Eligibility

`VERIFIED PRODUCT FACT` — Settings → General → Quote eligibility. **Customer type and country eligibility must both be satisfied.**

**Customer type**
- *All customers* (default) — unrestricted
- *Selected customers* — restricted by customer segments, individual customers, or **email patterns** (e.g. `*@company.com`)

**Guest quote submissions**
- Toggle controls whether a Shopify customer account is created automatically when a guest submits a quote. When disabled, guest details are attached to the quote for later conversion.
- Guest submission only applies with **email pattern** restrictions; **segment** and **individual customer** restrictions require login.

**Country eligibility**
- *All countries* (default) or specific countries, resolved by **server-side IP geolocation**
- When geolocation cannot be determined (VPN/proxy), eligibility is *"evaluated based on your Customer type settings"*

**Product eligibility**
- *All products* or *Selected Products & Collections*

**Minimum quote requirements**
- Minimum total quantity of products and/or minimum quote value in store currency
- Logical operator *All* (both required) or *Any* (either required)
- Optional message shown when requirements are unmet; the submit button is disabled

**Attachment limits** — 10 MB per file, 5 files per message; PDF, DOC, DOCX, JPG, PNG, XLS, XLSX, CSV, TXT.

## Pricing and Margin Controls

`VERIFIED PRODUCT FACT`
- **Minimum quote value** — when configured, prices auto-adjust on merchant-created quotes, and buyer submissions below the threshold are blocked with an optional explanatory message.
- **Margin Protection** — referenced in official docs only as a gate on the Convert quote action: *"If Margin Protection is enabled, this action may be disabled until approval is granted."*

`[NEEDS VERIFICATION]` — Margin Protection is **not** documented as a configurable feature anywhere in the current Settings & Advanced Configuration article. Its settings, thresholds (e.g. cost-based floors or maximum discount %), and the approval mechanism it triggers are unverified. Do not describe Margin Protection as a shipped, configurable feature in marketing copy until confirmed with the product team.

## Automation and Approval Logic

`VERIFIED PRODUCT FACT`
- **8 lifecycle emails** fire automatically across the quote lifecycle, including Send Quote, Quote Reminder, Quote Expiry Warning and Accept Quote.
- **Automated reminders** before expiry, at a merchant-set interval.
- **Automatic expiry** to the **Expired** status, with a warning email.
- **Automatic Draft Order creation** on acceptance or conversion.
- **Automatic customer account creation** for guest submissions (toggleable).
- **Automatic system logging** of detail updates and status changes on the Quote Timeline.
- **Slack notifications** via webhook for real-time quote update alerts (documented in the official FAQ).
- **Webhooks** for sending quote data to external systems; the FAQ recommends testing with webhook.site before connecting production systems.
- **Product addition modes**: Automatic (seamless) or Manual (*Add to Quote* buttons).
- **Post-submission redirect** to a login page, optional.

`[NEEDS VERIFICATION]` — auto-approval rules, approval workflows, and team-member permissions/roles are not documented in the current official articles. Do not claim them.

## Buyer Experience

`VERIFIED PRODUCT FACT` — Covered in full under **Buyer Quote Journey**. Distinguishing points worth carrying into copy:
- Buyer proposes their own price per line item, so the first message already contains a number
- Quote cart summary shows original vs. proposed totals before submitting
- Real-time status tracking and quote history in the Manage Quotes portal (login required)
- Attachments on both the initial request and during negotiation
- Guest quoting supported; logged-in buyers additionally get persistent history and chat

## Admin Experience

`VERIFIED PRODUCT FACT`
- Embedded in Shopify Admin under **Apps → SP Request a Quote (RFQ)**
- Manage Quotation list: search, Status/Customer/Created-date filters, sort by requested time or total value, bulk convert, per-row PDF download
- Quote detail: line items, negotiated prices, shipping method, estimated tax, read-only final total, messaging, Quote Timeline, internal notes (up to 3 pinned)
- Settings: quote ID format, quote eligibility, product eligibility, product info display and metafields, conversation settings, quote PDF, integrations, quote expiration, SMTP
- Email editor: 4 template designs (Classic, Editorial, Document, Sidebar Timeline), subject/code editing, variable insertion, live preview, test send, reset to default
- Admin dashboards display the store's timezone and currency from Shopify Markets settings

## Analytics

`VERIFIED PRODUCT FACT` — Quote Analytics dashboard, three blocks:

**1. Performance snapshot** — four metrics, each with a +/- % change vs. the previous comparable period:
- *Total quotes* — total number of quotes created
- *Acceptance rate* — percentage of quotes accepted by customers
- *Total quote value* — combined value of all quotes
- *Avg response time* — average time from quote request to merchant response

**2. Quote Volume Trend** — current vs. previous period side by side; uses quote count regardless of the currency filter.

**3. Top Opportunities** — three ranking tables: customers by quote count and value; most frequently quoted products; products with the highest acceptance rates.

**Filters** — date range (default: Last 30 days), quote status (all or specific), currency.

`[NEEDS VERIFICATION]` — analytics export/CSV is not documented. Do not claim it.

## Integrations

Classified per official evidence only:

| Integration | Class | Evidence |
|---|---|---|
| **SP Hide Price & Access Control** | **Native integration** | Named in the app's own Settings → Integrations section; merchants click *"Create Hide Price rule"* to hide prices and replace Add to Cart with Request a Quote. Quotes still submit normally and are managed inside RFQ. |
| **Shopify Draft Orders** | **Platform integration** | Accepted/converted quotes auto-create a Shopify Draft Order with a checkout link |
| **Shopify customer segments** | **Platform integration** | Used directly as a quote eligibility target |
| **Shopify Markets** | **Platform integration** | Quote currency preserved from the market at send time; all conversion and rounding rely on the store's Markets setup (Shopify exposes no public conversion-rate API) |
| **Shopify Admin** | **Platform integration** | Listed under "Works with" on the App Store listing |
| **Slack** | **Webhook/API capability** | Documented in the official FAQ as webhook-based real-time quote update notifications — not an OAuth Slack app |
| **Custom webhooks (CRM/ERP)** | **Webhook/API capability** | FAQ documents sending quote data to external endpoints, tested via webhook.site. No named CRM/ERP connector exists |
| **Custom SMTP** | **Platform capability** | Host/port/auth/username/password, with Gmail/GSuite auto-population and verification testing |

Do not describe Slack or CRM/ERP as "native integrations" — they are webhook-based.

## Relationship With Other Shopplaza Apps

`VERIFIED PRODUCT FACT`
- **SP Hide Price & Access Control** — the only Shopplaza app with a documented in-product integration. Hide Price controls *who sees prices* and swaps Add to Cart for Request a Quote; RFQ owns the quote itself. This is the anchor bundle for B2B storefronts.

`MARKETING RECOMMENDATION` — other B2B apps (SP Login As Customer, B2B Signup & Company Profiles, SP Smart Shipping & Batching, Wholesale Pricing) are **complementary / cross-sell only** in the absence of documented technical integration. Position them as workflow neighbours (account creation → price visibility → quoting → order handling), not as connected features.

`[NEEDS VERIFICATION]` — whether any RFQ-side data flows exist with B2B Signup & Company Profiles or Wholesale Pricing.

## Key Differentiators

`VERIFIED PRODUCT FACT` (each traceable to an official source)
- Buyer-side price proposal built into the quote cart — the request arrives with a number attached
- Built-in per-quote messaging with file attachments, replacing email threads
- **Convert quote** direct from Draft / Requested by customer / Under Negotiation, skipping the send-accept round trip
- Native Shopify Draft Order output with checkout link, shipping and estimated tax
- Built for Shopify badge (*verified 2026-08-14*)
- Free (*verified 2026-08-14*)
- Documented integration with SP Hide Price & Access Control
- Quote Analytics with previous-period comparison built in

`MARKETING RECOMMENDATION` — lead with the combination of *free + Built for Shopify + full negotiation-to-draft-order loop*, since paid competitors typically charge for the negotiation and conversion layer. Verify competitor pricing under `b2b/competitors/` before making comparative claims.

## Proof Points

`VERIFIED PRODUCT FACT` — usable as-is, with the verification date attached:
- 5.0 rating from 17 reviews on the Shopify App Store (*2026-08-14*)
- Built for Shopify badge (*2026-08-14*)
- Free, no monthly subscription (*2026-08-14*)
- Merchant testimonials from UK and Colombia merchants on the official landing page, citing support quality and functionality
- Published by Shopplaza B2B; launched 14 November 2025

Do not use: install counts, merchant counts, conversion lift, revenue lift, quote acceptance improvement, time-saved figures. None are published.

## SEO Topics

`MARKETING RECOMMENDATION` — not official positioning. Prioritised by intent:
- "request a quote Shopify app" / "Shopify RFQ app"
- "how to add a request a quote button on Shopify"
- "Shopify quote management for B2B / wholesale"
- "hide price and request a quote on Shopify" (bundle intent, pairs with SP Hide Price)
- "convert a quote into a Shopify draft order"
- "Shopify B2B price negotiation workflow"
- "wholesale quote request form Shopify"
- "quote expiration and follow-up automation for B2B"

## ASO Positioning

`MARKETING RECOMMENDATION` — keyword candidates, not verified listing metadata:
- Primary: request a quote, RFQ, quote app, B2B quote
- Secondary: wholesale quote, hide price request quote, negotiate price, draft order, quote management, custom pricing, bulk order quote
- Listing categories already held: Pricing quotes; Wholesale (`VERIFIED PRODUCT FACT`)

`MARKETING RECOMMENDATION` — the strongest listing assets to emphasise are the Built for Shopify badge, the free price point, and the negotiate → convert-to-draft-order loop.

## Messaging

`VERIFIED PRODUCT FACT` — official lines available for reuse verbatim:
- "A Complete Quote Workflow for Shopify"
- "Let buyers request custom pricing, negotiate offers, and accept quotes online."
- "Quote Requests Shouldn't Live in Emails and Spreadsheets."
- "B2B quote requests, negotiate pricing & convert to orders"

`MARKETING RECOMMENDATION` — angles to test:
- *Close the loop*: request → negotiate → draft order, without leaving Shopify
- *Get their number first*: buyers propose a price up front, so negotiation starts with data
- *Stop losing quotes in the inbox*: one dashboard, timeline and status per deal
- *Gate and quote*: pair with SP Hide Price & Access Control for price-hidden B2B catalogues
- *Free, and Built for Shopify*

## Claims Allowed

- Free to install and use (*with 2026-08-14 verification date*)
- Built for Shopify (*with date*)
- 5.0 rating from 17 reviews (*with date*)
- Buyers can request quotes from product, collection and cart pages or a floating widget
- Buyers can propose prices and attach files
- Merchants can negotiate inside the app and convert quotes to Shopify Draft Orders
- Seven quote statuses, as named above
- Quote eligibility by customer segment, individual customer, email pattern and country
- Minimum quantity and minimum quote value thresholds
- Automated reminder and expiry emails; optional custom SMTP
- Quote analytics with previous-period comparison
- Documented integration with SP Hide Price & Access Control
- Slack and external-system notifications via webhooks

## Claims To Avoid

- "Best", "#1", "leading", "most popular", "fastest", "highest rated"
- "Trusted by thousands", any install or merchant count
- Any conversion, revenue, acceptance-rate or time-saved improvement figure
- Margin Protection as a configurable feature (see `[NEEDS VERIFICATION]` above)
- Approval workflows, auto-approval, or team-member permissions/roles
- "Native Slack integration" or "CRM/ERP integration" — these are webhook-based
- Multi-language support — the listing shows English only (*2026-08-14*)
- Analytics export
- Comparative claims against named competitors without evidence in `b2b/competitors/`

## Limitations / Dependencies

`VERIFIED PRODUCT FACT`
- Requires the theme app embed to be enabled; the FAQ's first troubleshooting step is enabling app embeds, refreshing status, checking display settings and clearing theme cache
- Storefront widget behaviour depends on theme integration
- Currency conversion depends entirely on the store's Shopify Markets configuration — Shopify exposes no public conversion-rate API
- Estimated tax depends on the store's Shopify tax settings and the buyer's address
- **Sent**, **Accepted**, **Declined** and **Expired** quotes cannot be edited (duplication is the workaround)
- The Manage Quotes buyer portal requires login; guests do not get persistent history or chat
- Segment- and individual-customer eligibility restrictions require the buyer to be logged in; only email-pattern restrictions support guest submission
- Country eligibility relies on server-side IP geolocation and falls back to customer-type rules when geolocation fails (VPN/proxy)
- Attachments capped at 10 MB per file, 5 files per message
- Email deliverability may require SMTP configuration and SPF/DKIM/DMARC domain authentication
- English only on the listing (*2026-08-14*)

`[NEEDS VERIFICATION]` — the App Store lists the app as Free with no tiers, but the email documentation states the Classic template design is "Classic only on Free plan," implying paid plans exist or are planned. Confirm the current plan structure before writing pricing copy.

## Sources

All verified 2026-08-14.

1. Shopify App Store listing — https://apps.shopify.com/mp-request-a-quote-rfq
2. Shopplaza landing page — https://shopplaza.io/b2b-apps/request-a-quote/
3. Docs — Overview — https://shopplaza.io/docs/request-a-quote-rfq/
4. Docs — How to Manage Quotes (Merchant side) — https://shopplaza.io/docs/request-a-quote-rfq/how-to-manage-quotes
5. Docs — How to Customize Storefront Experience (Buyer side) — https://shopplaza.io/docs/request-a-quote-rfq/how-to-customize-storefront-experience
6. Docs — How to Automate Communication & Email — https://shopplaza.io/docs/request-a-quote-rfq/how-to-automate-communication-email
7. Docs — Settings & Advanced Configuration — https://shopplaza.io/docs/request-a-quote-rfq/settings-advanced-configuration
8. Docs — Quote Analytics — https://shopplaza.io/docs/request-a-quote-rfq/quote-analytics
9. Docs — Currency and Markets — https://shopplaza.io/docs/request-a-quote-rfq/currency-markets
10. Docs — FAQs — https://shopplaza.io/docs/request-a-quote-rfq/faqs

Other doc articles not consulted (low marketing value): On-site Content, Customize Quote Cart Template, Language.
