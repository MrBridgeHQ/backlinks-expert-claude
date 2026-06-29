# Qualifying a Backlink Target — Verify Before You Build

A target list is a list of *leads*, not a list of links. Every entry in
`target-database.md` (and anything you find elsewhere — a listicle, a competitor
backlink export, a "top 50 dofollow forums" blog) is a hypothesis: *this page might
be worth a link.* Qualification is the step that turns a hypothesis into a decision.

The discipline here mirrors the scraping principle of "verify, don't trust
stale data." A DA/DR number copied across forty SEO blogs is not a fact about the
page in front of you. A "dofollow" tag in a list article is the author's claim, not
the live `rel` attribute. The forum that was a goldmine in 2021 may be dead,
noindexed, or nofollow today. **Re-check before you spend effort.**

This page is the gate. Nothing from `target-database.md` should be acted on until it
clears this checklist.

---

## The non-negotiable rule: never fetch from this machine

Every check below that requires looking at a target page is performed through a
**managed API or remote scraping infrastructure — never a local HTTP request.** The
local IP is never exposed to a third-party site. No `curl`, no `requests`, no `httpx`,
no headless browser pointed at the target from this box. Route every live check through
a managed scraping/search API or remote job.

What runs where:

| Check | Run via | Notes |
|---|---|---|
| Fetch the page HTML to inspect `rel` on the link slot | **Firecrawl** `firecrawl_scrape` (`onlyMainContent: false`, `formats: ['html']`) or a ZenRows-style HTML pass-through | Need raw HTML, not markdown — markdown strips the `rel` attribute. |
| Check whether the page/thread is indexed | A SERP API / Firecrawl `firecrawl_search` with a `site:` query | `site:forum.example.com "thread title"` — if Google has it, it can pass discovery value. |
| Estimate organic traffic / DR / DA / spam score | A remote Ahrefs/Moz/SEMrush-style metric job, or the vendor's own API if you hold a key | Third-party metric, context only — see "DR/DA is not a Google signal" below. |
| Count outbound links on the page | Firecrawl/ZenRows HTML → parse `<a>` count | High OBL = diluted, often spammy. |
| Read forum rules / activity / last-post dates | Firecrawl `firecrawl_scrape` of the board index | Confirms the community is alive and link-tolerant. |
| Bulk-qualify a harvested pool | A remote batch job over a URL list, writing metrics to a dataset | The right tool when triaging dozens of leads — not one-off MCP calls. |

If a check can only be answered by hitting the site, route it through one of these.
If you cannot verify a claim without a live fetch and no managed path is available,
**mark the target UNVERIFIED and do not recommend it as fact** — say "claimed, not
checked."

---

## The qualification checklist

Run these in order. The cheap, decisive checks come first — relevance and dofollow
kill most leads before you spend a metric-API credit on them.

### 1. Relevance to the property's niche (decisive — check first)

The first golden rule: **relevance > authority > volume.** A topically-aligned link
from a modest site beats a high-DR link from an unrelated one. Google emphasizes
topical relevance; an off-niche link passes little to no value and, in a signature or
profile slot, can look like exactly the spam pattern forums are penalized for.

Ask:
- Does the target's topic overlap the property's niche? (e.g. dev/scraping/MCP/SEO for
  a developer-tool property; the relevant vertical — food/luxury/events for a consumer
  brand, travel/expat for a travel property — for a money site. Map to the property
  you're working on.)
- Would a link to the property *help a real reader of that page*? If you cannot write
  a sentence where the link is genuinely useful in context, it is off-niche.
- Is there a natural placement (a relevant thread, a resource page, a roundup),
  or would you have to force it?

**Reject if** the only thing the target has going for it is a high DA and there is no
topical fit and no plausible reader who benefits.

### 2. Dofollow check — inspect the live `rel`, do not trust the list

List articles lie about this constantly. One source in the seed tagged literally
every entry — including reddit.com and quora.com — as "DOFOLLOW"; both are nofollow.
A site's policy also changes over time (DigitalPoint, WebmasterWorld, and others
flipped to nofollow years after the lists were written).

Procedure:
- Fetch the **actual page where your link would sit** (post body, signature, profile
  field, directory entry) as raw HTML via a managed scrape.
- Inspect the `<a>` for your slot. Look for `rel="nofollow"`, `rel="ugc"`,
  `rel="sponsored"`. Most modern forums apply `ugc` or `nofollow` to user links
  automatically.
- Different slots on the same site can differ — a profile field may be nofollow while
  a contextual post link is followed, or vice versa. Check the slot you'll actually use.
- A link rendered with `javascript:` / `onclick` / a `<span>` instead of a real
  `<a href>` is not crawlable and is worthless for discovery — treat as nofollow-or-worse.

**Important framing:** nofollow is **not** a disqualifier by itself. A nofollow link
on a high-traffic, indexed, on-topic thread delivers referral traffic, brand
visibility, and a natural-looking link profile. It just doesn't pass ranking equity —
so file it as a *traffic/brand* play, not a *ranking* play, and never overstate it.

**Reject (as a ranking play) if** the slot is nofollow/ugc AND the page has no real
traffic AND it's off-niche — that link does nothing for you.

### 3. Indexation

If Google hasn't indexed the page your link sits on, the link can't be discovered or
counted. Run `site:domain.com "page or thread title"` via a SERP API or Firecrawl search.

- Indexed thread on an active board → discovery + (if followed) equity possible.
- Noindex / not-found in Google → the link is invisible to search; only direct
  referral traffic remains, if any.

**Reject if** the host section is systematically noindexed (some forums noindex new or
low-activity threads) — your link will never be seen by Google.

### 4. Real DR / DA / authority band — third-party metric, context only

DR (Ahrefs) and DA (Moz) are **not Google ranking signals.** They are third-party
estimates. The seed's DA columns are recycled, often years stale, and sometimes
self-contradictory (the same source listed one site at both DA 55 and DA 59). Use a
metric only as a coarse triage band — "is this a real site or a throwaway?" — never as
ground truth or as a value claim.

- Pull a *current* metric via a remote metric job or the vendor API (not the list's
  number).
- Treat it as a band (low / mid / high), not a precise score.
- Authority without relevance is worth little (see check 1).

**Reject if** the only argument for the target is its DR/DA and it fails relevance.

### 5. Spam score / link neighborhood

Check the site's spam score (Moz Spam Score or equivalent) and eyeball the
neighborhood: is it surrounded by gambling/adult/pharma/"gray niche" content, casino
sidebars, or thousands of unrelated outbound links?

**Reject if** spam score is high, or the page sits in an obviously toxic neighborhood —
a link from a bad neighborhood is a liability, especially for a money site.

### 6. Organic traffic

A site (and ideally the specific page) with real organic traffic offers referral value
even when the link is nofollow. Estimate via a traffic-metric job/API.

- Note: traffic is **not** a Google ranking factor (Google has said so). Use it to
  judge *referral* potential, not ranking potential.

**Reject if** the page has effectively zero traffic AND the link is nofollow AND it's
off-niche — there is no value left on any axis.

### 7. Outbound-link count (OBL)

The more outbound links on a page, the less any single one is worth, and a page
stuffed with hundreds of unrelated outbound links is a link-farm/directory-spam signal.
Count `<a>` to external domains in the page HTML.

**Reject if** the page is an OBL dump (a "links page" with hundreds of unrelated
external links) — that's the low-quality-directory pattern Google names as link spam.

### 8. Penalty / PBN / scaled-abuse signals

Look for the tells of a network or a penalized site:
- Thin, AI-spun, or off-topic content padding the domain.
- A "write for us / submit your link" page that sells followed links (paid followed =
  policy violation; the link is risky to be near).
- Footprint of a PBN: same template, same ad blocks, same hosting, interlinked
  thin sites, an expired domain repurposed with unrelated content.
- A site whose traffic graph fell off a cliff (a metric job often shows this) —
  possible Google penalty.

**Reject if** the target shows PBN/expired-domain-abuse footprints or sells followed
links — being in that neighborhood endangers the property, and the money sites get
nowhere near it.

### 9. Activity & link tolerance (for forums/communities)

A backlink on a dead forum yields nothing. Confirm:
- Recent posts and real replies (last-post dates within weeks, not years).
- Active moderation and readable rules — and that the rules permit links at all (a ban
  deletes all your links retroactively).
- That contextual links, not just signatures, are tolerated.

**Reject if** the forum is dead/abandoned, or its rules forbid links (you'll be banned
and lose everything you placed).

---

## "Reject if…" — the fast disqualifiers

Drop a target immediately if any of these is true:

- **Off-niche with no relevant placement** and nothing but a DA number to recommend it.
- **The link slot is nofollow/ugc AND the page is low-traffic AND off-niche** — zero
  value on every axis (a nofollow link that is on-topic and high-traffic is *kept* as a
  traffic play).
- **Host section is noindexed** — the link can never be discovered by Google.
- **Page is an outbound-link dump** (low-quality directory / links page).
- **High spam score or toxic neighborhood** (gambling/adult/pharma, casino sidebars).
- **PBN / expired-domain-abuse footprint**, or the site **sells followed links**.
- **Dead or link-hostile forum** (no recent activity, or rules ban links).
- **Not a real `<a href>`** (JS/onclick/span "link") — not crawlable, no SEO value.
- **You cannot verify the claim and no managed-API path exists** — keep it tagged
  UNVERIFIED; never present a guess as a fact.
- **It's a paid *followed* link without `sponsored`/`nofollow`** — policy violation;
  see `ethics-risk.md`.
- **Money-site context + any tier-2/risk signal** — money sites stay conservative;
  when in doubt on a money site, reject. (See the per-property posture in
  `property-profiles.md`.)

---

## Output of a qualification pass

For each lead, record the verdict so the campaign planner can use it:

```
target: forums.cpanel.net (hosting forum)
property: yourbrand.com (dev/scraping niche)
relevance:    PASS — infra/hosting overlaps scraping/MCP audience
dofollow:     nofollow (ugc) on post links — VERIFIED via managed scrape (raw HTML)
indexed:      yes (site: query returns threads)
DR/DA band:   high (third-party, context only)
spam score:   low
traffic:      high
OBL:          normal
penalty/PBN:  none
activity:     active, links tolerated in context per rules
VERDICT:      USE as a traffic/brand play (nofollow — not a ranking link);
              place a contextual, genuinely-helpful answer, one link max.
checked:      <date> — re-verify before next use
```

A target is only ever "qualified **as of** the date you checked it." Re-run the gate
before reusing a stale verdict — the same way you would re-verify a scraper target
that worked last month.
