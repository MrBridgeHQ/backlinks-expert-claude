# Campaign Planning - The Strategist

Discovery finds opportunities and qualification vets them. This page is what sits between "here is a pile of vetted targets" and "here is what we actually do, in what order, at what pace, and how we know it worked." A link-building campaign is not a list of links - it is a plan with a goal, a budget, a velocity, a tier ratio, and a measurement loop.

The whole plan is governed by one inversion of the usual instinct: **the property dictates the posture, not the other way around.** A money site and a tool page can chase the same keyword and still need almost opposite link mixes. Plan per property.

This is strategy, not legality. The boundary discipline - what we will and won't build, Google's link-spam policy, disclosure, money-site protection - lives in `ethics-risk.md`. Read that page first if you haven't; everything here assumes it.

---

## Step 0 - Name the goal before touching tactics

A campaign without a measurable goal becomes a link-count race, which is the failure mode this entire skill exists to prevent. Pin down four things first:

1. **The property and its URL(s).** Which page(s) actually need to rank or get discovered? A backlink campaign that points at the wrong page wastes every link.
2. **The posture** (from `property-profiles.md`): money site (conservative, tier-1-heavy) or tool/product page (more tier-2 tolerated). This single decision drives the tier ratio, the anchor mix, and the risk budget.
3. **The objective**, stated as a movement, not a vanity number:
   - *Ranking* - move target keyword(s) from page 3 to page 1. Needs editorial, relevant, equity-passing links.
   - *Discovery / indexation* - get a new domain crawled and indexed. Needs links on already-indexed, frequently-crawled pages; nofollow is acceptable here because the job is crawl-path discovery, not equity.
   - *Referral traffic / brand* - get qualified humans to the property. Forum/Q&A/community links do this well even when nofollow.
   - These need different tactics. Confusing "I want rankings" with "I want traffic" produces a plan that delivers neither.
4. **The budget**, in money and in hours. Editorial link-building is time-expensive, not cash-expensive. Be honest about which you actually have.

Write these four down. The rest of the plan is derived from them.

---

## The tier model (recap, for ratios)

Full catalog and risk labels are in `tactics-tiers.md`. For planning, three buckets:

- **Tier-1 (editorial / earned)** - guest posts on relevant sites, niche edits / link insertions into existing relevant articles, digital PR (HARO/Connectively), original-research link-bait, free micro-tools hosted on your own domain, resource-page links, broken-link building, podcast appearances, reclaimed brand mentions. These are the only links that reliably pass ranking credit. They are slow and effortful. **Equity plays.**
- **Tier-2 (foundational, risk-labeled)** - genuine forum participation, profile links, niche directory entries, Q&A answers (Reddit/Quora/StackExchange). Mostly nofollow/UGC in 2026. Per `ethics-risk.md`, their value is **referral traffic + brand + link-profile diversity**, *not* ranking equity. Used in moderation, real participation only - never bulk. **Traffic/brand/discovery plays.**
- **Out of scope** - PBNs, undisclosed paid followed links, mass automated forum/profile/directory spam, reciprocal-link schemes, expired-domain abuse. See the "WHAT WE WON'T DO" list in `ethics-risk.md`. These are never in a plan.

---

## Step 1 - Set the tier ratio from the posture

The ratio is the heart of differentiated planning. It is a target distribution of *referring domains acquired in the campaign window*, not a hard quota.

| Posture | Tier-1 (editorial/earned) | Tier-2 (foundational, risk-labeled) | Rationale |
|---|---|---|---|
| **Money site** (revenue-bearing business) | **~80–90%** | ~10–20% | A real business with revenue and reputation cannot afford a manual action. Tier-1 editorial links are both the safest and the only equity-passing kind. The small tier-2 slice is for genuine community presence and traffic, not ranking. |
| **Tool / product page** (third-party platform, dev-facing pages) | ~50–65% | **~35–50%** | A developer-audience tool page lives natively in dev/SEO/webmaster communities. Forum, GitHub-profile, dev-community, and Q&A links here are *on-topic participation*, drive real qualified traffic, and the page is lower-stakes than a revenue site. More tier-2 is defensible. Still never bulk/automated. |

Two non-negotiables regardless of posture:
- **No tier of links is ever bulk or automated.** "More tier-2 allowed" for a tool page means more *hand-built, real-participation* tier-2, not a submission run.
- **Relevance gates everything.** An off-niche tier-1 link is worth less than an on-niche tier-2 one. A money site does not chase dev-forum links to pad its tier-2; it finds its own vertical's communities (see `property-profiles.md`).

---

## Step 2 - Set the anchor-text mix

Anchor distribution is the single most common over-optimization tripwire. Google's own guidance (`developers.google.com/.../links-crawlable`): good anchors are **descriptive, concise, relevant**; avoid keyword-stuffed or over-long anchors (named as a spam signal); avoid bare "click here." A natural backlink profile is dominated by branded and URL anchors, with exact-match commercial anchors *rare*.

Target distribution (across all earned/placed links in the campaign):

| Anchor type | Example (a wine e-commerce money site) | Target share | Notes |
|---|---|---|---|
| **Branded** | "[Brand]" | ~35–45% | The natural default. A real editor citing you uses your name. |
| **Naked URL** | "example.com" | ~15–25% | Common in forum/directory/citation contexts. |
| **Generic / contextual** | "this French natural-wine shop", "see their selection here" | ~15–25% | Reads human; what real writers actually do. |
| **Partial / topical** | "natural wine from the Loire" | ~10–20% | Descriptive, relevant - Google's preferred kind. |
| **Exact-match commercial** | "acheter vin nature en ligne" | **<5–10%** | Rare on purpose. A spike of exact-match anchors is the classic algorithmic-penalty pattern. The more money-site the property, the lower this goes. |

For a tool/product page the same shape holds; branded = the tool/brand name (e.g. "[Brand] Price Scraper"), partial = "price scraper", exact-match = "price scraper API" kept rare. **You do not control anchors on editorial links you earn** - that's fine and natural; you steer anchors only where you author the text (guest posts, your own profiles, directory entries), and even there you keep the mix natural rather than stuffing.

Product/tool URLs carry your tracking/referral param where one applies (a store/product-content convention; restated here because plans place those links).

---

## Step 3 - Set velocity and pacing

Link velocity = referring domains acquired per unit time. The rule is **natural, steady, no spikes.** There is no official "safe number" from Google - this is a risk heuristic, not a published rule - but a sudden burst of links to a page that has never attracted links before is exactly the pattern algorithmic spam systems and manual reviewers look for.

Principles:
- **Steady beats bursty.** A handful of quality referring domains per month, sustained, beats fifty in week one and zero after. Model the velocity on what a genuinely growing site of that size would naturally attract.
- **Match velocity to the property's baseline.** A brand-new domain with zero links that suddenly gains 30 in a month looks engineered. An established site can absorb more. Ramp up, don't spike.
- **Earned links arrive on their own clock.** Digital PR can deliver several links in a day when a story lands - that's natural and fine, because it's genuinely earned and the pattern (many outlets citing one story) is recognizably editorial. Engineered placements should not mimic that burst shape without the underlying story.
- **Tier-2 cadence is participation-paced.** Earn trust in a community first (5–10 genuine, link-free contributions), then ~one contextual link per useful reply, roughly weekly. ~5–15 quality forum links/month across a community footprint, not hundreds.
- **Front-load nothing on a money site.** For revenue-bearing properties, deliberately slow. Reputation is the asset being protected.

A practical pacing default: express the plan as "referring domains/month" per tier, ramping gently, with the money-site number visibly lower than the tool-page number.

---

## Step 4 - Sequence the work

Order matters because some tactics seed others.

1. **Foundation & relevance signals first (light).** A few genuine community profiles and one or two relevant niche directories establish a baseline, diversify the profile, and create indexed pages that link to you (aids discovery). Keep it small - this is not the campaign, it's the warm-up. Money sites: minimal.
2. **Create the link-worthy asset.** Before outreach, there must be something worth linking to: original research, a data study, a free tool, a genuinely useful guide hosted on your own domain. This is the engine for all of tier-1. (Prose for these assets routes through a prose-humanization pass.)
3. **Outreach & editorial placement (the core).** Guest posts, niche edits, resource-page and broken-link outreach, digital PR/HARO around the asset. This is where the ranking equity comes from; it runs continuously and is the largest time investment.
4. **Community participation in parallel (tier-2).** Forums and Q&A run alongside, paced by genuine participation, not by quota. Tool pages do more of this; money sites do a little.
5. **Reclaim & compound.** Set Google Alerts for brand mentions; convert unlinked mentions to links. Repurpose the asset (podcast appearances, a roundup post that names sites you then notify). This compounds with no new asset cost.

Sequencing the asset (step 2) before outreach (step 3) is the most common thing teams get backwards - they pitch guest posts with nothing distinctive to offer, get low response, and drift toward buying links. Build the asset first.

---

## Step 5 - KPIs and tracking

Measure outcomes, not activity. The metrics below are the scoreboard; the deprioritized list after it is what we deliberately ignore.

**Primary KPIs (the ones that matter):**

| KPI | What it tells you | How to track (free-first) |
|---|---|---|
| **Referring domains** (unique linking domains, not total links) | Profile growth. One new domain >> ten new links from a domain you already had. | GSC Links report (free); Ahrefs/Semrush if available. Count *domains*. |
| **Anchor-text distribution** | Whether you're drifting toward over-optimization. Watch exact-match share creeping up. | GSC top linking text; backlink tool anchor report. Compare to the Step-2 target mix. |
| **Indexation of placed links** | A link Google hasn't crawled/indexed passes nothing. Confirms the placement page is actually crawlable and indexed. | `site:` / URL inspection on the *placement page*; confirm it's a real `<a href>` (JS/`span`/`javascript:` links don't count). |
| **Organic ranking movement for target keywords** | The actual objective for ranking campaigns. The point of equity links. | GSC Performance (position for tracked queries); a rank tracker. Segment by the page the campaign targets. |
| **Cost-per-referring-domain** | Efficiency, and whether the mix is sane. Includes *hours* for editorial, not just cash. | Spend (cash + valued hours) ÷ net new relevant referring domains, per tactic. Lets you kill low-yield tactics. |

For a **discovery/indexation** objective (new domain), the headline KPI is "is the domain getting crawled and indexed" (GSC coverage, crawl stats), and referral-traffic from tier-2 placements - *not* ranking movement, which comes later.

**DEPRIORITIZED - vanity metrics we explicitly do not optimize for:**
- **Raw total link count.** Ten links from one domain is one referring domain. Counting links rewards exactly the bulk behavior we refuse.
- **DA / DR as a goal.** DA (Moz) and DR (Ahrefs) are **third-party metrics, not Google signals.** They're a rough triage heuristic at best (and the source listicles recycle stale, self-contradictory DA numbers - same site shown as DA 55 and 59 on one page). Chasing high DR on irrelevant sites buys nothing. Relevance first.
- **"DoFollow link count" as a trophy.** A dofollow link on a dead, noindex, off-niche page is worth less than a nofollow link on a live, indexed, on-topic, high-traffic page that sends real readers.
- **Sheer number of forums/directories submitted to.** This is the metric the spam lists optimize. It's an anti-goal.

Track the primary KPIs monthly; review the anchor distribution and velocity every cycle to catch drift before it becomes a pattern.

---

## Worked example A - a wine e-commerce money site (FR)

**Goal (Step 0):** move the homepage + the "vin nature Loire" category page from page 2–3 to page 1 for mid-tail French natural-wine queries. **Posture: money site → conservative, tier-1-heavy.** Budget: modest cash, steady founder hours. Objective: *ranking* (with referral traffic welcome).

**Tier ratio (Step 1):** ~85% tier-1 / ~15% tier-2. The business has revenue and a reputation; a manual action is unacceptable. Tier-2 is for genuine French wine-community presence and traffic, not ranking.

**Anchor mix (Step 2):** Branded ~40%, naked URL ~20%, generic/contextual ~20%, partial/topical ("vin nature de Loire", "cave en ligne nature") ~15%, exact-match commercial ("acheter vin nature") **<5%** - deliberately near-zero on a money site.

**Tactic mix:**
- *Tier-1:* a genuinely useful FR asset (e.g. an original "carte des vignerons nature de Loire" or a tasting/region guide) hosted on the site → outreach to FR wine bloggers, natural-wine media, sommelier sites for editorial mentions and niche edits. A clean roundup play (write a roundup naming domaines/cavistes, then notify them) fits FR norms. Partner/supplier links from the domaines and importers stocked. A podcast or interview in the FR wine scene.
- *Tier-2 (small):* one or two genuine, paced contributions in FR wine/food communities and a relevant FR food/wine directory - for traffic and a little profile diversity. Real participation, ~monthly, never a submission run.

**Velocity (Step 3):** deliberately slow and steady - a few relevant referring domains per month, ramped gently. No bursts. Reputation > speed.

**KPIs (Step 5):** referring *domains* from FR wine/food sites; ranking movement for the target FR queries in GSC; anchor distribution staying branded-dominant with exact-match near zero; referral traffic from the community placements. Ignored: total link count, DR of any non-wine site.

---

## Worked example B - a developer-tool product page (third-party platform, EN)

**Goal (Step 0):** rank the tool's listing/landing page for "price scraper" / "price-monitoring scraper / API" and drive qualified developer traffic + installs. **Posture: tool page → more tier-2 tolerated.** Objective: mix of *ranking* and *referral traffic/discovery*. Budget: founder hours, low cash.

**Tier ratio (Step 1):** ~55% tier-1 / ~45% tier-2. The audience is developers who genuinely live in dev/SEO/webmaster communities, so on-topic community links are native, high-traffic, and defensible. Still hand-built only.

**Anchor mix (Step 2):** branded "[Brand] Price Scraper" / "[Brand]" ~40%, naked URL (the funnel URL) ~20%, generic/contextual ~20%, partial ("price scraper", "price-data tool") ~15%, exact-match ("price scraper API") rare. Product/tool links carry your tracking/referral param where one applies.

**Tactic mix:**
- *Tier-1:* a technical asset on your own domain (e.g. "how wine pricing data flows across sources", or a free micro-tool) → guest posts / dev.to articles / niche edits on scraping, data-engineering, and SEO blogs; HARO/Connectively for data-journalism quotes; a GitHub repo/README that legitimately references the tool.
- *Tier-2 (larger, still genuine):* real participation in dev/SEO/webmaster communities surfaced in `target-database.md` (e.g. SitePoint, DigitalOcean community, webmaster/SEO forums, relevant StackExchange/Reddit answers) - earn-trust-first, one contextual link per genuinely useful answer. These are mostly nofollow → counted as **traffic/brand/discovery**, not equity, in the plan.

**Velocity (Step 3):** can ramp a little faster than the money site (lower stakes), still steady - model it on a tool that's organically gaining adoption. Community participation paced weekly.

**KPIs (Step 5):** referring domains from dev/SEO sites; tool page ranking for the target queries; *referral traffic and installs* attributable to placements (the tool-page objective leans more on traffic than the money site does); indexation of placed links; cost-per-referring-domain (mostly hours). Ignored: number of forums posted to, DR of unrelated high-authority sites.

---

## The one-paragraph campaign brief (output format)

When asked to plan, produce this for each property:

> **Property / URL:** … (product/tool URLs carry the tracking/referral param) · **Posture:** money / tool · **Objective:** ranking / discovery / traffic · **Tier ratio:** X% tier-1 / Y% tier-2 · **Anchor mix:** branded/URL-dominant, exact-match <N% · **Velocity:** ~N referring domains/month, ramped, no spikes · **Sequence:** foundation → asset → outreach (+ community in parallel) → reclaim · **KPIs:** referring domains, anchor distribution, indexation, ranking movement, cost-per-referring-domain · **Deprioritized:** raw link count, DA/DR of irrelevant links.

Then the tactic list, each tactic tagged with its tier and (for tier-2) its risk label from `tactics-tiers.md`, and each asset's prose routed through a prose-humanization pass.
