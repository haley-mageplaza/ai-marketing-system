# Shopplaza Brand Knowledge

Shopplaza is a Shopify app publisher operating across three product lines.

## Product Lines

| Product Line | Status | Focus |
|---|---|---|
| **B2B** | Active (primary marketing focus) | Wholesale, pricing control, B2B operations |
| **B2C** | Active (managed by separate team) | Retail conversion, UX, engagement |
| **Checkout** | Pre-launch | [Details pending launch] |

## Directory Structure

```
shopplaza/
├── brand/          Brand-level identity, positioning, audience, tone
├── shared/         Cross-product-line rules (SEO, ASO, content)
├── b2b/            B2B product line context, strategy, and per-app knowledge
├── b2c/            B2C product line context and per-app knowledge
└── checkout/       Checkout product line (PRE-LAUNCH)
```

## Context Loading

Load context selectively based on the task:

- **B2B task** → `brand/` + `shared/` + `b2b/` + relevant `b2b/apps/<app>.md`
- **B2C task** → `brand/` + `shared/` + `b2c/` + relevant `b2c/apps/<app>.md`
- **Checkout task** → `brand/` + `shared/` + `checkout/`
- **Brand-wide task** → `brand/` + `shared/`

Do not load the entire knowledge tree for every task.
