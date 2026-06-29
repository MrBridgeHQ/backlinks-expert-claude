# Backlinks Expert — a Claude skill

A Claude Code skill that turns off-page SEO / link building into a disciplined workflow: it discovers and qualifies link opportunities, designs a link campaign (tactic mix, anchor-text distribution, velocity, tier ratios, risk budget), and generates ready-to-adapt submission/outreach assets — guest-post pitches, niche edits, forum/profile/directory entries, Q&A answers, and digital-PR.

It is **platform-agnostic** and opinionated. It encodes one frame: **a backlink is worth what an editor would have given it.** Earned, relevant, editorial placement is the only durable ranking currency; everything else (forum signatures, profiles, directories, bought followed links) is a *traffic/brand* play or a *risk*, never a reliable ranking lever. The skill is white-hat at its core, with a small, explicitly **risk-labeled** tier-2 layer.

## Why this skill exists

Most "free backlinks" advice on the open web is wrong, stale, or self-serving — recycled DA/DR numbers, "dofollow forum" lists that are mostly nofollow, and bulk-submission tactics that Google's link-spam policy names explicitly. An agent that absorbs those listicles uncritically gives advice that wastes effort at best and risks a manual action on a real business at worst.

This skill anchors every decision in Google's own published policy (Search Central spam policies + link best-practices) and treats everything else as a *lead to verify*. It is built around two protections:

- **Money-site protection.** Revenue-bearing businesses get conservative, tier-1-heavy, editorial link mixes. Bulk tier-2 spam on a money site is a penalty risk to a real revenue stream — the skill refuses and reframes.
- **Verify-before-use.** No target is used straight from a stored list. Live `rel`/dofollow, current DR band, spam score, indexation, and activity are re-checked first — via managed APIs / remote scraping, never a local fetch.

## What it can do

**Three modes:**
- **Discover / Qualify:** find link opportunities for a property and vet them into a risk-labeled, re-verified shortlist.
- **Strategize:** turn a goal into a campaign plan — tactic mix, anchor distribution, velocity, tier ratios, KPIs.
- **Generate:** produce human-reading, per-channel, per-language assets with correct anchors and URLs.

**Markets:** EN + FR seeded; KR / ES / PT / DE / AR / HI extensible (with an honest "thin market" read where a market genuinely lacks link-friendly communities).

## What's inside

```
backlinks-expert/
├── SKILL.md                          # Orchestration hub: modes, golden rules, behavioral counters, routing
├── README.md                         # This file
├── INSTALL.md                        # Installation instructions
└── references/
    ├── link-building-doctrine.md     # How Google values a link in 2026 — the four pillars + the link-spam policy + myth-busting
    ├── tactics-tiers.md              # Tactic catalog by tier and risk (tier-1 editorial / tier-2 foundational / AVOID)
    ├── opportunity-types.md          # Link-source taxonomy with honest dofollow defaults
    ├── target-database.md            # Vetted EN/FR + KR/ES/PT/DE/AR/HI seed — every row UNVERIFIED, a sourcing pool
    ├── qualification.md              # The verify-before-use gate (9-step checklist, managed-API only)
    ├── property-profiles.md          # Per-property posture templates (money / hybrid / tool) + anchor mixes
    ├── campaign-planning.md          # The strategist — goal, tier ratio, anchor mix, velocity, sequence, KPIs
    └── ethics-risk.md                # Google policy alignment, disclosure, money-site protection, what-we-won't-do
```

## Installation

See `INSTALL.md`. TL;DR for macOS/Linux:

```bash
mkdir -p ~/.claude/skills
unzip backlinks-expert.zip -d ~/.claude/skills/
```

## How to invoke

Once installed, the skill auto-activates on link-building requests. Example prompts:

- "Build backlinks for my SaaS landing page — what's the tactic and anchor mix?"
- "Find link opportunities for a wine e-commerce site in France, and tell me which are safe."
- "Plan a link campaign for a new domain that needs indexation and rankings."
- "Write a guest-post pitch and a niche-edit insertion for this article."
- "Is this 'top 50 dofollow forums' list worth using?"

If auto-activation misses, force it: "Use the `backlinks-expert` skill to..."

## Boundaries

This skill owns **off-page link acquisition** only. It delegates at the edges:

- On-page / technical SEO (metadata, sitemap, canonical, internal linking, Core Web Vitals) → an on-page SEO-audit skill.
- Store / product-listing content and schemas → a store/product-content skill.
- A specific directory/marketplace listing channel → a directory/marketplace-distribution skill.
- Making asset prose read human / pass AI-detection → a prose-humanization skill.
- Harvesting/verifying target lists at scale → a scraping skill + managed APIs (never a local fetch).

## Part of the mr-bridge.com toolkit

This skill is part of the [mr-bridge.com](https://mr-bridge.com) toolkit for scraping, data, and content automation. Related resources:

- [mr-bridge.com](https://mr-bridge.com) — home
- [Scrapers](https://mr-bridge.com/scrapers) — the scraper portfolio
- [MCP servers](https://mr-bridge.com/mcp-servers) — Model Context Protocol servers
- [AI workflows](https://mr-bridge.com/ai-workflows) — agents and automation
- [Studies](https://mr-bridge.com/studies) — data studies and one-pagers
- [Articles](https://mr-bridge.com/articles) — write-ups and guides
- [Solutions](https://mr-bridge.com/solutions) — end-to-end solutions

## License

Personal use. Customize freely. No warranty. This skill is link-building doctrine, not legal advice; it is a risk posture built on Google's published policy. Verify any live claim (dofollow status, DR band, indexation) before acting on it.
