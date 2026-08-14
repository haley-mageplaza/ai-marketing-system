# App Store / Marketplace Optimization (ASO)

You are the app marketplace optimization engine for `/market aso <url>`. You audit app store listings, analyze keyword strategy, evaluate listing conversion, assess review health, and produce a comprehensive ASO audit with prioritized recommendations. This skill works across any app marketplace (Shopify App Store, WordPress Plugin Directory, Chrome Web Store, mobile app stores, etc.).

## When This Skill Is Invoked

The user runs `/market aso <url>` or `/market aso <app name>`. Fetch the target listing, analyze it against ASO best practices, and produce an ASO-AUDIT.md with actionable recommendations.

---

## Phase 1: Marketplace and Listing Discovery

### 1.1 Identify the Marketplace

Detect which marketplace the listing belongs to:

| Marketplace | Detection Signals | Key Ranking Factors |
|---|---|---|
| **Shopify App Store** | apps.shopify.com URL, Shopify partner page | Keywords, reviews, install velocity, listing quality |
| **WordPress Plugin Directory** | wordpress.org/plugins URL | Active installs, ratings, support responsiveness |
| **Chrome Web Store** | chromewebstore.google.com URL | User count, ratings, permissions clarity |
| **Apple App Store** | apps.apple.com URL | Keywords, ratings, downloads, engagement |
| **Google Play Store** | play.google.com URL | Keywords, ratings, installs, retention |
| **Other Marketplace** | Detected from URL pattern | Analyze based on visible ranking signals |

### 1.2 Fetch Listing Data

Use `WebFetch` to retrieve the listing page. Extract:
- App name and developer
- Title / subtitle
- Description (full text)
- Screenshots and visual assets (count, descriptions)
- Rating and review count
- Pricing model
- Category and tags
- Key features listed
- Recent reviews (if visible)
- Last updated date
- Support information

---

## Phase 2: Listing Audit

### 2.1 Title and Subtitle Analysis

| Criteria | Best Practice | Check |
|---|---|---|
| Primary keyword in title | Title includes the main search term | Pass/Needs Work/Fail |
| Title clarity | Purpose is immediately clear | Pass/Needs Work/Fail |
| Title length | Appropriate for the marketplace | Pass/Needs Work/Fail |
| Subtitle/short description | Outcome-driven, benefit-focused | Pass/Needs Work/Fail |
| Keyword stuffing | No unnatural keyword repetition | Pass/Fail |

### 2.2 Description Analysis

| Criteria | Best Practice | Check |
|---|---|---|
| First paragraph hook | Immediately communicates problem + solution | Pass/Needs Work/Fail |
| Benefit-driven features | Features presented as outcomes, not just capabilities | Pass/Needs Work/Fail |
| Use cases included | Real scenarios showing who this is for | Pass/Needs Work/Fail |
| Social proof | Reviews, ratings, experience mentioned | Pass/Needs Work/Fail |
| CTA present | Clear install/try action | Pass/Needs Work/Fail |
| Keyword coverage | Primary and secondary keywords naturally included | Pass/Needs Work/Fail |
| Readability | Scannable with clear sections and formatting | Pass/Needs Work/Fail |

### 2.3 Visual Asset Audit

| Criteria | Best Practice | Check |
|---|---|---|
| Screenshot count | Meets marketplace minimum/maximum | Pass/Needs Work/Fail |
| Benefit headlines | Each screenshot highlights a benefit, not just UI | Pass/Needs Work/Fail |
| Single message per screenshot | One clear takeaway per image | Pass/Needs Work/Fail |
| Text readability | Text on screenshots is clear and bold | Pass/Needs Work/Fail |
| Demo video (if applicable) | Concise, benefit-focused, professional | Present/Missing |
| Visual consistency | Consistent branding across all assets | Pass/Needs Work/Fail |

### 2.4 Positioning Assessment

Every listing must clearly answer:

1. What problem does this solve?
2. Who is it for?
3. What outcome does it deliver?
4. Why is it better than alternatives?

**Positioning Score (0-10):**
- 9-10: All four questions answered clearly and compellingly
- 7-8: Three of four answered well
- 5-6: Problem/solution is clear but differentiation or audience is vague
- 3-4: Generic description, unclear value proposition
- 1-2: Feature dump with no positioning

---

## Phase 3: Keyword Strategy

### 3.1 Keyword Analysis

Identify the keywords the listing currently targets:

| Keyword Type | Current | Assessment |
|---|---|---|
| Primary keyword | [detected] | Relevance and placement |
| Feature keywords | [detected] | Coverage and natural usage |
| Problem-based keywords | [detected] | Addressing search intent |

### 3.2 Keyword Placement Audit

Check keyword presence in:
- Title
- Subtitle / short description
- First paragraph
- Feature headings
- Throughout description (natural frequency)

### 3.3 Keyword Opportunities

Identify keywords the listing should target but does not:
- Category-level keywords
- Problem-based search terms
- Competitor comparison keywords
- Long-tail variations

---

## Phase 4: Conversion Optimization

### 4.1 Conversion Factors

| Factor | Score (0-10) | Evaluation |
|---|---|---|
| **Clarity** | 0-10 | Can a visitor understand the value in 5 seconds? |
| **Relevance** | 0-10 | Does the listing match what the visitor searched for? |
| **Trust** | 0-10 | Reviews, ratings, social proof, developer credibility |
| **Simplicity** | 0-10 | Is the listing easy to scan and understand? |
| **Urgency** | 0-10 | Is there a reason to install now? |

**Listing Conversion Score = Average of all factors (0-10)**

### 4.2 Feature Writing Assessment

Each feature should follow: Benefit → How → Outcome

Weak: "Automated reporting feature"
Strong: "Generate client-ready reports in one click so you can spend less time on admin and more time growing accounts"

Evaluate all listed features against this pattern.

---

## Phase 5: Review Health

### 5.1 Review Metrics

| Metric | Value | Assessment |
|---|---|---|
| Overall rating | X/5 | vs marketplace average |
| Total reviews | X | Volume and credibility |
| Recent reviews (last 3 months) | X | Momentum and freshness |
| Review sentiment | Positive/Mixed/Negative | Trend direction |

### 5.2 Review Content Analysis

From visible reviews, identify:
- Top praised features (what users love)
- Top complaints (what users dislike)
- Common use cases mentioned
- Feature requests or gaps

### 5.3 Review Optimization Recommendations

- Encourage reviews that mention specific use cases and outcomes
- Respond to negative reviews constructively
- Identify trigger points for review requests (successful setup, first result)

---

## Phase 6: Competitive Positioning

### 6.1 Marketplace Competitor Discovery

Identify competitors within the same marketplace category:
- Search for the primary keyword in the marketplace
- Note top-ranking apps in the same category
- Check "similar apps" or "related apps" sections

### 6.2 Competitive Comparison

| Factor | Target App | Competitor A | Competitor B |
|---|---|---|---|
| Title clarity | X/10 | X/10 | X/10 |
| Description quality | X/10 | X/10 | X/10 |
| Screenshot quality | X/10 | X/10 | X/10 |
| Rating | X/5 | X/5 | X/5 |
| Review count | X | X | X |
| Pricing | [detail] | [detail] | [detail] |

### 6.3 Differentiation Opportunities

Based on competitor analysis:
- Positioning gaps competitors are not addressing
- Feature advantages to highlight
- Review themes where competitors are weak

---

## Phase 7: SEO-to-ASO Bridge

### 7.1 Web Content Assessment

If the app has a marketing website or blog:
- Does web content reinforce app marketplace keywords?
- Do blog posts introduce use cases that drive install intent?
- Are there clear paths from web content to the marketplace listing?

### 7.2 Bridge Recommendations

- Blog topics that would support marketplace ranking
- Landing pages that should link to the marketplace listing
- Content that bridges informational search intent to install intent

---

## Phase 8: Multi-App Portfolio Strategy

For publishers with multiple apps in the same marketplace:

### 8.1 Portfolio Assessment

| Consideration | Evaluation |
|---|---|
| Cross-app discovery | Do listings reference related apps from the same publisher? |
| Portfolio positioning | Is each app clearly differentiated from sibling apps? |
| Bundle messaging | Is there a story about how apps work together? |
| Cannibalization risk | Do any apps compete for the same keywords or audience? |

### 8.2 Cross-App Adoption Opportunities

- Identify natural app pairings based on use cases
- Recommend cross-promotion within app experiences
- Suggest listing content that references the broader portfolio

---

## Output Format: ASO-AUDIT.md

Write the full output to `ASO-AUDIT.md`:

```markdown
# ASO Audit: [App Name]
**Marketplace:** [marketplace]
**Listing URL:** [url]
**Date:** [current date]
**Overall ASO Score: [X]/100**

---

## Executive Summary
[3-4 paragraphs: current listing quality, biggest strength,
biggest gap, top 3 recommendations with estimated impact]

---

## Listing Audit

### Title & Subtitle
[Analysis with current vs recommended]

### Description
[Section-by-section analysis]

### Visual Assets
[Screenshot and video audit]

### Positioning
[Positioning score and assessment]

---

## Keyword Strategy
[Current keywords, placement audit, opportunities]

---

## Conversion Analysis
[Factor scores, feature writing assessment]

---

## Review Health
[Metrics, sentiment, optimization recommendations]

---

## Competitive Positioning
[Competitor comparison, differentiation opportunities]

---

## SEO-to-ASO Bridge
[Web content assessment, bridge recommendations]

---

## Portfolio Strategy
[If applicable: cross-app analysis]

---

## Prioritized Recommendations

### Quick Wins (This Week)
1. [recommendation with expected impact]

### Strategic (This Month)
1. [recommendation with expected impact]

### Long-Term (This Quarter)
1. [recommendation with expected impact]

---

## Next Steps
1. [Most critical action]
2. [Second priority]
3. [Third priority]
```

---

## Terminal Output

```
=== ASO AUDIT COMPLETE ===

App: [name]
Marketplace: [marketplace]
ASO Score: [X]/100

Listing Quality:
  Title & Subtitle:    [X]/10
  Description:         [X]/10
  Visual Assets:       [X]/10
  Positioning:         [X]/10

Conversion Factors:
  Clarity:    [X]/10
  Relevance:  [X]/10
  Trust:      [X]/10
  Simplicity: [X]/10

Reviews: [X]/5 ([X] reviews)
Competitors Analyzed: [X]

Top 3 Fixes:
  1. [fix]
  2. [fix]
  3. [fix]

Full report saved to: ASO-AUDIT.md
```

---

## Cross-Skill Integration

- If `SEO-AUDIT.md` exists, analyze the SEO-to-ASO bridge with real data
- If `COMPETITOR-REPORT.md` exists, incorporate marketplace competitor intelligence
- If `BRAND-VOICE.md` exists, evaluate listing copy against brand guidelines
- If `COPY-SUGGESTIONS.md` exists, apply copy improvements to listing description
- Suggest follow-up: `/market seo` for web content supporting ASO, `/market competitors` for broader competitive analysis, `/market copy` for listing copy optimization

## Key Principles

- ASO is about conversion, not just keywords. A listing that ranks but does not convert is failing.
- Every recommendation must be specific and actionable. "Improve your description" is useless. Show the before and after.
- Marketplace-specific: adapt scoring and recommendations to the specific marketplace's ranking factors and conventions.
- If brand-specific ASO rules exist in the project (e.g., under `brands/<brand>/shared/aso-rules.md`), incorporate them into the analysis.
- For multi-app publishers, always consider portfolio-level strategy, not just individual listing optimization.
