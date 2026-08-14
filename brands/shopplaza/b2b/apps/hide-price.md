# SP Hide Price & Access Control

## Identity

- **Official name:** SP Hide Price & Access Control
- **App Store tagline:** "Hide price, login to see price, wholesale lock pages"
- **Developer (App Store):** Shopplaza B2B
- **Product line:** B2B — see [b2b-context.md](../b2b-context.md)
- **Status:** Live on the Shopify App Store (listed since 14 Aug 2025)
- **Shopify App Store URL:** https://apps.shopify.com/hide-price-access-control
- **Shopplaza landing page:** https://shopplaza.io/b2b-apps/hide-price-access-control/
- **Documentation:** https://shopplaza.io/docs/hide-price-access-control/
- **App Store categories:** Pricing quotes (primary), Accounts and login (secondary)
- **Last verified:** 2026-08-14

Brand-level identity, partner pages and social channels live in [brand-context.md](../../brand/brand-context.md). Naming conventions (the `SP` prefix) live in [terminology.md](../../shared/terminology.md).

---

## Product Summary

VERIFIED PRODUCT FACT — SP Hide Price & Access Control lets merchants hide prices and lock pages, products, or collections behind rules based on login status, customer segment/tag, email, country, IP address, password, or age. Hidden prices can be replaced with a custom message and CTA (login, contact, request a quote, WhatsApp, call for price). Setup requires no coding and the app works on any Shopify plan.

Two rule engines run side by side:

1. **Hiding Price Rules** — the price is concealed, the page stays reachable.
2. **Access Rules** — the product, collection, page, or URL itself is blocked or redirected.

---

## Target Users

VERIFIED PRODUCT FACT — the landing page names three merchant types:

- B2B store operators
- Wholesale businesses
- Multi-segment sellers running B2B and B2C on one store

Broader B2B audience definition is maintained in [b2b-context.md](../b2b-context.md); do not restate it here.

---

## Problems Solved

- Public retail pricing exposes wholesale rates to retail shoppers and competitors. The landing page frames this as: *"Public Pricing Is Costing You Wholesale Deals."*
- Merchants have no native Shopify way to gate pricing by customer segment without theme code edits.
- Wholesale or trade-only catalogs need to stay off-limits to the general public.
- Prices leak into Google Search results even after they are hidden on the storefront (the app addresses this — see Limitations for the required theme step).
- Region-, IP-, or age-restricted catalogs need gating that Shopify does not provide natively.

---

## Core Use Cases

- Hide prices from guest (not logged-in) visitors — the docs flag this as the recommended setting for wholesale/B2B.
- "Login to see price": show prices only to approved or logged-in customers.
- Hide prices only for specific customer segments/tags, specific emails, or specific countries.
- Lock a wholesale collection, product set, page, or custom URL entirely.
- Password-protect private or pre-release content.
- Age-gate age-restricted products.
- Block access by country or by IP address.
- Replace hidden prices with a "Request a Quote," "Contact Us," "Call for Pricing," or WhatsApp CTA to keep the lead in the funnel.
- Keep prices out of Google Search results for trade-only catalogs.

---

## Core Workflow

VERIFIED PRODUCT FACT — Hide Price rule creation (from the official docs):

1. Open the app in Shopify Admin → **Hiding Price Rules** → **Add Rule**.
2. Set rule name, optional internal description, and active/inactive status.
3. Choose scope: all products, specific products, or products in selected collections.
4. Define audience: all customers / block guest visitors / customer segments (tags) / specific email addresses — combinable with country conditions.
5. Choose the replacement display: custom message with button, Request a Quote, Get Price on WhatsApp, or Call for Price.
6. Check the **Quick Preview** panel, then save.

Access Rule creation follows six phases: open **Access Rules** → general settings → select protected content → choose protection type → configure redirect and messaging → save.

---

## Core Features

VERIFIED PRODUCT FACT:

- Hide prices on products, collections, pages, and Google Search results
- "Login to see price" gating for approved or logged-in customers
- Page/product/collection locking by login, customer tag, location, IP, or age
- Replace hidden prices with a Login button, WhatsApp link, or custom CTA
- Real-time rule preview
- Bulk rule management
- Conflict detection between overlapping rules
- API support (stated on the App Store listing) — scope and endpoints [NEEDS VERIFICATION]
- Per-language rule messages with a required Default message and automatic fallback
- Global enable/disable toggle for all rules
- Custom CSS for storefront messages (color, spacing, font, layout)

---

## Targeting and Eligibility Logic

VERIFIED PRODUCT FACT.

**Hide Price rules — audience conditions**

| Dimension | Options |
|---|---|
| User | All customers · Block guest visitors (not logged in) · Customer segments (tags) · Specific email addresses |
| Location | All countries · One or more specific countries |

Conditions combine (e.g. guests **AND** selected countries).

**Hide Price rules — content scope**

- All products
- Specific products
- Products within selected collections

**Access Rules — five protection types**

| Type | Detail |
|---|---|
| User-based | Block unauthenticated visitors · exclude specific customer segments/tags · restrict named email addresses · combinable. Docs mark this "recommended for B2B/wholesale." |
| Geographic | Block one or multiple countries |
| IP address | IPs entered one per line, each with an optional note identifying the group |
| Password | 4–50 characters, strength indicator, optional hint, 1–10 attempt limit |
| Age verification | Age range 1–100, custom title/description, optional image (JPG/PNG/GIF), optional terms checkbox, custom agree/disagree buttons |

**Access Rules — protectable content:** all products or selected products · collections (via product selection) · pages (searchable, individually selected) · custom URLs (relative paths starting with `/` or full URLs, one per line).

---

## Merchant Configuration

VERIFIED PRODUCT FACT:

- Rule name, internal description, active/inactive toggle per rule
- Rule list with status, applied items, and edit / duplicate / delete actions
- App-level enable/disable switch that activates or deactivates all rules at once
- Admin interface language selection (does **not** change storefront messages)
- Advanced settings: custom CSS for storefront message styling
- Replacement CTA configuration: button text, styling, and destination
- Access Rule redirect destination: login page, 404, registration page, homepage, or custom URL
- Configurable auto-redirect delay in seconds
- Blocked-content messaging: headline, description, CTA button text and styling
- Per-language message variants

---

## Storefront Experience

VERIFIED PRODUCT FACT:

- Where a Hide Price rule matches, the price is replaced by the configured message and CTA rather than left blank.
- Replacement CTA options: Login button, custom message + button, Request a Quote, Get Price on WhatsApp, Call for Price.
- Where an Access Rule matches, the visitor sees the configured block message or is redirected to the chosen destination after the configured delay.
- Password-protected content prompts for a password with an optional hint and a bounded number of attempts.
- Age-gated content shows a verification screen with optional image and terms checkbox.
- Storefront messages render in the visitor's language when a variant exists, otherwise fall back to the Default message.
- Storefront message styling is CSS-customizable.

---

## Admin Experience

VERIFIED PRODUCT FACT:

- Embedded in Shopify Admin under Apps; App Store lists "Works with: Shopify Admin."
- Built on Shopify Polaris; the app reports "Built for Shopify" status.
- Separate list views for Hiding Price Rules and Access Rules.
- Live preview panel on the right during rule setup; Quick Preview for hidden-price display.
- Conflict detection warns when overlapping rules may misbehave.
- No coding required for standard setup; docs state setup takes a few minutes.
- Support is described as 24/7, including theme-code adjustments where a theme needs them.

---

## Integrations

Verification date: 2026-08-14.

**Native integration**

- **SP Request a Quote (RFQ)** — the Hide Price replacement display offers a "Request a Quote" option that requires the RFQ app to be installed and enabled. The app warns when RFQ is selected but not enabled, and **automatically pauses affected Hide Price rules if the RFQ app is later disabled.** This dependency is documented in the official Hide Price rule guide.

**Platform**

- **Shopify Admin** — the only entry in the App Store "Works with" list.
- **Shopify customer segments / customer tags** — used as targeting input for both rule engines.
- **API support** — stated on the App Store listing; capabilities not documented. [NEEDS VERIFICATION]

**Compatible workflow**

- **Theme layer** — works with most themes automatically; some themes need extra setup, and Google schema Price/Offer markup must be removed or commented out to keep hidden prices out of search results.

**Cross-sell / complementary app (no verified technical integration)**

The Shopplaza landing page lists these as related B2B apps, not as integrations: SP B2B Wholesale Pricing, B2B Signup & Company Profiles, SP Login As Customer, SP Smart Shipping & Batching.

---

## Relationship With Other Shopplaza Apps

- **SP Request a Quote (RFQ)** — the one verified functional dependency. Hide Price gates the price; RFQ captures the lead. This is the strongest bundle story and the only one that can be described as a native integration.
- **SP B2B Wholesale Pricing** — complementary in concept (Hide Price controls *who sees* pricing; Wholesale Pricing controls *what price* they get), but no source verifies a technical integration between the two. Describe as complementary, not integrated. [NEEDS VERIFICATION] for any shared configuration.
- **B2B Signup & Company Profiles**, **SP Login As Customer**, **SP Smart Shipping & Batching** — listed as related B2B apps on the Shopplaza site; treat as cross-sell only.

Portfolio-wide relationships are maintained in [integration-map.md](../integration-map.md); see section E of the accompanying report for a correction recommended there.

---

## Key Differentiators

VERIFIED PRODUCT FACT:

- **Two engines in one app** — price hiding and full content/access locking, rather than price hiding alone.
- **Six targeting dimensions** — login status, customer segment/tag, email, country, IP, age — plus password protection.
- **Free with all features unlocked**, on any Shopify plan; Shopify Plus is not required.
- **Built for Shopify** badge.
- **Search-result price hiding**, not just storefront hiding.
- **Conflict detection** across overlapping rules.
- **Live preview** before publishing.
- **Per-language rule messages** with default fallback.
- **Access Rules cover custom URLs**, not only Shopify-native objects.

---

## Proof Points

Verification date: 2026-08-14. These are dynamic — re-verify before use in any published asset.

- Shopify App Store rating: **5.0** from **51 reviews** (98% five-star, 2% four-star)
- **Built for Shopify** badge present on the listing
- Listed since **14 August 2025**
- Pricing: **Free** — the listing shows no paid plans
- Supported languages (19): English, German, Chinese (Simplified), Chinese (Traditional), Czech, Danish, Spanish, French, Italian, Dutch, Norwegian (Bokmål), Polish, Portuguese (Brazil), Portuguese (Portugal), Finnish, Swedish, Turkish, Thai, Japanese, Korean
- Merchant testimonials on the Shopplaza landing page emphasise ease of setup and support quality

Install count is not published on the listing. [NEEDS VERIFICATION]

---

## SEO Topics

MARKETING RECOMMENDATION — topic opportunities, not official positioning. Methodology lives in [seo-rules.md](../../shared/seo-rules.md).

Existing Shopplaza content already ranking on these themes (verified live):

- https://shopplaza.io/blog/how-to-hide-prices-on-shopify.html
- https://shopplaza.io/blog/hide-shopify-store.html
- https://shopplaza.io/blog/best-shopify-b2b-apps/

Recommended topic gaps to build toward the app:

| Intent | Topic |
|---|---|
| Informational | "Login to see price" on Shopify — how it works |
| Informational | How to stop Shopify prices appearing in Google Search results |
| Informational | Shopify age verification for restricted products |
| Informational | Block Shopify store access by country or IP |
| Informational | Password-protect a Shopify page or collection |
| Commercial | Best Shopify apps to hide prices |
| Commercial | Shopify wholesale-only store setup guide |
| Commercial | Hide price vs. B2B catalog: which fits your store |
| Transactional | The app landing page at `/b2b-apps/hide-price-access-control/` |

Internal linking should follow the funnel rules in [seo-rules.md](../../shared/seo-rules.md) — explain the problem before linking to the app, and pair hide-price content with RFQ content given the verified dependency.

---

## ASO Positioning

MARKETING RECOMMENDATION unless marked otherwise. Methodology lives in [aso-rules.md](../../shared/aso-rules.md).

VERIFIED PRODUCT FACT — the live listing title is "SP Hide Price & Access Control" with the tagline "Hide price, login to see price, wholesale lock pages," in the Pricing quotes and Accounts and login categories.

Recommended keyword targets:

- **Primary:** hide price shopify
- **Secondary:** login to see price · shopify wholesale lock · hide price app · call for price shopify · b2b pricing visibility
- **Feature keywords:** age verification shopify · password protect page shopify · block country shopify · restrict collection shopify · hide price from google
- **Problem keywords:** stop competitors seeing my prices · wholesale prices visible to public · trade-only shopify store

Positioning concepts to test, following the Benefit → How → Outcome rule:

- "Choose exactly who sees your prices — guests, tagged segments, or whole countries — so wholesale rates stay between you and your buyers."
- "Turn a hidden price into a lead: swap it for Request a Quote, Contact Us, or Call for Pricing."
- "Hide the price and lock the page — one app for both, free on every Shopify plan."

Conversion levers already supported by verified facts: free with all features unlocked, Built for Shopify, no coding, works on every Shopify plan, live preview, 5.0 rating.

---

## Messaging

Approved angles, each backed by a verified fact:

1. **Pricing privacy** — "Public pricing is costing you wholesale deals." (Landing page copy.)
2. **Login to see price** — approved/logged-in customers see pricing; guests do not.
3. **Two jobs, one app** — hide the price *and* lock the content.
4. **Granular targeting** — login, segment, email, country, IP, password, age.
5. **Hidden price becomes a lead** — Request a Quote, WhatsApp, Call for Price CTAs.
6. **Zero friction** — free, no code, minutes to set up, works on every Shopify plan.
7. **Preview before you publish** — live preview plus conflict detection.
8. **Beyond the storefront** — keeps prices out of Google Search results.

Tone and terminology (merchant / install / listing) per [terminology.md](../../shared/terminology.md). CTA convention: "Try free on Shopify App Store."

---

## Claims Allowed

- "Free" and "all features unlocked" — verified 2026-08-14; re-verify before publishing.
- "Built for Shopify" — badge verified on the listing 2026-08-14.
- "No coding required" — stated in official docs and landing page (note the schema-markup caveat below).
- "Works with every Shopify plan" / "Shopify Plus not required" — stated on the landing page.
- "Rated 5.0 on the Shopify App Store" — with the review count and verification date attached.
- "Set up in minutes" — stated on the landing page.
- "24/7 support" — stated on the landing page and docs.
- Specific feature and targeting claims listed in Core Features and Targeting sections above.
- "Available in 19 languages" (admin interface; storefront messages are configured per language by the merchant).

## Claims To Avoid

- "Best," "#1," "leading," "top-rated," "highest rated," "most popular" — no source supports any of these.
- "Trusted by thousands of merchants" — install count is not published.
- "X+ installs" or any install-count figure.
- "Free forever" — the listing shows a free plan today, not a permanent commitment.
- "Integrates with Wholesale Pricing / Company Accounts / Login As Customer / Smart Shipping" — only the RFQ dependency is verified.
- "Removes prices from Google instantly" — removal takes days to weeks and depends on Google recrawl.
- "Works with every theme with zero setup" — some themes need extra setup.
- "Hides prices while staying eligible for Google Shopping" — hidden prices cause Google Shopping product disapproval.
- Any revenue-lift, conversion-lift, or margin-protection percentage — no data source exists.

---

## Limitations / Dependencies

VERIFIED PRODUCT FACT, from official docs:

- **Google schema markup must be edited manually.** Price/Offer schema tags have to be removed or commented out from theme code, otherwise hidden prices still surface in search results. This is the one step that is not no-code.
- **Search-result removal is not immediate** — a few days to a few weeks, depending on Google's recrawl schedule.
- **Google Shopping incompatibility** — Google Shopping requires visible pricing; hiding prices causes product disapproval. Docs recommend organic search, SEO, and display ads with "Request a Quote" CTAs instead.
- **RFQ dependency** — the Request a Quote replacement option requires the SP Request a Quote app to be installed and enabled. If RFQ is disabled, affected Hide Price rules automatically pause.
- **Access Rules are blacklist-only** — docs state a whitelist option "will be available soon."
- **Theme variance** — some themes require extra setup for consistent price display; support can adjust theme code.
- **Admin language ≠ storefront language** — changing the app's admin language does not change storefront messages; those are configured per language per rule.
- **Rule conflicts** — overlapping rules can misbehave; the app surfaces warnings but the merchant resolves them.
- **Plan dependencies** — none found. The app is free and the landing page states it works on every Shopify plan.

---

## Sources

All fetched and verified 2026-08-14.

1. Shopify App Store listing — https://apps.shopify.com/hide-price-access-control
2. Shopplaza app landing page — https://shopplaza.io/b2b-apps/hide-price-access-control/
3. Shopplaza docs overview — https://shopplaza.io/docs/hide-price-access-control/
4. Shopplaza docs, Hide Price rule — https://shopplaza.io/docs/hide-price-access-control/how-to-create-a-hide-price-rule/
5. Shopplaza docs, Access Control rule — https://shopplaza.io/docs/hide-price-access-control/how-to-create-an-access-control-rule/
6. Shopplaza docs, FAQs — https://shopplaza.io/docs/hide-price-access-control/faqs
7. Shopplaza homepage app index — https://shopplaza.io/
8. Repository context — [brand-context.md](../../brand/brand-context.md), [product-portfolio.md](../../brand/product-portfolio.md), [b2b-context.md](../b2b-context.md), [terminology.md](../../shared/terminology.md)
