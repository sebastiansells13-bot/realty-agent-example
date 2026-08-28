# realty-agent-example

A live, deployed example of a real-estate agent site built from
[client-site-starter](https://github.com/sebastiansells13-bot/client-site-starter),
demonstrating the template applied to a different business type — listings, agent
bio, testimonials, and market-update posts instead of a menu/services page.

**Live site:** https://sebastiansells13-bot.github.io/realty-agent-example/

## ⚠️ This is a pitch mockup, not a real agent's site

All identifying details — agent name, brokerage office, city, phone, email, license
number, and every listing address and testimonial — are **placeholders** (shown in
`[brackets]` in the source data), not a real person or real property. This exists to
demonstrate the site to a prospective real-estate client before real details are
supplied.

**No actual CENTURY 21 trademarked logo or official brand assets are used.** The site
references "CENTURY 21" by name (accurate, truthful text describing an actual
franchise affiliation, standard practice for real agent sites) and uses a black/gold
color palette evoking the brand's signature look — but the literal logo graphic is a
registered trademark this project has no license to reproduce. If this becomes a real
engagement with an actual CENTURY 21-affiliated agent, replace:

- Every `[bracketed placeholder]` in `src/_data/business.json`, `listings.json`, and
  `testimonials.json` with the real agent's real details
- The color palette in `src/_includes/css/variables.scss` with the agent's actual
  official brand assets, if/when they provide them
- `business.photo` in `src/_data/business.json` — currently empty; add the real
  agent's own photo, not a stock placeholder

See [CREDITS.md](CREDITS.md) for photo sourcing, including photos deliberately
rejected during sourcing and why.

## What's different from the template

- New `listings` content type (`src/_data/listings.json`, `src/listings.njk`) —
  property cards with price, beds/baths/sqft, and status badge
- New `testimonials` content type, shown on the homepage
- "Services" repurposed as "How I Can Help" (`src/how-i-help.njk`) — buying, selling,
  market analysis instead of a generic service list
- "Team" removed — solo agent bio lives directly in `business.json` and renders on
  `src/about.njk`
- Blog posts retagged for real estate (`market-update`, `seller-tips`, etc.)
- `pathPrefix` and sitemap/feed hostnames point at
  `sebastiansells13-bot.github.io/realty-agent-example` — needed only because this
  demo lives at a GitHub Pages *project* URL rather than a custom domain

## Local development

```bash
npm install
npm start
```
