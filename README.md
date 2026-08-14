# ai-marketing-system

Claude Code marketing automation workspace for Mageplaza and Shopplaza teams.

## What This Does

Automates marketing tasks across all channels — SEO, ASO, email, social media, ads, competitor research, landing page optimization, funnel analysis, and reporting.

## Architecture

```
.claude/skills/    Reusable marketing capabilities (generic, brand-agnostic)
brands/            Brand, product-line, and product knowledge (source of truth)
workflows/         Orchestration of skills + relevant context for recurring use cases
outputs/           Generated working outputs, organized by brand
```

## Brands

| Brand | Focus | Directory |
|---|---|---|
| **Mageplaza** | Magento 2 extensions & services | `brands/mageplaza/` |
| **Mageplaza Vietnam** | Vietnamese market | `brands/mageplaza-vietnam/` |
| **Shopplaza** | Shopify apps (B2B, B2C, Checkout) | `brands/shopplaza/` |

## How To Use

1. Open this folder in VS Code or your terminal
2. Run `claude`
3. Run commands like `/market audit https://www.mageplaza.com`

## Key Commands

| Command | What it does |
|---|---|
| `/market audit <url>` | Full marketing audit |
| `/market seo <url>` | SEO content audit |
| `/market aso <url>` | App store / marketplace listing optimization |
| `/market funnel <url>` | Sales funnel analysis |
| `/market landing <url>` | Landing page CRO analysis |
| `/market competitors <url>` | Competitive intelligence |
| `/market copy <url>` | Copywriting analysis and generation |
| `/market emails <topic>` | Email sequence generation |
| `/market social <topic>` | 30-day social content calendar |
| `/market ads <url>` | Ad creative and copy generation |
| `/market launch <product>` | Product/feature launch playbook |
| `/market brand <url>` | Brand voice analysis |
| `/market proposal <client>` | Client proposal generation |
| `/market report <url>` | Marketing report (Markdown) |
| `/market report-pdf <url>` | Marketing report (PDF) |

## Folder Structure

```
ai-marketing-system/
├── .claude/skills/         Marketing skill definitions
│   ├── market/             Main orchestrator
│   ├── market-aso/         App Store / Marketplace Optimization
│   ├── market-audit/       Full marketing audit
│   ├── market-seo/         SEO content audit
│   └── ...                 (15 more skills)
│
├── brands/
│   ├── mageplaza/          Magento extensions & services context
│   ├── mageplaza-vietnam/  Vietnamese market context
│   └── shopplaza/          Shopify apps context
│       ├── brand/          Brand identity, positioning, audience, tone
│       ├── shared/         Cross-product-line rules (SEO, ASO, content)
│       ├── b2b/            B2B product line + per-app knowledge
│       ├── b2c/            B2C product line + per-app knowledge
│       └── checkout/       Checkout product line (pre-launch)
│
├── workflows/
│   └── shopplaza/          Shopplaza-specific marketing workflows
│
└── outputs/                Generated marketing outputs
```
