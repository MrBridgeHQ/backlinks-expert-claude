# Target Database - A Vetted Seed, Not a Frozen List

**Scope note - read this before using anything below.** These are **UNVERIFIED leads**
harvested from low-authority "list" articles (the "top 50 dofollow forums" genre). None
of the rows were visited and checked live; the DA/DR numbers are the source articles'
own claims (mostly recycled Moz DA, often years stale, sometimes self-contradictory);
the "dofollow?" column is what the source *asserted*, not the live `rel` attribute. Two
authoritative Google Search Central pages were also consulted and they overrule the
listicles wherever they disagree.

Three hard truths this table is built around:

1. **Most forum / profile / directory links are a traffic/brand play, not a ranking
   play.** Google explicitly names forum-signature links and low-quality directory
   links as link spam; honest sources concede these links have little-to-no direct SEO
   equity and are mostly nofollow/UGC. Their value is referral traffic, brand
   visibility, and profile diversity - file them there, do not overstate them.
2. **Reddit and Quora are nofollow.** Any source tagging them "dofollow" is wrong.
   Same for Stack Exchange. Traffic/brand only.
3. **DA/DR is not a Google signal.** It's a third-party metric, useful only as a coarse
   "is this a real site?" triage band - never as a value claim.

**Every row carries an implicit `UNVERIFIED - verify before use` warning.** Before you
act on any target, run it through `qualification.md` (relevance → live dofollow check →
indexation → real metric → spam → traffic → OBL → penalty/PBN → activity). The list is
a *starting pool to hand-pick from*, never a deploy list. Treat it like a stale scraper
target: re-check before you trust it.

This is **Approach A**: a vetted seed with verify-before-use, not an authoritative
frozen database. It rots; qualification is what keeps it honest.

Tag legend:
- **risk tier** - `T1` editorial/earned (lowest risk); `T2` foundational
  forum/profile/directory (risk-labeled, use in moderation, traffic/brand only);
  `AVOID` (paid-followed, blackhat, PBN, bulk-submission).
- **dofollow? (verify!)** - source claim only; the live `rel` MUST be re-inspected
  per-slot per `qualification.md` §2.
- **niche-fit** - which kind of property the lead plausibly serves (dev = developer /
  tool / SEO properties; wine = a wine vertical, used here only as an illustrative niche;
  travel = a travel vertical; - = off-niche / generic). Map these to your own
  properties' niches.
- **cost** - free unless noted; paid intermediaries flagged `AVOID` for followed links.

---

## EN / language-neutral targets (seed)

All rows: **UNVERIFIED - re-verify via `qualification.md`.** DA = source-claimed only.

| target | type | market/lang | claimed DA (source-claimed) | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| sitepoint.com/community | forum (web dev) | EN | 87 | claimed yes | dev | T2 | free |
| stackoverflow / github.com (profile/README) | profile/community (dev) | EN | 96 | profile link (verify) | dev | T2 | free |
| digitalocean.com/community | community (dev/cloud) | EN | 88–89 | unstated | dev (high fit) | T2 | free |
| webhostingtalk.com | forum (hosting) | EN | 63–75 | claimed yes | dev/infra | T2 | free |
| forums.cpanel.net | forum (hosting) | EN | 94 | claimed yes | dev/infra | T2 | free |
| ubuntuforums.org | forum (linux) | EN | 79 | claimed yes | dev/infra | T2 | free |
| forums.mysql.com | forum (DB/dev) | EN | 92 | claimed yes | dev | T2 | free |
| forum.xda-developers.com | forum (mobile dev) | EN | 92 | claimed yes | dev | T2 | free |
| dev.to (publish, not a dead slug) | publishing/community (dev) | EN | high | author links | dev (high fit) | T1/T2 | free |
| stackexchange (various) | qa (dev) | EN | high | **nofollow** | dev | T2 (traffic) | free |
| warriorforum.com | forum (internet marketing) | EN | 66–71 | claimed yes | dev/SEO (adjacent) | T2 | free |
| forums.seochat.com | forum (SEO) | EN | 69 | claimed yes | dev/SEO | T2 | free |
| forums.seroundtable.com | forum (SEO news) | EN | 74 | unstated | dev/SEO | T2 | free |
| seo-forum.link-assistant.com | forum (SEO) | EN | 59 | claimed yes | dev/SEO | T2 | free |
| forums.digitalpoint.com | forum (webmaster/IM) | EN | 72 | **disputed** (policy changed) | dev/SEO | T2 | free |
| webmasterworld.com | forum (webmaster) | EN | 78 | **partial/historically nofollow** | dev/SEO | T2 | free |
| moz.com/community/q | qa (SEO) | EN | high | gated (Moz Pro) | dev/SEO | T2 | gated |
| forum.joomla.org | forum (CMS) | EN | 91 | claimed yes | dev | T2 | free |
| phpbb.com/community | forum (software) | EN | 88 | claimed yes | dev | T2 | free |
| forum.filezilla-project.org | forum (software) | EN | 88 | claimed yes | dev | T2 | free |
| forum.openoffice.org | forum (software) | EN | 86 | claimed yes | - | T2 | free |
| forum.parallels.com | forum (software) | EN | 92 | claimed yes | dev | T2 | free |
| 000webhost.com/forum | forum (hosting) | EN | 92 | claimed yes | dev/infra | T2 | free |
| namepros.com | forum (domains) | EN | 50–70 | claimed yes | dev (domains/expired) | T2 | free |
| dnforum.com | forum (domains) | EN | 40–61 | claimed yes | dev (domains) | T2 | free |
| antionline.com | forum (security) | EN | 50 | claimed yes | dev (adjacent) | T2 | free |
| v7n.com / ozzu.com | forum (IM/webmaster) | EN | 51 / 52 | claimed yes | dev/SEO | T2 | free |
| cheftalk.com/forums | forum (cooking) | EN | - | claimed yes | **food/wine** | T2 | free |
| weddingwire.com / hitched.co.uk | forum (weddings) | EN | - | "DOFOLLOW" (verify) | **events/food** | T2 | free |
| fragrantica.com | forum (perfume/taste) | EN | - | "DOFOLLOW" (verify) | luxury/taste (adjacent) | T2 | free |
| disboards.com | forum (Disney/travel) | EN | - | "DOFOLLOW" (verify) | **travel** | T2 | free |
| caminodesantiago.me | forum (travel) | EN | - | "DOFOLLOW" (verify) | **travel** | T2 | free |
| cruise.co.uk | community (travel) | EN | - | "DOFOLLOW" (verify) | **travel** | T2 | free |
| expat.com / expat-blog.com | community (travel/expat) | EN | 59 | unstated | **travel/expat** | T2 | free |
| aseannow.com (was tripadvisor-listed) | forum (travel SEA) | EN | 49 | claimed yes | **travel** | T2 | free |
| investing.com (forum) | forum (finance) | EN | - | "DOFOLLOW" (verify) | dev (BI/pricing angle) | T2 | free |
| analystforum.com | forum (finance) | EN | - | "DOFOLLOW" (verify) | dev (BI angle) | T2 | free |
| cnet.com/forums | forum (tech) | EN | 95 | claimed yes (status uncertain) | - | T2 | free |
| city-data.com/forum | forum (general/local) | EN | 86 | claimed yes | - | T2 | free |
| forum.wordreference.com | forum (language) | EN/multi | 81–92 | claimed yes | - | T2 | free |
| forum.audacityteam.org | forum (audio) | EN | 84 | claimed yes | - | T2 | free |
| blenderartists.org | forum (3D) | EN | 56–63 | claimed yes | - | T2 | free |
| deviantart.com | community (creative) | EN | 89 | claimed yes | - (off-niche) | T2 | free |
| forum.bodybuilding.com | forum (fitness) | EN | 79–86 | claimed yes | - (off-niche) | T2 | free |
| skyscrapercity.com / gardenweb.com / filesharingtalk.com / windowsforum.org | forum (various) | EN | - | claimed yes | - (off-niche) | T2 | free |
| reddit.com | qa/community | EN | high | **nofollow (UGC) - list "dofollow" is FALSE** | varies by subreddit | T2 (traffic only) | free |
| quora.com | qa | EN | high | **nofollow** | varies | T2 (traffic only) | free |
| HARO / Connectively | journalist outreach (digital PR) | EN | n/a | earns editorial links | all (high fit) | **T1** | free |
| blackhatworld.com | forum (blackhat) | EN | 55–59 | listed only | - | **AVOID** (reputational) | free |
| LinkBuilder.com, WMLinks, LinksClerk, NeedMyLink, Love To Link, BackLinker, Links-Stream, CrowdLinks, BrandCitations, WebOperators | crowd-platforms / guest-post marketplaces | EN | - | paid (mostly nofollow) | - | **AVOID** for followed links | $ paid |

---

## FR targets (seed)

All rows: **UNVERIFIED - re-verify via `qualification.md`.**

| target | type | market/lang | claimed DA (source-claimed) | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| webrankinfo.com/forum | forum (SEO) | FR | - | unstated (verify) | dev/SEO (high fit) | T2 | free |
| scripts-seo.com | forum (technical SEO) | FR | - | unstated (verify) | dev/SEO (high fit, low spam) | T2 | free |
| forum.lesmakers.fr | forum (business/digital) | FR | - | unstated | dev/SEO (SEO section) | T2 | free |
| forums.commentcamarche.net (référencement) | forum (tech) | FR | high | unstated | dev/SEO | T2 | free |
| forums.futura-sciences.com | forum (science) | FR | 90 | claimed yes | dev (adjacent) | T2 | free |
| webmaster-hub.com | forum (webmaster) | FR | - | unstated | dev/SEO | T2 | free **(possibly dead - verify activity)** |
| support.google.com/webmasters/community (FR) | community (official) | FR | - | **nofollow (official)** | dev/SEO | T2 (authority, no juice) | free |
| livementor (communauté) | community (business) | FR | - | unstated | - | T2 | free |
| phpbb-fr.com/forums | forum (software) | FR | 49 | claimed yes | dev | T2 | free |
| bathotel.free.fr | forum | FR | 77 | unstated | - | T2 | free **(odd entry - verify)** |
| forum.nature-and-garden.com | forum (gardening) | FR/EN | - | "DOFOLLOW" (verify) | - | T2 | free |
| forum.magic.fr | forum | FR | - | "DOFOLLOW" (verify) | - | T2 | free |
| forum.taggle.org | forum (SEO) | FR | - | n/a | dev/SEO | **archive only - defunct** | - |
| FR paid-link platforms (e.g. RocketLinks, netlinking.fr, Boosterlink) | FR paid-link platforms | FR | - | paid | - | **AVOID** for followed links (~150€+/link) | $ paid |
| expired-domain marketplaces | expired-domain / PBN sourcing | FR | - | n/a | - | **AVOID** (expired-domain abuse) | $ paid |

Adjacent-language strays found in the FR lists (not FR - reclassify if used): `forum.html.it` (IT, dev, DA 62, claimed dofollow); `forum.abakus-internet-marketing.de` (DE, SEO, DA 43, claimed dofollow).

---

## Extensible market slots - KR / ES / PT / DE / AR / HI

If a property is multilingual (EN/FR/ES/PT/DE/AR/HI) or targets a specific local or
export market, seed those markets the same way. The slots below are **seeded (UNVERIFIED)** - real leads harvested via managed search, never verified live; re-verify before use, and
top up on demand using the method below. Do not invent targets; harvest, then qualify.

### Method to fill a market slot

1. **Harvest leads (never local-scrape).** Use a managed search/scrape API (e.g.
   Firecrawl `firecrawl_search` / `firecrawl_scrape`, `onlyMainContent: true`, cache via
   `maxAge`) or a SERP API to find, in the target language, the equivalent "list"
   sources and the actual communities:
   - SERP queries in-language: e.g. KR `"개발자 포럼"` / `"SEO 포럼"`, DE `"SEO Forum
     dofollow Liste"`, ES `"foros para backlinks"`, PT `"fóruns dofollow"`, AR/HI
     equivalents; plus niche queries (your vertical) in-language.
   - Competitor backlink exports (via a remote Ahrefs/SEMrush-style metric job) for a
     same-market competitor - far higher-signal than listicles.
   - In-market directories, niche communities, and local digital-PR/journalist outlets.
2. **Tag each lead** with the same columns (type | market/lang | claimed DA/DR |
   dofollow? | niche-fit | risk tier | cost) and mark every row **UNVERIFIED**.
3. **Qualify before use** via `qualification.md` - in particular the live dofollow
   check and indexation check, which matter even more cross-language (translated
   listicles recycle stale, wrong claims).
4. **Prefer in-language, in-market relevance.** A modest in-market community beats a
   high-DR English forum for an in-market-targeted page (relevance > authority).

### Slots (illustrative seed - UNVERIFIED, re-verify before use)

#### KR (Korean) - dev + a local-market vertical (illustrative)
All rows **UNVERIFIED - re-verify via `qualification.md`.** Harvested via managed search (in-Korean SERP). DA/DR not stated by sources (KR listicles rarely cite Moz DA) - left blank, triage live.
| target | type | market/lang | claimed DA/DR | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| okky.kr | community/Q&A (dev) | KR | - | unstated (verify) | dev (high fit - largest KR dev community, ~180k devs) | T2 | free |
| velog.io | publishing/community (dev) | KR | - | author links (verify) | dev (high fit - popular KR dev blog platform) | T2 | free |
| wine21.com | wine portal/media + community | KR | - | unstated (verify) | **wine (high fit - largest KR wine portal; illustrative vertical)** | T2 | free |
| sommeliertimes.com | wine news/community (동호회 coverage) | KR | - | unstated (verify) | **wine (KR wine trade/community media; illustrative)** | T2 | free |
| wine.co.kr | wine portal | KR | - | unstated (verify) | **wine (illustrative vertical)** | T2 | free |
| blog.naver.com / tistory.com | blog platforms (Naver/Daum ecosystem) | KR | - | mostly **nofollow** (verify) | dev/vertical (KR domestic reach, traffic only) | T2 (traffic) | free |

#### ES (Spanish) - dev + vertical
All rows **UNVERIFIED - re-verify via `qualification.md`.** Harvested via managed search (in-Spanish SERP). DA blank unless a source asserted one.
| target | type | market/lang | claimed DA/DR | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| mediavida.com/foro/dev | forum (dev/tech) | ES | - | unstated (verify) | dev (high fit - active ES dev forum) | T2 | free |
| betabeers.com (foro/comunidad) | community (dev) | ES | - | unstated (verify) | dev (ES/LatAm dev reference - **verify still active**) | T2 | free **(may be dormant - verify activity)** |
| foro.elhacker.net | forum (security/dev) | ES | - | unstated (verify) | dev (adjacent - security/IT) | T2 | free |
| forocoches.com | forum (general, very high traffic) | ES | - | likely **nofollow** (verify) | - (off-niche, traffic only) | T2 (traffic) | free |
| foros de Xataka / ADSLZone / Hard2mano | forum (tech/consumer) | ES | - | unstated (verify) | dev/tech (adjacent) | T2 | free |
| verema.com/foros/foro-vino | forum (wine) | ES | - | unstated (verify) | **wine (high fit - top ES wine forum; illustrative)** | T2 | free |
| foro.e-nologia.com | forum (enology/viticulture + wine buy/sell) | ES | - | unstated (verify) | **wine (high fit, technical/trade; illustrative)** | T2 | free |
| ES backlink-list articles (source of leads, not targets) | ES backlink-list articles | ES | - | n/a | - (meta - mostly point to global Web 2.0 platforms) | n/a | free |
| business directories (Yelp ES / local equivalents) | business directory | ES | - | mostly **nofollow** (verify) | - (citation/NAP, traffic) | T2 | free |

#### PT (Portuguese, BR+PT) - dev + vertical
All rows **UNVERIFIED - re-verify via `qualification.md`.** Harvested via managed search (in-Portuguese SERP). Dev side is strong (BR); a wine-style vertical came up thin (only events/trade orgs - institutional, not link-friendly community forums).
| target | type | market/lang | claimed DA/DR | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| tabnews.com.br | community (dev/tech, reddit-style) | PT-BR | - | unstated (verify) | dev (high fit - active BR dev community) | T2 | free |
| forum.casadodesenvolvedor.com.br | forum (dev) | PT-BR | - | unstated (verify) | dev (high fit - BR developer forum) | T2 | free |
| devmedia.com.br/forum | forum (dev Q&A) | PT-BR | - | unstated (verify) | dev (high fit - large BR programming forum) | T2 | free |
| _(a wine-style PT vertical: no link-friendly community forum found - only trade/event orgs; treat as digital-PR/news targets, T1 if earned, not forum-style)_ | trade/news org | PT | - | n/a | vertical (PR angle only) | T1 (if earned) | free |

#### DE (German) - dev/SEO + vertical
All rows **UNVERIFIED - re-verify via `qualification.md`.** Harvested via managed search (in-German SERP). Note: in-German "SEO Forum dofollow Liste" queries mostly returned **English** listicles - genuine DE-specific list articles are thin; the rows below are real DE communities found directly, not from a DE listicle.
| target | type | market/lang | claimed DA/DR | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| forum.abakus-internet-marketing.de | forum (SEO) | DE | 43 (from FR list) | claimed yes (verify) | dev/SEO (high fit - top DE SEO forum) | T2 | free |
| dev-community.de | community (dev/tech) | DE | - | unstated (verify) | dev (high fit - German dev community, successor of coding-board.de) | T2 | free |
| dasweinforum.de | forum (wine) | DE | - | unstated (verify) | **wine (high fit - dedicated DE wine forum; illustrative)** | T2 | free |
| forum.restaurant-ranglisten.de (Sommeliers/Winzer/Wein) | forum (gourmet/wine/sommelier) | DE | - | unstated (verify) | **wine (sommelier/wine board; illustrative)** | T2 | free |
| webmaster-forum / webmaster.de-style boards | forum (webmaster) | DE | - | unstated (verify) | dev/SEO | T2 | free **(verify each is live - many DE webmaster forums have died)** |

#### AR (Arabic) - dev
**Thin market.** In-Arabic SERP for `منتديات دوفولو` / backlink directories returned almost entirely **paid backlink-seller landing pages** and how-to guide articles - **not** open communities. Treat paid sellers as **AVOID** for followed links. Almost no genuine, link-friendly AR dev/tech forum surfaced (the historic ones were not confirmed live in this harvest). Only honest leads below; do not pad.
| target | type | market/lang | claimed DA/DR | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| ar.quora.com | qa | AR | - | **nofollow** | varies | T2 (traffic only) | free |
| paid AR backlink sellers | paid backlink services | AR | - | paid (claimed dofollow) | - | **AVOID** (paid-followed) | $ paid |
| _(no genuine open AR dev/tech community forum confirmed live in this harvest - re-harvest with named targets and verify before adding)_ | - | AR | - | - | - | - | - |

#### HI (Hindi / India) - dev
All rows **UNVERIFIED - re-verify via `qualification.md`.** Harvested via managed search. **Caveat:** the India market is overwhelmingly **English-language**, not Hindi - `dofollow forums India` returns EN-India submission lists, and real India dev/finance communities operate in English. So this slot overlaps the EN seed; rows are India-market (IN), not Hindi-language. The "directory submission sites India" genre is the **bulk-submission / spam-adjacent** category - file as AVOID-leaning, not as quality leads.
| target | type | market/lang | claimed DA/DR | dofollow? (verify!) | niche-fit | risk tier | cost |
|---|---|---|---|---|---|---|---|
| developersindia.in | community (dev/tech) | IN (EN) | - | unstated (verify) | dev (high fit - India's largest dev community, 1M+) | T2 | free |
| caclubindia.com | community (finance/CA/tax) | IN (EN) | - | claimed dofollow (verify) | dev (BI/finance angle, adjacent) | T2 | free |
| Indian "directory submission sites" lists | bulk directory-submission lists | IN | claimed high DA | claimed dofollow (mostly low-quality/recycled) | - | **AVOID-leaning** (bulk submission = link spam) | free |
| _(no Hindi-language community forum of value found - India's quality dev/finance communities are English; use the EN seed for India targeting)_ | - | HI | - | - | - | - | - |

---

## How to use this seed (the short version)

1. Pick the property and read its posture in `property-profiles.md` (money sites stay
   conservative and T1-heavy; tool/product pages tolerate more T2).
2. Filter the seed to rows whose **niche-fit** matches the property.
3. Run each candidate through **`qualification.md`** - relevance, live dofollow,
   indexation, real metric, spam, traffic, OBL, penalty/PBN, activity. All checks run
   via managed APIs / remote scraping, **never a local fetch**.
4. Keep only what survives. Record the verdict and the date checked.
5. **Re-verify before reusing** any row - a green verdict is only valid as of its check
   date. This list rots; the gate is what keeps it safe.

Never present a seed row's DA/dofollow/value as a fact. It is a claim until verified.
