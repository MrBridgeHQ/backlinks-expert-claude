# Property Profiles - Per-Property Link-Building Posture

A backlink campaign is only as good as the property it serves. The same tactic that's fine for a tool page on a third-party platform can quietly endanger a retail business that pays the rent. This file is the per-property rulebook: niche, market, audience, **risk posture**, the canonical funnel URL (anchors must point at these, not at arbitrary deep pages), a seed anchor-text mix, and a do/don't list.

Read the profile **before** you discover targets, plan a campaign, or generate an asset. The posture decides everything downstream - which tier ratio is acceptable, how aggressive the anchor mix can be, and which channels are off-limits.

The principle: **money sites are protected by default; product/tool pages can absorb more tier-2.** A Google manual action on an e-commerce site costs real revenue. A nofollow forum link to a tool page that ages out costs nothing. Calibrate the risk you take to the cost of being wrong.

The profiles below are **illustrative templates**, not a fixed registry. Use them to classify whatever property you are working on, then fill in the real niche, market, and funnel URL for that property. Placeholder domains like `example.com` and `yourbrand.com` stand in for the real ones.

---

## How to read a posture

| Posture | Means | Tier mix | Anchor stance |
|---|---|---|---|
| **MONEY → conservative/editorial** | Real business, real revenue. Penalty = lost income. | Tier-1 editorial almost exclusively; tier-2 only on clearly genuine, high-traffic, on-niche communities, in tiny volume. | Branded + naked URL dominate. Exact-match anchors essentially never. |
| **hybrid** | Brand + lead-gen site; some revenue, more tolerance than a pure money site. | Tier-1 led, tier-2 in moderation where relevant. | Branded + naked dominant; descriptive phrase occasional; exact-match rare. |
| **tool (more tier-2 OK)** | A product page on a platform you don't own. Discovery and referral traffic matter more than equity; the page can't be "penalized" the way a domain can. | Tier-1 where you can earn it; tier-2 (dev/SEO communities, profiles, dev directories) is acceptable in larger share. | Branded + naked dominant; descriptive ("MCP server for X") fine; exact-match still kept rare. |

Anchor mixes below are **seeds** - starting distributions, not quotas. The campaign planner re-balances against the property's existing anchor profile (you never want to pour exact-match onto a site that already over-indexes on it). Every distribution keeps **branded + naked URL dominant and exact-match rare** - that's the non-negotiable spine, lifted straight from Google's own anchor guidance (descriptive, concise, relevant; avoid keyword-stuffed anchors).

> **Two rules that apply to every profile below, no exceptions:**
> 1. Every link to a product/tool page on a third-party platform carries **your tracking/referral param** where one applies. No bare links that forfeit attribution.
> 2. Every asset's prose runs through a **prose-humanization** pass before it's posted or sent. This file does not restate that doctrine - the humanization skill owns it. Just route to it.

---

## Template A - Product / tool pages on a third-party platform

| Field | Value |
|---|---|
| **Property type** | Product pages on a third-party platform (a marketplace / app store) |
| **Niche** | Whatever the tool does - e.g. dev tooling, scrapers, MCP servers, AI agents |
| **Market / language** | Typically EN - a global developer / technical audience |
| **Audience** | Developers, data engineers, SEO/growth people, automation builders, no-code/low-code users evaluating the tool |
| **Risk posture** | **tool - more tier-2 OK.** A marketplace listing isn't a domain you own; the upside is discovery + qualified referral traffic, not link equity to a site you control. You can run a more aggressive tier-2 share here than on owned domains. |
| **Funnel URL** | `https://platform.example.com/<your-account>/<slug>` (always with your tracking/referral param where one applies) |

**Seed anchor-text mix** (per product/tool page):

| Anchor type | Share | Examples |
|---|---|---|
| Branded | ~35% | "the [Brand] scraper", "the [Brand] MCP server" |
| Naked URL | ~30% | the funnel URL |
| Generic / contextual | ~20% | "this tool", "an Actor that does X", "here" (used sparingly, in genuine context) |
| Descriptive / partial | ~12% | "an MCP server for web scraping", "a price scraper" |
| Exact-match | ~3% | "price scraper" - only when it reads naturally |

**Do**
- Lead with dev/SEO/infra communities and Q&A where the tool is a genuine answer: SitePoint, DigitalOcean Community, webhostingtalk, dev.to (publish, don't drop), Stack-family (nofollow but topical traffic), SEO forums.
- Use GitHub profile/README and dev directories - high relevance, accepted contributor-link placements.
- Treat any single marketplace/directory listing channel as its own playbook - **delegate to a directory/marketplace-distribution skill**; don't reinvent its listing mechanics here.
- Favor "I built a tool that solves X" posts with a working demo over bare link drops.

**Don't**
- Don't drop the tool link in forum signatures across dozens of off-niche forums - that's the exact "forum signature spam" Google names as link spam, and it gets the *host* penalized (so the link dies anyway).
- Don't omit your tracking/referral param - a clean link forfeits attribution.
- Don't claim the tool does something it doesn't to win a placement.

---

## Template B - Owned brand / lead-gen hub (hybrid)

| Field | Value |
|---|---|
| **Property type** | Owned domain (your own site) |
| **Niche** | A brand/lead-gen hub - e.g. a portfolio site bridging a technical product line and a content/BI offering |
| **Market / language** | EN primary, optionally **multilingual** - EN / FR / ES / PT / DE / AR / HI |
| **Audience** | The buyers for each side of the business, plus the multilingual long tail those locales open up |
| **Risk posture** | **hybrid.** It's an owned domain, so a penalty *does* hurt - more caution than third-party tool pages. But it's a brand/lead-gen hub, not a checkout-driven money site, so it tolerates more tier-2 than a transacting business. Tier-1 editorial leads; tier-2 used in moderation, on-niche. |
| **Funnel URL** | `https://yourbrand.com/*` - point anchors at the most relevant page (e.g. `/solutions/*`, `/scrapers`, `/studies`, `/articles`). Treat your important landing pages as **intentional SEO targets**; preserve them. |

**Seed anchor-text mix:**

| Anchor type | Share | Examples |
|---|---|---|
| Branded | ~40% | "[Brand]", "yourbrand.com", "the [Brand] studies" |
| Naked URL | ~25% | `yourbrand.com`, `yourbrand.com/studies` |
| Descriptive / partial | ~20% | "their guide to scraping pricing data", "an MCP workflow walkthrough" |
| Generic / contextual | ~12% | "this analysis", "their writeup" |
| Exact-match | ~3% | rare; only when the target page's topic genuinely is the anchor |

**Do**
- Use the bilingual/multilingual reach: an EN dev post can link a dev landing page; an FR post can link an FR-localized page. Match link language to landing-page language.
- Pitch guest posts and digital-PR (HARO/Connectively) on the strength of original research the site already hosts - earned links to genuinely link-worthy content is the cleanest play.
- Reclaim unlinked brand mentions (Google Alerts → ask for the link).
- Use the hub as the **link target for a product-ecosystem story** (e.g. an article that contextualizes several tools), keeping the tracked product links inside that content.

**Don't**
- Don't run niche-A anchors on niche-B communities (e.g. BI anchors on dev forums or dev anchors on a consumer forum) - relevance gates value; off-niche links pass little and look manufactured.
- Don't strip or shorten intentional landing-page link blocks when reusing content - these are deliberate SEO targets; move them if needed, but treat removal as a decision, not a cleanup default.

---

## Template C - Owned money site, retail / e-commerce

| Field | Value |
|---|---|
| **Property type** | Owned domain - **a real business (money site)** |
| **Niche** | A revenue-bearing vertical - e.g. e-commerce, market-intelligence services, a transacting storefront |
| **Market / language** | Whatever the business sells into (a single market, or international + a specific local market) |
| **Audience** | The business's actual customers and trade buyers |
| **Risk posture** | **MONEY → conservative / editorial.** This earns revenue; a manual action or algorithmic suppression costs real money. **Tier-1 editorial almost exclusively.** Tier-2 only on unmistakably genuine, active, high-traffic, on-niche communities, and in tiny volume. No foundational-link volume plays. |
| **Funnel URL** | `https://example.com` (own site; relevant deep pages where they exist) |

**Seed anchor-text mix** (deliberately tame):

| Anchor type | Share | Examples |
|---|---|---|
| Branded | ~50% | "[Brand]", "example.com", "the [Brand] team" |
| Naked URL | ~28% | `example.com` |
| Generic / contextual | ~15% | "their market report", "this buyer's guide" |
| Descriptive / partial | ~5% | "their import service" |
| Exact-match | ~2% | almost never; only in genuinely editorial context |

**Do**
- Earn links: digital PR (trade press, journalist outreach via Connectively/HARO), original market-data pieces (proprietary or derived insight makes genuinely citable content), guest articles on reputable vertical publications, supplier/partner pages, trade-association directories, podcast appearances.
- For a specific local market: in-language trade media, association listings, in-language guest content. Match anchor language to the page.
- Use adjacent enthusiast/trade communities **only** for genuine participation that yields referral traffic and brand visibility - treat any link there as traffic/brand, not equity.

**Don't**
- Don't buy followed links, don't use crowd-marketing/link-marketplace platforms for followed links, don't touch PBNs or expired-domain schemes - the penalty risk to a revenue site is unacceptable.
- Don't run exact-match commercial anchors ("buy [product] online" etc.) - over-optimization on a money site is the fastest route to a manual action.
- Don't run bulk forum/profile/directory submissions. A handful of relevant, real links beats hundreds of low-value ones, and the volume play is what gets money sites hurt.

---

## Worked variant - a money site in a non-English market (FR example)

The same MONEY posture, localized. For a French e-commerce money site:

- **Anchor mix** stays deliberately tame: branded ~50%, naked URL ~28%, generic/contextual ~15% ("leur boutique", "ce caviste en ligne", "leur sélection"), descriptive ~5%, exact-match ~2% (quasi-jamais ; uniquement en contexte éditorial réel).
- **Do:** privilégier le earned link FR - relations presse / blogs spécialisés FR, articles invités sur des sites reconnus, annuaires légitimes du secteur, partenariats fournisseurs, opérations "top 10 / sélection" (écrire un roundup citant des acteurs, puis leur demander le lien). Communautés FR pertinentes **uniquement** pour participation sincère → trafic référent et notoriété, pas équité de lien. Disclosure quand un placement est sponsorisé/payé (mention claire + `rel="sponsored"`).
- **Don't:** pas d'achat de liens suivis sur des plateformes de netlinking pour des liens *dofollow* - risque de pénalité inacceptable pour un site marchand (si lien payé, alors `rel="sponsored"`/`nofollow` + divulgation) ; pas d'ancres exact-match commerciales ; pas de soumissions de masse (forums/profils/annuaires) ni de PBN/domaines expirés.

The doctrine is identical to Template C; only the language of the anchors, the targets, and the disclosure label changes.

---

## Extensibility - adding a new property

This file is a set of templates, not a closed set. **New property = add a profile**, same shape as above (pick the closest template, then fill the real fields).

To add a profile, fill every field:

1. **Property type** - owned domain vs. third-party product page (decides whether "penalty" even applies).
2. **Niche** - used to gate relevance during discovery/qualification.
3. **Market / language** - decides which target lists and which asset-template language to use.
4. **Audience** - sanity-checks whether a target's readers are actual prospects.
5. **Risk posture** - MONEY / hybrid / tool. This is the load-bearing field; everything downstream keys off it.
6. **Funnel URL** - the canonical destination. Product/tool URLs **must** carry your tracking/referral param where one applies.
7. **Seed anchor mix** - branded + naked dominant, exact-match rare, calibrated to posture.
8. **Do / Don't** - the property-specific guardrails.

When in doubt about posture: if the property earns money directly, treat it as MONEY until proven otherwise. It's cheaper to be conservative on a property that could have tolerated more than to be aggressive on one that couldn't.
