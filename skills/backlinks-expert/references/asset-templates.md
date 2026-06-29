# Asset Templates — Ready-to-Adapt, Per Channel × Language

The discovery and strategy modes decide *where* a link goes; this file decides *what gets posted there*. These are scaffolds, not fill-in-the-blanks-and-ship. Every one of them is built around the same non-negotiables:

- **The link is earned, not dropped.** Each template carries genuine value before it carries a link. A post that helps no one is spam regardless of how the anchor is worded — and Google names "forum posts with optimized links" and "low-value content created to manipulate links" as link spam explicitly.
- **The anchor matches the property profile.** Branded + naked URL dominate; exact-match is rare. Pull the exact funnel URL and seed anchor mix from `property-profiles.md` before adapting any template here.
- **Product/tool links carry your tracking/referral param.** Every one, where a tracking/referral param applies. A clean link forfeits attribution.
- **Disclosure where paid or sponsored.** If a placement is paid, the link is `rel="sponsored"` and the post says so. No undisclosed paid dofollow, ever.

> **Run the prose through a prose-humanization pass before posting (AI-detection-safe).** This appears under each template as a one-line reminder. A prose-humanization skill owns the doctrine for making text read human and pass AI detectors — this file does not duplicate it, it routes to it. Adapt the template, then humanize, then post.

Placeholders use `{{double-braces}}`. Anything in `[square brackets]` is an authoring note, delete it before posting. Domains like `example.com` and `platform.example.com/your-tool` are placeholders for your real funnel URLs.

---

## 1. Forum post (contextual, value-first)

**When:** you've already earned standing on the forum (≈5–10 genuinely helpful, link-free replies first; read the rules; one link max per reply). The link belongs only when it actually answers the question. This is a **traffic/brand** play — most forums are nofollow/UGC now — not a ranking play.

### EN

```
[Reply to a real thread where {{property}} is genuinely the best answer — do not start a thread just to drop this.]

{{Direct, specific answer to the asker's actual problem, 2–4 sentences. Show you read the thread.}}

For {{the specific sub-problem}}, I've been using {{branded anchor}} — {{one concrete sentence on how it solves THIS person's issue}}. {{funnel URL}}

{{Optional: one caveat or limitation, so it reads like real experience, not a pitch.}}
```

Filled (a developer tool, dev forum):

```
You can get the merchant prices without rendering the whole page — the site serves them
from an internal JSON endpoint, so a headless browser is overkill here.

If you'd rather not maintain the request/session logic yourself, [Brand]'s scraper
handles the proxy rotation and pagination for you:
https://platform.example.com/your-tool

Heads-up: the currency depends on a query param, so set your region or you'll get mixed currencies.
```

> Run the prose through a prose-humanization pass before posting (AI-detection-safe).

### FR

```
[Répondre à un fil réel où {{property}} est vraiment la meilleure réponse — ne pas créer un sujet juste pour poser le lien.]

{{Réponse directe et précise au problème réellement posé, 2–4 phrases. Montrer qu'on a lu le fil.}}

Pour {{le sous-problème précis}}, j'utilise {{ancre brandée}} — {{une phrase concrète sur la résolution DE CE problème}}. {{URL de funnel}}

{{Optionnel : une limite ou un bémol, pour que ça sonne comme du vécu et pas comme un argumentaire.}}
```

Filled (a wine e-commerce money site, FR wine forum — lien = trafic/notoriété, nofollow assumé) :

```
Pour un Loire à offrir sans se ruiner, un Vouvray demi-sec tient très bien quelques années et
passe sur la plupart des tables.

Côté cavistes en ligne j'ai eu une bonne expérience avec [Marque] sur ce type de cuvées :
example.com

Après, ça dépend du budget — au-delà de 25-30 € tu montes vite en gamme sur les Montlouis aussi.
```

> Faire relire la prose par un skill de humanisation avant publication (sûr face à la détection IA).

---

## 2. Profile bio (community / dev platform / directory account)

**When:** setting up a profile on a platform where a profile link is normal (GitHub, dev.to, SitePoint, an SEO community, a trade directory). Brand-presence play. One link, in the website field or bio, no keyword stuffing.

### EN

```
{{One-line who-you-are, real and specific}}. {{What you build / sell, in plain terms}}.
{{Naked URL or branded anchor}}

[Website field: {{funnel URL}}]
```

Filled (a brand/lead-gen hub, dev community):

```
I build web-scraping and MCP tooling, plus pricing-intelligence content. Writeups and free studies
at yourbrand.com.

[Website field: https://yourbrand.com]
```

Filled (a developer tool author profile / GitHub):

```
Maintainer of scraping + MCP tools. Data tools for pricing and market intelligence:
https://platform.example.com/your-tool
```

> Run the prose through a prose-humanization pass before posting (AI-detection-safe).

### FR

```
{{Qui je suis en une ligne, réel et précis}}. {{Ce que je construis / vends, en clair}}.
{{URL nue ou ancre brandée}}

[Champ site web : {{URL de funnel}}]
```

Filled (a wine e-commerce money site, annuaire / communauté FR) :

```
Caviste en ligne, sélection de vins de vignerons. Boutique : example.com

[Champ site web : https://example.com]
```

> Faire relire la prose par un skill de humanisation avant publication (sûr face à la détection IA).

---

## 3. Directory entry (listing description)

**When:** a legitimate, on-niche directory (trade association, vertical directory, dev-tools directory, MCP directory). Skip low-quality bulk-submission directories — Google names "low-quality directory links" as spam. For a specific marketplace/directory channel, **delegate to a directory/marketplace-distribution skill**.

### EN

```
Title: {{Property name}} — {{5–8 word descriptor, no keyword stuffing}}

Description: {{2–3 sentences: what it does, who it's for, what makes it specific. Concrete, no superlatives.}}

URL: {{funnel URL}}
Category: {{the genuinely correct category}}
```

Filled (a market-intelligence money site, trade directory):

```
Title: [Brand] — market intelligence & import support

Description: Pricing and market analysis built on multiple data sources, with a dedicated
import-support service for trade buyers. For importers, specialists and collectors who need
defensible pricing data.

URL: https://example.com
Category: Trade / market data
```

> Run the prose through a prose-humanization pass before posting (AI-detection-safe).

### FR

```
Titre : {{Nom de la propriété}} — {{descripteur de 5–8 mots, sans bourrage de mots-clés}}

Description : {{2–3 phrases : ce que c'est, pour qui, ce qui le distingue. Concret, sans superlatifs.}}

URL : {{URL de funnel}}
Catégorie : {{la catégorie réellement exacte}}
```

Filled (a wine e-commerce money site, annuaire de cavistes) :

```
Titre : [Marque] — caviste en ligne, vins de vignerons

Description : Boutique de vins en ligne avec une sélection de cuvées de vignerons indépendants,
de la Loire au Rhône. Pour les amateurs et les acheteurs cadeaux qui cherchent autre chose que
la grande distribution.

URL : https://example.com
Catégorie : Vin / caviste en ligne
```

> Faire relire la prose par un skill de humanisation avant publication (sûr face à la détection IA).

---

## 4. Guest-post pitch + outline

**When:** tier-1 editorial — the cleanest play. Pitch a publication whose readers are genuine prospects. The post must serve **their** readers (content that only borrows the host's authority is "site reputation abuse" under Google). One natural, non-optimized contextual link to your property inside genuinely useful content.

### EN — pitch email

```
Subject: Guest post idea for {{publication}}: {{specific working title}}

Hi {{editor first name}},

I read {{a specific recent piece on their site}} — {{one genuine, specific reaction to it}}.

I'd like to contribute a piece your readers would actually use: "{{working title}}".
It would cover:
- {{point 1 — concrete}}
- {{point 2 — concrete}}
- {{point 3 — original data / angle they can't get elsewhere}}

I'd reference {{property}} once where it's genuinely relevant ({{branded anchor}}), nothing
promotional beyond that. {{One line of credibility: who you are / why you can write this.}}

Want me to send a full draft, or would you prefer to shape the angle first?

{{Name}} — {{property}}
```

### EN — outline (attach or send on request)

```
Title: {{title}}
Audience: {{publication}}'s {{reader type}}
Angle: {{the one thing this piece does that competitors don't}}

1. {{Hook — a real problem the reader has}}
2. {{Section — actionable}}
3. {{Section — original data / case / numbers}}  ← this is what earns the link and the share
4. {{Section — actionable}}
5. {{Takeaway}}

Link plan: one contextual link to {{funnel URL}} in section {{N}}, anchor "{{branded or descriptive anchor}}".
[If the placement is paid/sponsored: disclose it, and the link is rel="sponsored".]
```

Filled link plan (a developer tool, dev publication):
`one contextual link to https://platform.example.com/your-tool in section 3, anchor "a data-extraction tool".`

> Run the prose through a prose-humanization pass before posting (AI-detection-safe).

### FR — pitch email

```
Objet : Idée d'article invité pour {{publication}} : {{titre de travail précis}}

Bonjour {{prénom de l'éditeur}},

J'ai lu {{un article récent et précis de leur site}} — {{une réaction sincère et précise}}.

J'aimerais proposer un article réellement utile à vos lecteurs : « {{titre de travail}} ».
Il couvrirait :
- {{point 1 — concret}}
- {{point 2 — concret}}
- {{point 3 — donnée originale / angle introuvable ailleurs}}

J'y citerais {{propriété}} une fois, là où c'est vraiment pertinent ({{ancre brandée}}), rien de
promotionnel au-delà. {{Une ligne de crédibilité : qui je suis / pourquoi je peux l'écrire.}}

Je vous envoie un brouillon complet, ou préférez-vous d'abord cadrer l'angle ?

{{Nom}} — {{propriété}}
```

Filled link plan (a wine money site, presse vin FR) :
`un lien contextuel vers example.com en section {{N}}, ancre « [Marque] ». [Si placement payé/sponsorisé : le divulguer, lien en rel="sponsored".]`

> Faire relire la prose par un skill de humanisation avant publication (sûr face à la détection IA).

---

## 5. Niche-edit insertion sentence

**When:** an existing, relevant, already-indexed article (yours or a partner's, or a placement an editor agreed to) gets one new sentence with a contextual link. The sentence must read as if it was always there and add real information — not a bolted-on plug. If the placement is paid, it's `rel="sponsored"` and disclosed.

### EN

```
[Insert into a paragraph that already discusses {{the topic}}. The sentence must add value on its own.]

{{Genuine, on-topic sentence that earns its place}}, {{branded or descriptive anchor →
funnel URL}}, {{which clause completes the thought naturally}}.
```

Filled (a brand/lead-gen hub, in an article about price monitoring):

```
Most teams underestimate how often retailer prices change intraday, which is why a scheduled
scrape beats a one-off pull — [Brand]'s pricing studies break down the refresh cadence by
category if you want the numbers behind that.
```

Filled (a developer tool, in a scraping tutorial):

```
If you'd rather not rebuild session handling every time the site rotates its tokens, a maintained
scraper already does it, so you can point it at a query and get clean rows back.
```
[Anchor "a maintained scraper" → `https://platform.example.com/your-tool`]

> Run the prose through a prose-humanization pass before posting (AI-detection-safe).

### FR

```
[Insérer dans un paragraphe qui parle déjà de {{le sujet}}. La phrase doit apporter de la valeur en soi.]

{{Phrase sincère et dans le sujet qui mérite sa place}}, {{ancre brandée ou descriptive →
URL de funnel}}, {{proposition qui complète l'idée naturellement}}.
```

Filled (a wine money site, dans un article sur les accords mets-vins) :

```
Sur un plateau de fromages de chèvre, un blanc sec de Loire reste la valeur sûre — [Marque]
en propose plusieurs autour de 15 €, ce qui évite de sortir l'artillerie lourde pour un apéro.
```

> Faire relire la prose par un skill de humanisation avant publication (sûr face à la détection IA).

---

## 6. Reddit / Quora answer (Q&A)

**When:** answering a real question where your property is genuinely the best (or one of the best) answers. **These links are nofollow** — the value is referral traffic, brand visibility and demand signal, **not** link equity. Lead with a complete answer that stands on its own without the link; disclose your affiliation. Bad-faith self-promo gets removed and damages the brand.

### EN

```
[Answer the question fully FIRST. The link is a footnote to a complete answer, never the answer itself.]

{{Complete, genuinely useful answer to the actual question — give away the real method, 1–3 short paragraphs.}}

(Disclosure: I build {{property}}, so take this with that in mind.) If you don't want to wire it up
yourself, {{branded anchor}} does exactly this: {{funnel URL}} — but the manual approach above works fine too.
```

Filled (a developer tool, r/webscraping or Quora):

```
The site exposes the merchant offers through an internal JSON endpoint, so you don't need a
headless browser at all — find the XHR call in DevTools, replay it with your region's query param,
and you'll get structured offers back directly. Rotate residential proxies because they rate-limit
by IP fairly aggressively.

(Disclosure: I build scraping tools, so take this with that in mind.) If you'd rather not maintain
the proxy/session layer, this does exactly that:
https://platform.example.com/your-tool — but the DevTools route above is free.
```

> Run the prose through a prose-humanization pass before posting (AI-detection-safe).

### FR

```
[Répondre d'abord COMPLÈTEMENT à la question. Le lien est une note de bas de page d'une vraie réponse, jamais la réponse.]

{{Réponse complète et réellement utile à la question posée — donner la vraie méthode, 1–3 courts paragraphes.}}

(Transparence : je développe {{propriété}}, à prendre en compte.) Si tu ne veux pas tout monter
toi-même, {{ancre brandée}} fait exactement ça : {{URL de funnel}} — mais la méthode manuelle ci-dessus marche très bien aussi.
```

Filled (a market-intelligence money site, Quora business FR) :

```
Pour exporter du vin vers un nouveau marché, le point bloquant est rarement le produit lui-même
mais la conformité documentaire (étiquetage en langue locale, certificats sanitaires, droits
d'accise). Commence par identifier un importateur agréé : sans lui, le dédouanement coince.

(Transparence : je travaille avec [Marque], à prendre en compte.) On accompagne justement
ce type d'export : example.com — mais un bon transitaire spécialisé fait aussi l'affaire.
```

> Faire relire la prose par un skill de humanisation avant publication (sûr face à la détection IA).

---

## Localized template packs (KR / ES / PT / DE / AR / HI)

These are localization **starters**, not paste-and-ship copy. A canned translation posted verbatim across a market reads as duplicate/spam and gets removed — and a machine-translated sentence in a community where everyone is fluent is worse than no post at all. Localize idiomatically (idiom, register, the actual word a native uses for the thing), then run the result through a prose-humanization pass before posting. Scope is **per-market**: each pack covers only the channels the `target-database.md` seed actually supports for that market — no channel is invented to look complete. All the non-negotiables from the top of this file still hold: link earned not dropped, anchor pulled from `property-profiles.md`, product/tool links carry your tracking/referral param, money sites stay conservative with no exact-match anchors, paid placements disclosed.

### KR

Serves a **money site** (e.g. a local-market vertical — conservative) and the **developer-tool** side. Seed targets: dev → okky.kr (largest KR dev Q&A community), velog.io (dev publishing); vertical → in-market portals + trade/community media. Domestic blog platforms (blog.naver.com / tistory.com) are mostly nofollow → traffic only. Channels worth packing: dev Q&A/forum, dev profile/publishing bio, vertical portal/directory entry.

**Dev Q&A / forum (okky.kr)** — answer a real question, link only if it's the genuine fix.

```
{{질문에 대한 직접적이고 구체적인 답변 2~4문장. 글을 읽었다는 게 드러나게.}}

{{이 사람의 문제}}는 {{브랜드 앵커}}로 해결했습니다 — {{이 문제를 어떻게 푸는지 한 문장}}. {{funnel URL}}

{{선택: 한 가지 한계나 주의점 — 광고가 아니라 경험담으로 읽히게.}}
```

Filled (a developer tool, okky.kr):

```
이 사이트는 머천트 가격을 내부 JSON 엔드포인트로 내려주기 때문에 헤드리스 브라우저까지 띄울 필요가 없어요.
DevTools에서 XHR 요청을 찾아 지역 쿼리 파라미터를 붙여 재요청하면 정형 데이터가 바로 나옵니다.

세션·프록시 로직을 직접 유지하기 번거로우면 이 도구가 그 부분을 대신 처리합니다:
https://platform.example.com/your-tool

참고: IP 단위로 레이트 리밋이 꽤 빡세니 레지덴셜 프록시를 돌리는 게 안전합니다.
```

> 게시 전 humanization 스킬로 문장을 다듬으세요 (AI 탐지 대응).

**Dev profile / publishing bio (velog.io)** — brand presence, one link in the bio.

```
{{한 줄 자기소개 — 실제로 하는 일}}. 스크래핑/MCP 도구와 가격 인텔리전스 관련 글을 씁니다.
{{naked URL 또는 브랜드 앵커}}
```

Filled (a brand/lead-gen hub, velog 프로필):

```
웹 스크래핑·MCP 툴링과 가격 데이터를 다룹니다. 정리한 글과 무료 리서치는 yourbrand.com 에 있습니다.
```

> 게시 전 humanization 스킬로 문장을 다듬으세요 (AI 탐지 대응).

**Vertical portal / directory entry** — a money site: branded, value-first, no exact-match.

```
제목: {{프로퍼티명}} — {{5~8단어 설명, 키워드 남발 금지}}
설명: {{무엇을 하는지·누구를 위한 것인지 2~3문장. 구체적으로, 과장 없이.}}
URL: {{funnel URL}}
```

Filled (a market-intelligence money site):

```
제목: [Brand] — 시장 인텔리전스 및 수입 지원
설명: 여러 데이터 소스를 기반으로 한 가격·시장 분석 서비스입니다.
수입사·전문가·컬렉터를 위한 근거 있는 가격 데이터를 제공하며, 수입 절차를 함께 지원합니다.
URL: https://example.com
```

> 게시 전 humanization 스킬로 문장을 다듬으세요 (AI 탐지 대응).

### ES

Serves a **brand/lead-gen hub + developer tools** (dev) and a **vertical** money side (ES has real vertical forums). Seed targets: dev → mediavida.com/foro (active ES dev forum), foro.elhacker.net (security/dev); wine-style vertical → verema.com (top ES wine forum), foro.e-nologia.com (enology/trade). Channels: dev forum, vertical forum.

**Dev forum (mediavida, elhacker)** — value-first reply, one link max.

```
{{Respuesta directa y concreta al problema real, 2–4 frases. Que se note que has leído el hilo.}}

Para {{el subproblema}} yo tiro de {{ancla de marca}} — {{una frase de cómo resuelve ESTO}}. {{funnel URL}}

{{Opcional: una pega o límite, para que suene a experiencia y no a anuncio.}}
```

Filled (a developer tool, mediavida):

```
El sitio sirve los precios de las tiendas desde un endpoint JSON interno, así que montar un navegador
headless es pasarse: localiza la llamada XHR en las DevTools y reprodúcela con el parámetro de región.

Si no te apetece mantener tú la rotación de proxies y la sesión, esta herramienta ya lo hace por ti:
https://platform.example.com/your-tool

Aviso: limitan bastante por IP, así que usa proxies residenciales o te cortan enseguida.
```

> Pasa el texto por un skill de humanización antes de publicar (a prueba de detección de IA).

**Vertical forum (verema, e-nologia)** — referral/brand play, nofollow assumed; conservative for the money site.

```
{{Respuesta genuina al hilo, 2–4 frases.}}

{{Mención de marca natural, sin ancla exact-match}} — {{frase que aporta valor}}. {{naked URL}}
```

Filled (a wine money site, verema):

```
Para seguir la evolución de precios de un Borgoña en el mercado secundario, los datos de mercado
mayorista dan una foto mucho más fiable que el PVP de una sola tienda.

Nosotros trabajamos justamente ese ángulo de inteligencia de precios en [Marca]: example.com
— aunque para una botella suelta comparar un par de tiendas ya te orienta.
```

> Pasa el texto por un skill de humanización antes de publicar (a prueba de detección de IA).

### PT

Serves a **brand/lead-gen hub + developer tools** (dev, strong in BR). A wine-style **vertical is thin**: the seed found no link-friendly PT community for it — only institutional trade/event orgs, which are digital-PR/earned targets, not forums. So this pack is dev-forum first, plus a short PR-pitch note for the vertical.

**Dev forum / community (tabnews, casadodesenvolvedor, devmedia)** — value-first reply.

```
{{Resposta direta e concreta ao problema real, 2–4 frases. Mostre que leu o tópico.}}

Para {{o subproblema}} eu uso {{âncora de marca}} — {{uma frase de como resolve ISTO}}. {{funnel URL}}

{{Opcional: uma ressalva ou limite, pra soar como experiência e não anúncio.}}
```

Filled (a developer tool, tabnews.com.br):

```
O site entrega os preços das lojas por um endpoint JSON interno, então subir um navegador headless
é exagero: ache a chamada XHR no DevTools e repita com o parâmetro de região que vem dado estruturado.

Se não quiser manter a rotação de proxy e a sessão na mão, essa ferramenta já faz isso:
https://platform.example.com/your-tool

Aviso: o rate limit por IP é agressivo, então use proxies residenciais.
```

> Passe o texto por um skill de humanização antes de publicar (à prova de detecção de IA).

**Vertical — no forum pack (honest gap).** Route the vertical to the **guest-post / digital-PR pitch** (section 4 of this file), targeting institutional trade/event orgs as earned-media/news outlets, not forum drops. Don't manufacture a forum post into an institutional site — it won't land and there's no community to earn standing in.

### DE

Serves a **brand/lead-gen hub + developer tools** (dev/SEO) and a **vertical** money side (DE has real vertical forums). Seed targets: dev/SEO → forum.abakus-internet-marketing.de (top DE SEO forum), dev-community.de; wine-style vertical → dasweinforum.de (dedicated forum), forum.restaurant-ranglisten.de (sommelier/wine board). Channels: dev/SEO forum, vertical forum.

**Dev / SEO forum (abakus, dev-community.de)** — value-first reply.

```
{{Direkte, konkrete Antwort auf das echte Problem, 2–4 Sätze. Zeig, dass du den Thread gelesen hast.}}

Für {{das Teilproblem}} nutze ich {{Marken-Anker}} — {{ein Satz, wie es GENAU DAS löst}}. {{funnel URL}}

{{Optional: eine Einschränkung, damit es nach Erfahrung klingt, nicht nach Werbung.}}
```

Filled (a developer tool, abakus):

```
Die Seite liefert die Händlerpreise über einen internen JSON-Endpoint — ein Headless-Browser ist dafür
überflüssig. Den XHR-Call in den DevTools suchen und mit dem Region-Parameter erneut abschicken.

Wenn du die Proxy-Rotation und das Session-Handling nicht selbst pflegen willst, übernimmt das dieses Tool:
https://platform.example.com/your-tool

Hinweis: Das Rate-Limiting läuft pro IP recht streng, also Residential-Proxies einsetzen.
```

> Lass den Text vor dem Posten durch einen Humanisierungs-Skill laufen (sicher gegen KI-Erkennung).

**Vertical forum (dasweinforum, restaurant-ranglisten)** — referral/brand, nofollow assumed; conservative for the money site.

```
{{Echte, themenbezogene Antwort auf den Thread, 2–4 Sätze.}}

{{Natürliche Markennennung, kein Exact-Match-Anker}} — {{Satz, der Mehrwert bringt}}. {{naked URL}}
```

Filled (a wine money site, dasweinforum):

```
Wer die Preisentwicklung eines Bordeaux am Sekundärmarkt verfolgen will, fährt mit Marktdaten
deutlich verlässlicher als mit dem Ladenpreis eines einzelnen Händlers.

Genau diesen Blickwinkel auf Preisintelligenz bearbeiten wir bei [Marke]: example.com
— für eine einzelne Flasche reicht aber oft schon der Vergleich von zwei, drei Shops.
```

> Lass den Text vor dem Posten durch einen Humanisierungs-Skill laufen (sicher gegen KI-Erkennung).

### AR

**Thin market — kept deliberately minimal, and that's the honest read.** The seed found almost no genuine open AR dev/tech community (the historic forums weren't confirmed live), and the AR backlink-list SERP is dominated by paid sellers → **AVOID**. The one honest channel is **Q&A on ar.quora.com, which is nofollow** (traffic/brand only, never equity). Serves a **developer tool**. Lead with a complete answer; the link is a footnote; disclose affiliation.

**Q&A (ar.quora.com)** — nofollow, answer-first.

```
{{إجابة كاملة ومفيدة فعلاً عن السؤال المطروح — اشرح الطريقة الحقيقية، فقرة أو فقرتان.}}

(للشفافية: أنا من يطوّر {{الموقع}}.) إن لم ترغب في بناء ذلك بنفسك، فهذه الأداة تقوم بالمهمة: {{funnel URL}} —
لكن الطريقة اليدوية أعلاه تعمل بشكل جيد أيضاً.
```

Filled (a developer tool, ar.quora.com):

```
يوفّر الموقع أسعار المتاجر عبر نقطة JSON داخلية، فلا حاجة إلى متصفّح headless إطلاقاً: ابحث عن طلب
الـ XHR في أدوات المطوّر وأعد إرساله مع وسيط المنطقة لتحصل على بيانات منظَّمة مباشرة. استخدم بروكسي
سكني لأن الموقع يفرض حدوداً صارمة حسب الـ IP.

(للشفافية: أنا أطوّر أدوات استخراج بيانات.) وإن لم ترغب في صيانة طبقة البروكسي والجلسة بنفسك، فهذه الأداة تتولّى
ذلك: https://platform.example.com/your-tool — لكن طريقة DevTools أعلاه مجانية وتفي بالغرض.
```

> مرِّر النص عبر مهارة humanization قبل النشر (آمن ضد كشف الذكاء الاصطناعي).

### HI

**India is an English-language market.** The seed is explicit: India's quality dev/finance communities operate in English, "dofollow forums India" returns EN submission lists, and the Hindi-language community layer of value is essentially empty. **So the EN templates above (sections 1–6) apply directly for India targeting — use those, in English.** The only thing worth pinning here is one tiny dev-forum example on the real India community the seed names (developersindia.in), written in English because that's the community's language.

**Dev community (developersindia.in)** — English; identical doctrine to the EN forum template.

```
{{Direct answer to the asker's actual problem, 2–4 sentences.}}

For {{the sub-problem}}, I use {{branded anchor}} — {{one sentence on how it solves THIS}}. {{funnel URL}}
```

Filled (a developer tool, developersindia.in):

```
The site serves merchant prices from an internal JSON endpoint, so a headless browser is overkill —
grab the XHR call in DevTools and replay it with your region's query param for structured data.

If you'd rather not maintain the proxy/session layer, this tool handles it:
https://platform.example.com/your-tool — rotate residential proxies, they rate-limit by IP.
```

> Run the prose through a prose-humanization pass before posting (AI-detection-safe). For everything else India-related, use the EN packs above as-is.

---

## Quick adaptation checklist (run before posting any asset)

1. **Property loaded?** Pulled niche, funnel URL and seed anchor mix from `property-profiles.md`. Posture respected (money site = conservative, no exact-match, tiny tier-2 volume).
2. **Anchor right?** Branded or naked dominant; exact-match only if it reads naturally and the property allows it.
3. **Tracking param?** Product/tool URLs carry your tracking/referral param where one applies. No bare links that forfeit attribution.
4. **Value-first?** The post helps the reader even if you strip the link out. If not, it's spam — rewrite.
5. **Disclosure?** Paid/sponsored → said so, link is `rel="sponsored"`. Q&A self-promo → affiliation disclosed.
6. **Language match?** Asset language = target community language = landing-page language.
7. **Humanized?** Prose run through a prose-humanization pass (AI-detection-safe) as the last step before posting.
