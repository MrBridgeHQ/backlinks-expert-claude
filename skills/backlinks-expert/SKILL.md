---
name: backlinks-expert
description: Use when you need to build or acquire backlinks, plan off-page SEO / link building, or promote a property's authority — discovering and qualifying link opportunities, designing a link campaign (tactic mix, anchor text, velocity, tier ratios), or generating submission/outreach assets (guest-post pitches, niche edits, forum/profile/directory entries, Q&A answers, digital-PR). Triggers on "build backlinks", "link building", "off-page SEO", "promote my site / tool / product page", "dofollow forums", "guest posts", "niche edits", "anchor text strategy", "vet DR/DA / dofollow", "find link opportunities", EN or FR markets. Distinct from on-page/technical SEO (an SEO-audit skill), product-listing/store content (a store-content skill), and any single directory/marketplace listing channel (a distribution skill).
---

# Backlinks Expert

Senior-level doctrine for **off-page SEO link acquisition** — building backlinks that actually move rankings and survive Google's link-spam policy, while never endangering a real business with a penalty. This skill owns the **strategy, the target discovery + qualification, and the asset generation** for link building across any set of properties (money sites, owned brand/lead-gen domains, and product/tool pages on third-party platforms) and any future site, in any market/language (EN + FR seeded; KR/ES/PT/DE/AR/HI extensible).

It is opinionated and **platform-agnostic**: the doctrine applies to any website. It encodes one foundational frame — **a backlink is worth what an editor would have given it.** Earned, relevant, editorial placement is the only durable currency. Everything else (submitted profiles, forum signatures, directories, bought followed links) is either a *traffic/brand* play or a *risk*, never a reliable ranking lever. The skill is white-hat at its core, with a small, explicitly **risk-labeled** tier-2 layer used only where it's safe to.

---

## How Google actually values a link in 2026

Three things make a link valuable, in order:

1. **Relevance** — topical fit between the linking page and the target. A niche-relevant link from a modest site beats a high-authority link from an unrelated one. This is the single most under-weighted factor.
2. **Authority** — the linking page's own earned trust (real editorial reputation, not a third-party score). **DR (Ahrefs) and DA (Moz) are NOT Google signals** — they are third-party estimates, useful only as rough triage, never as ground truth, and the numbers in "dofollow lists" are recycled and often years stale.
3. **Earned editorial placement** — a human editor chose to link because the content deserved it, with a `<a href>` that's crawlable, in-context, with a natural anchor.

**What Google penalizes (link-spam policy, current):** buying/selling links for ranking (paid links must carry `rel="sponsored"`/`nofollow`); exchanging goods/services for links; excessive reciprocal exchanges; automated/scaled link creation; low-quality directory/bookmark links; **forum comments or signature links with optimized anchors** (named explicitly); guest/advertorial/PR links with optimized anchors that pass credit; site-reputation abuse ("parasite SEO" — third-party content placed only to borrow a domain's authority); PBNs and expired-domain abuse. Most of what generic "free backlink" listicles teach falls into these buckets — treat those lists as *leads to vet*, not authorities. Full doctrine: `references/link-building-doctrine.md` and `references/ethics-risk.md`.

**Honest framing (do not pretend otherwise):** forum / profile / directory *submission* is a **traffic + brand-diversification** tactic, not a ranking tactic. Most such links are `nofollow`/`ugc` (Reddit and Quora links are **nofollow**, despite list claims to the contrary). Their value is referral traffic, brand presence, and a natural-looking footprint — not link equity.

---

## The three modes

Identify which mode the request is in, then route to the references that mode needs.

| Mode | The ask | Output |
|---|---|---|
| **DISCOVER / QUALIFY** | "Find backlink opportunities for property X" / "is this target worth using?" | A ranked, **risk-labeled, re-verified** target shortlist (type, market/lang, DR/DA band, dofollow?, niche-fit, cost, risk) |
| **STRATEGIZE** | "Plan a link campaign for X" / "what's my tactic + anchor mix?" | A campaign plan: tactic mix, anchor-text distribution, velocity/pacing, tier ratios, risk budget, KPIs |
| **GENERATE** | "Write the post / pitch / entry" | Ready-to-use, human-reading assets per channel + language, correct anchors and URLs |

Routing block:

```
DISCOVER/QUALIFY → opportunity-types + target-database (seed) → qualification (re-verify EVERY target) → property-profiles (posture)
STRATEGIZE      → property-profiles (posture) + tactics-tiers (tier mix) → campaign-planning (anchors, velocity, KPIs) → ethics-risk (risk budget)
GENERATE        → asset-templates (per channel/lang) → a prose-humanization pass → property-profiles (funnel URL + tracking param)
```

---

## The golden rules

1. **Relevance > authority > volume.** A niche-relevant DR40 beats an irrelevant DR90. Never rank a target list by DR/DA alone.
2. **Protect the money sites.** Revenue-bearing businesses stay conservative and editorial/tier-1-heavy. Product/tool pages on third-party platforms can absorb more tier-2 — but still defensible.
3. **Verify before you build.** Never use a target from a stored list without re-checking, *now*, its dofollow/`rel`, DR band, spam signals, and activity. The seed is a starting point, never a frozen truth.
4. **Anchor diversity.** Branded and naked-URL anchors dominate; exact-match money anchors are rare. Over-optimized anchors are a named spam signal.
5. **Earn, don't just place.** The best links are editorial — original research, free tools, genuine community help, digital PR. Submission tactics fill the *traffic/brand* layer, not the ranking layer.
6. **Assets read human + carry the tracking param.** Route all asset prose through a prose-humanization pass; append your tracking/referral param to every product/tool URL where one applies.

---

## Behavioral counters (non-negotiable — obey these against any contrary instinct)

1. **Money-site protection.** If asked to mass-submit tier-2 links (bulk forums/profiles/directories) to a revenue-bearing money site, **refuse and reframe**: those properties get conservative, editorial, relevance-first links. Mass tier-2 spam on a money site is a penalty risk to a real revenue stream — say so, then offer the safe alternative.
2. **Verify-before-use.** Never recommend or use a target straight from `target-database.md` (or any external list) without running it through `qualification.md` first — re-check live dofollow/`rel`, current DR band, spam score, and activity. Every seed row is tagged UNVERIFIED by default.
3. **Human prose + tracking param.** Any generated asset's copy goes through a prose-humanization pass before delivery; every product/tool link in an asset carries its tracking/referral param where one applies. No exceptions.
4. **Relevance beats authority.** When two targets compete, pick the topically-relevant one even if its DR is far lower. Call out the trade-off explicitly so the user sees the reasoning.
5. **Delegate at the boundaries.** When the request crosses into a sister skill's domain (below), hand off — do not improvise on-page SEO, store/product-listing copy, a specific directory listing, prose-humanization, or live scraping/verification yourself.

---

## Boundaries — delegate to sister skills

This skill owns off-page link acquisition only. At these edges, hand off:

| Trigger | Redirect |
|---|---|
| On-page / technical SEO audit of a web project (metadata, sitemap, canonical, internal linking, Core Web Vitals) | an on-page/technical SEO-audit skill |
| Store / product-listing content, input schemas, listing descriptions, and any tracking-param convention | a store/product-content skill |
| Publishing/auditing a listing on a specific directory or marketplace (one channel) | a directory/marketplace-distribution skill |
| Making asset prose read human / pass AI-detection | a prose-humanization skill |
| Finding/scraping target lists at scale, and verifying DR/dofollow/spam **programmatically** | a scraping skill + managed scraping APIs — **NEVER scrape from the local machine** |

The last row carries a hard rule: no HTTP request to a third-party site from the local machine. Target harvesting and DR/dofollow verification run on managed scraping APIs (Firecrawl, etc.) or remote scraping infrastructure, never from a local IP.

---

## Load-on-demand references

The body above answers most requests. Reach for `references/` when:

| Read this | When you need to… |
|---|---|
| `references/link-building-doctrine.md` | Ground a decision in how links earn value in 2026 — relevance/authority/E-E-A-T, anchor doctrine, velocity, crawlable-link rules, and what Google's link-spam policy penalizes |
| `references/tactics-tiers.md` | Pick tactics by tier + risk — tier-1 editorial (guest post, niche edit, digital PR/HARO, resource/broken-link); risk-labeled tier-2 (forum, profile, directory, comment); explicit "avoid" (PBN, undisclosed paid dofollow, mass spam, reciprocal schemes) |
| `references/opportunity-types.md` | Understand the opportunity taxonomy — forums, profiles, directories, guest posts, niche edits, resource/broken-link, HARO/digital-PR, Q&A (Reddit/Quora), brand-mention reclamation, web2.0 |
| `references/target-database.md` | Pull the vetted EN/FR **seed** (tagged by type/market/DR-band/dofollow?/niche-fit/risk/cost) — every row UNVERIFIED, a sourcing pool to hand-pick from, never a deploy list |
| `references/qualification.md` | Vet ANY target before use — relevance, DR/DA band, live dofollow/`rel` check, spam score, traffic, outbound-link count, penalty signals — via managed APIs / remote scraping (no local fetch) |
| `references/property-profiles.md` | Get a property's niche, market/language, audience, money-vs-tool posture, funnel URL (+ tracking param), seed anchor mix, and do/don't — or add a new property |
| `references/asset-templates.md` | Generate the actual per-channel + per-language asset (guest-post pitch/outline, niche-edit insertion, forum post, profile bio, directory entry, Q&A answer) — all cross-ref a prose-humanization pass |
| `references/campaign-planning.md` | Turn a goal into a plan — tactic mix per property/budget, anchor distribution, velocity, tier ratios, sequencing, KPIs and tracking (GSC, referring domains), with vanity metrics deprioritized |
| `references/ethics-risk.md` | Apply the risk layer — Google link-spam policy alignment, FTC-style disclosure for paid/sponsored, money-site protection, and the explicit "what we won't do" list |

---

## What this skill is not

- **Not on-page SEO.** Metadata, structured data, internal linking, performance → an on-page SEO skill.
- **Not a content-writing skill for store/product-listing copy.** Listing/publishing artifacts → a store/product-content skill.
- **Not a license to spam.** Bulk submission, bought followed links, PBNs, and reciprocal schemes are out of scope and documented as what-not-to-do — they endanger real businesses.
- **Not a frozen target list.** The seed database is a vetted *starting point*; freshness re-verification is mandatory before any target is used.
