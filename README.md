# Lattelis Editions

**Publishing & Discovery**

Lattelis Editions is an independent public-facing discovery platform for publications, research, guides, articles, media, tools, projects, and curated collections.

Target public URL: `https://lattelis-editions.pages.dev/`

Contact: `lattelis.hub@gmail.com`

## Role

Lattelis is not a publisher profile page and does not claim ownership of the independent projects it indexes. Its public role is:

`Discovery -> Catalog -> Asset Detail -> Project / Creator -> Official Destination`

The official destination remains the source of truth for current price, availability, checkout, download, or project status.

## Catalog rules

- Search covers title, topic, project, creator, category, format, language, and keyword.
- Categories are Editions, Research, Guides, Articles, Visual, Video, Music, Tools, Projects, and Collections.
- Empty categories remain honest empty states; do not invent assets to make the catalog look larger.
- A `Paid` label is allowed only when the external destination is known to be a paid asset.
- Show a numeric price only when it is verified from a current source of truth.
- Never invent a Buy button or checkout URL.
- Related assets are discovery suggestions, not ownership claims.
- Lattelis is independent from Digital Index Base and from the projects it indexes.

## Revenue priority

`Payment > Checkout > Qualified Action > Qualified Visit > Discovery > Page View`

The platform should optimize discovery and routing without pressuring every asset into a sale.

## Analytics contract

The frontend emits lightweight custom browser events without requiring a third-party key:

- `lattelis:search`
- `lattelis:filter`
- `lattelis:collection_open`
- `lattelis:category_open`
- `lattelis:asset_view`
- `lattelis:official_destination_click`
- `lattelis:paid_destination_click`

A future analytics layer may subscribe to these events without rewriting catalog behavior.

## Deployment state

The source is prepared for `https://lattelis-editions.pages.dev/`. A GitHub Pages fallback workflow was tested, but the connected GitHub App cannot enable the repository Pages setting (`Resource not accessible by integration`). Do not treat the GitHub Pages fallback as live until an authorized user enables it.

The preferred production destination remains the reserved Cloudflare Pages URL above.
