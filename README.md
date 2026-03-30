# ai-marketing-system

Claude Code marketing automation workspace for Mageplaza and Shopplaza teams.

## What This Does
Automates marketing tasks across all channels — SEO, email, social media, 
ads, competitor research, landing page optimization, and reporting.

## Brands
- **Mageplaza** — Magento 2 extensions & services (mageplaza.com)
- **Shopplaza** — Shopify apps (shopplaza.io)
- **Mageplaza Vietnam** — Vietnamese market (mageplaza.com/vi/)

## Folder Structure
- `.claude/` — Brand context files (Claude reads these automatically)
- `reports/` — Audit and performance reports
- `emails/` — Generated email sequences
- `social/` — Social media content calendars
- `blog/` — SEO blog drafts
- `ads/` — Ad copy variations

## How To Use
1. Open this folder in VS Code
2. Open the terminal and type `claude`
3. Run commands like `/market audit https://www.mageplaza.com`

## Key Commands
| Command | What it does |
|---|---|
| `/market audit <url>` | Full marketing audit |
| `/market seo <url>` | SEO analysis |
| `/market emails <topic>` | Generate email sequence |
| `/market social <topic>` | 30-day social calendar |
| `/market copy <url>` | Rewrite page copy |
| `/market competitors <url>` | Competitor research |
| `/market report-pdf <url>` | Generate PDF report |