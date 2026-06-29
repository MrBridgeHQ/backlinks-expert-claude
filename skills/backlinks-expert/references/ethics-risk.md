# Ethics, Risk, and the Lines We Don't Cross

Link building sits in a reputational grey area the same way scraping sits in a legal one. The technical question — "can we get this link?" — is almost always yes. The right question is "should we, and what does it cost us if Google notices?" This page is the boundary discipline for the whole skill: Google's link-spam policy, how penalties actually happen, disclosure obligations, why real businesses must stay conservative, and the explicit list of things this skill will not build or do.

This is not legal advice and it is not a Google insider's certainty. It is a risk posture built on Google's own published policy and on being honest about what is and isn't a ranking signal. Everything in `campaign-planning.md` and `tactics-tiers.md` is governed by the limits here.

The core principle, stated once: **we earn and place links that we'd be comfortable showing the property owner, the linking site's editor, and a Google reviewer simultaneously.** If a link only works because one of those three doesn't know about it, we don't build it.

---

## The authority: Google's link-spam policy

Two Google Search Central pages are authoritative and overrule every SEO listicle:

- **Source A** — `developers.google.com/search/docs/essentials/spam-policies` (Link spam section).
- **Source B** — `developers.google.com/search/docs/crawling-indexing/links-crawlable` ("Link best practices").

When a "free backlinks" article and Google disagree, Google wins. The listicles that seed `target-database.md` are *leads to verify*, never authorities.

### What Google explicitly calls link spam (Source A)

Links intended to manipulate ranking are a spam-policy violation. Named categories:

- **Buying or selling links** for ranking purposes (passing followed credit).
- **Exchanging goods, services, or free products for links** — including "send us your product and we'll review it with a followed link."
- **Excessive reciprocal links** / link-exchange schemes ("link to me and I'll link to you" at scale).
- **Automated / programmatic link creation.**
- **Requiring a link** (e.g. in terms of service, contracts, widgets) without allowing it to be qualified with `nofollow`/`sponsored`.
- **Advertorial, native, guest-post, or press-release links with optimized anchor text** that pass ranking credit.
- **Low-quality directory or bookmark links.**
- **Forum comments with optimized links** in the post body or signature (named explicitly).
- **Widely distributed footer / template / widget links** across many sites.
- **Creating low-value content for the sole purpose of acquiring links.**

This list directly indicts the bulk of the "forum / directory / profile submission" tactics the source listicles teach. That's why those tactics live in tier-2 and are framed as *traffic/brand* plays, not ranking plays.

### Paid links are allowed — if qualified (Source A)

Buying and selling links is "a normal part of the web economy" for advertising and sponsorship. The line is the `rel` attribute: **a paid link must carry `rel="sponsored"` or `rel="nofollow"`.** A *followed* paid link is a violation. There is no honest exception to this. "Paid but dofollow and undisclosed" is the single clearest way to earn a manual action.

### Qualify UGC and untrusted links (Source B)

- `rel="sponsored"` — paid or advertising links.
- `rel="ugc"` — user-generated content (forum posts, Q&A answers, comments — links *you* insert into other people's UGC platforms).
- `rel="nofollow"` — untrusted or paid links you don't want to vouch for.

Google may treat these as hints rather than directives, but using them correctly is the difference between "honest participant" and "link spammer."

### Anchor text (Source B — authoritative, drives our anchor mix)

Good anchor text is **descriptive, concise, and relevant** to both pages and gives context. **Avoid** generic "click here"/"read more"; **avoid keyword-stuffed or over-long anchors** (explicitly named as keyword-stuffing spam); don't chain adjacent links; for image links the `alt` text is the anchor. → This is *why* `campaign-planning.md` mandates a branded/URL-dominant mix with exact-match anchors kept rare. Over-optimized anchors are a self-inflicted penalty risk.

### Crawlable links only (Source B)

Google reliably follows only real `<a href="">` elements with a resolvable URL. JavaScript `onclick`, `<span href>`, and `javascript:` "links" may not be parsed at all. → A "backlink" that isn't a true `<a href>` is worthless for SEO discovery. Verify the actual markup, not just the visible text.

### Site-reputation abuse (parasite SEO) (Source A)

Third-party content hosted on a strong domain *primarily to borrow that domain's ranking* is a violation — e.g. guest content placed only to rank on the host's authority, with no genuine value to the host's readers. **Not** a violation: genuine editorial/op-eds, wire/PR services, real UGC forums, correctly-handled affiliate links. → Our guest posts must genuinely serve the host's readers, not just rent its DA. If the only reason for a placement is "this domain is strong," it's parasite SEO and we don't do it.

### User-generated spam (Source A)

Spammy forum posts, profile spam, and comment spam are a spam category the **host site** gets penalized for. This is precisely why forums moderate, nofollow, and ban: they are actively fighting the exact tactic the "free backlinks" lists teach. Mass posting links into communities harms the community *and* gets your links deleted (and your accounts banned), which destroys the placements you spent time on.

### Machine-generated / scaled abuse (Source A)

Automated link creation and mass low-value page generation are violations. → This rules out the "9000 profile-creation sites," "1,352 forum-submission sites," and "200+ list" approaches as primary tactics. Those lists are a *sourcing pool* to hand-pick a few relevant, active communities — never a submission run.

---

## How penalties actually happen

Two mechanisms, both real, both worth fearing for a money site.

### Algorithmic devaluation / demotion

Google's core ranking and spam systems (SpamBrain and successors) detect unnatural link patterns automatically and continuously. The usual outcome is **not** a notification — it's silent: the manipulative links are *neutralized* (pass no credit) or the page/site is *demoted*. You often can't tell the difference between "links ignored" and "site demoted" without careful diagnosis. The patterns that trigger this are the ones `campaign-planning.md` is built to avoid: anchor over-optimization (exact-match spike), unnatural velocity (burst of links to a page that never attracted any), low-quality/irrelevant link clusters, and footprints shared across many sites (the PBN signature).

### Manual actions

A human reviewer at Google assesses the site and applies a **manual action**, which *does* appear in Google Search Console ("Manual Actions" report). For links, the typical labels are "Unnatural links to your site" (and historically "...impacting only this site"). Consequences range from devaluing specific links to demoting or deindexing the site. Recovery requires *cleaning up* the bad links (removal or `disavow`) and filing a **reconsideration request** — a slow, uncertain process that can take weeks and may not fully restore rankings.

The asymmetry is the whole argument: building manipulative links is fast and cheap; recovering from a manual action is slow, uncertain, and can cost a real business months of revenue. That asymmetry is why money sites stay conservative.

---

## Disclosure — FTC-style obligations for paid/sponsored placements

Separate from Google policy, there is an advertising-disclosure obligation. In the US the FTC requires that **material connections** (payment, free product, affiliation) behind an endorsement be **clearly and conspicuously disclosed**. The EU/FR equivalents (and platform rules) point the same way: sponsored content must be identifiable as such. This is law/regulation, not just SEO best practice.

Practical rules this skill follows:
- **A paid or sponsored placement is disclosed as such** — to the reader (a visible "Sponsored"/"Partenaire" label or equivalent) *and* to Google (`rel="sponsored"`). The two obligations are independent and we satisfy both.
- **Gifted product in exchange for coverage** is a material connection: disclose it, and the resulting link is `nofollow`/`sponsored`, never followed-for-ranking.
- **Affiliate / referral links** (including any tracking/referral param you append to product URLs when placed as affiliate/referral) are handled correctly: affiliate links don't pass ranking credit and should be qualified; where a placement is an affiliate/referral relationship, it's disclosed per the platform's rules.
- **We never ask a publisher to hide a paid relationship**, drop the `sponsored` attribute "for SEO," or label sponsored content as editorial. Asking a publisher to do that makes us the source of *their* policy violation.

Undisclosed-but-paid is the intersection of an FTC problem and a Google problem. We don't operate there.

---

## Money-site protection — why real businesses stay conservative

This is the load-bearing distinction of the whole skill. A revenue-bearing business is a **real business with revenue, inventory, customers, and a brand**. A product/tool page on a third-party platform is a listing that can be rebuilt, renamed, or relaunched with little cost. These are not the same risk class, and they don't get the same link mix.

Why money sites are conservative by default:

1. **The downside is existential, not cosmetic.** A manual action or algorithmic demotion on an e-commerce site means lost sales during the months-long recovery. For a tool page, a demotion is an inconvenience.
2. **Recovery is slow and uncertain.** Disavow + reconsideration can take weeks and may not restore prior rankings. A revenue business cannot gamble its primary acquisition channel on a fast-link shortcut.
3. **Brand reputation compounds the SEO risk.** A brand caught with spammy links or undisclosed paid placements damages trust with customers, suppliers, and the press — harm that outlives any ranking change.
4. **The asymmetry is unforgiving.** The time saved by aggressive tactics is small; the time lost to a penalty is large. The expected value is negative for any property you can't afford to lose.

So: **money sites get mostly tier-1 editorial links, near-zero exact-match anchors, slow steady velocity, and only a small slice of genuine community tier-2** (for traffic, not ranking). Tool/product pages can absorb more tier-2 — because it's *genuine on-topic developer-community participation*, the audience actually lives there, and the stakes are lower. "More tier-2 for a tool page" still means hand-built, real-participation links — never bulk, never automated, never the things in the next section.

When the user asks for something aggressive on a money site, the response is to name the boundary, explain the asymmetry, and propose the conservative tier-1 variant that gets the same goal without betting the business.

---

## Honest truths we don't let the listicles overwrite

The source articles are full of recycled claims that are simply wrong in 2026. We state the truth instead:

- **DA/DR is not a Google signal.** Domain Authority (Moz) and Domain Rating (Ahrefs) are third-party metrics. Useful as a *rough triage heuristic*, never as ground truth or a goal. The listicles' DA columns are recycled and self-contradictory (same site shown as DA 55 and 59 on one page). We chase relevance and real traffic, not a DR number.
- **Forum / profile / directory links are mostly traffic & brand, not ranking.** Honest sources concede these have "little-to-no" direct SEO value and are mostly nofollow/UGC now. Their real value is referral traffic, brand visibility, and profile diversity. We count them as such — never as equity.
- **"These lists are dofollow" is unreliable.** One source labels *every* entry "DOFOLLOW," including reddit.com and quora.com, which are nofollow. Always re-inspect the `rel` attribute on the actual page before relying on a link (this is what `qualification.md` enforces).
- **Raw traffic is not a confirmed ranking factor.** Don't plan as if sending traffic to a page ranks it. Traffic is a goal in itself, not a ranking lever.
- **Reciprocal links and affiliate links don't pass ranking credit** the way the lists imply — and excessive reciprocal exchange is named link spam.

Being honest about these protects the user from spending effort (and risk budget) on tactics that don't do what the listicles claim.

---

## WHAT WE WON'T BUILD OR DO

Drawing the line clearly. Regardless of property or how much a client wants it, this skill does not build, recommend, or assist with:

- **Undisclosed paid *followed* links.** Buying or selling links that pass ranking credit without `rel="sponsored"`/`rel="nofollow"` and without disclosure. This is the single clearest Google link-spam violation and an FTC problem at once. (Paid placements that are correctly qualified *and* disclosed are fine.)
- **Mass / automated forum, profile, comment, or directory spam.** No submission runs against "9000 profile sites," no bots posting links into forums or comments, no programmatic profile creation. Tier-2 is hand-built genuine participation only.
- **Private Blog Networks (PBNs).** Building or buying into a network of sites that exist to link to the property. Named as expired-domain abuse / link spam; high penalty risk; never recommended for a real property.
- **Expired-domain abuse.** Buying expired/aged domains to repurpose their authority for links. Same category, same answer: no.
- **Link schemes and link exchanges.** Reciprocal "you link me, I link you" at scale, three-way exchange rings, or any "link in exchange for goods/services/free product" arrangement that passes followed credit.
- **Buying followed links** from crowd-marketing or guest-post marketplaces where the deliverable is a *followed* link sold for ranking. (Their nofollow/sponsored, disclosed inventory may occasionally be a legitimate *advertising* buy — but that's an ad, not a ranking link, and it's planned and labeled as such.)
- **Site-reputation abuse / parasite SEO.** Placing content on a strong host purely to borrow its ranking, with no genuine value to the host's readers.
- **Anchor over-optimization.** Engineering a high share of exact-match commercial anchors. We keep them rare by design.
- **Asking publishers to violate their own policies.** No requests to strip `sponsored`/`nofollow` "for SEO," relabel sponsored content as editorial, or hide a paid relationship.
- **Spammy automated content for links.** Generating low-value pages or AI slop whose only purpose is to host or attract links. (Genuine assets route through a prose-humanization pass and exist to serve readers.)

When a request lands in this territory, the response is to explain the boundary, name the specific Google policy or law it crosses, and propose the white-hat variant that reaches the same goal defensibly. There is almost always a legitimate version of the objective that doesn't carry the risk.

---

## When in doubt, three questions

Before planning or building any link:

1. **Would the linking site's editor, if they fully understood the arrangement, be comfortable with it?** If the link only works because they don't know the full picture, it's not a clean link.
2. **Would this link survive a Google reviewer reading it?** If you'd want to hide it during a manual review, that's the signal.
3. **Would I do this to the money site?** If a tactic is too risky for a revenue-bearing property, be honest about why you're considering it for any property. (The answer can legitimately be "yes, because it's genuine participation and the stakes are lower" — but make the reasoning explicit.)

These aren't tests of whether you'd get caught. They're tests of legitimacy. Legitimate link building survives scrutiny — from the publisher, from Google, and from the brand's own standards. The capability is rarely the question; the legitimacy is.
