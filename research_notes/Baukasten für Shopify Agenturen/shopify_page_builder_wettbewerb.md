# Wettbewerb: Shopify Page Builder & Section-/Komponenten-Bibliotheken (Fokus Agenturen) — Stand Nov 2026

> **Method note (read first):** In this research session, direct page fetches were blocked (apps.shopify.com and all other hosts could not be reached via WebFetch, because the session's network allowlist did not include them). Everything below comes from **web search result summaries**, which show snippets from the cited pages. Each URL is the page a given snippet came from, as best it could be attributed. Most sources are **2026 comparison blogs, and many are vendor- or affiliate-owned**. section.store, pagefly.io, gempages.net, zipify.com, instant.so, fudge.ai, getlandra, ecomwize and similar sites sell competing products. Prices and ratings in these sources often contradict each other; contradictions are flagged inline. **Before using any number in a final report, check it against the live Shopify App Store listing (apps.shopify.com/<app>) and the vendor pricing page.**

## 1. Which page builders and section libraries exist for Shopify? (Landscape, positioning, ratings, market leaders)

### Takeaway
The market splits into three layers:
- **(a) Full app-based page builders:** PageFly, GemPages, EComposer, Shogun, Replo, Instant, Zipify, Foxify. They have their own editor and usually their own runtime.
- **(b) Theme-section libraries:** Section Store (formerly "Section Factory"), Kava, Puco, Oxify, Flexi, Section Kit and others. They install native Liquid sections into the theme and usually charge one-time per section.
- **(c) Shopify's native stack:** Horizon themes with nested theme blocks, plus AI block generation in the Theme Editor and Sidekick. This layer is increasingly eating into (a) and (b).

PageFly is clearly the leader by installs. PageFly, GemPages and EComposer lead by review volume, each with around 4.9 stars. Replo and Instant are the premium tools for design-driven DTC brands and agencies, with far fewer reviews.

### Cited Findings
**Ratings / review counts (snapshots from secondary sources; not live-verified):**
- PageFly 4.9/5 with 5,686 reviews; GemPages 4.9/5 with 3,484 reviews; Replo 4.7/5 with 171 reviews (all as of June 2026, per a roundup) — [fudge.ai: Best Shopify Page Builders 2026](https://www.fudge.ai/blog/best-shopify-page-builders/); [fudge.ai: PageFly alternatives](https://www.fudge.ai/blog/pagefly-alternatives/) (fudge.ai sells a competing AI builder)
- Typical rating range across 2026 roundups: GemPages, EComposer and PageFly around 4.9; Shogun around 4.7–4.8; Replo around 4.7 — [instant.so: 9 Best Page Builders 2026](https://instant.so/blog/9-best-page-builders-for-shopify-in-2026); [appstoreresearch.com](https://appstoreresearch.com/blog/best-shopify-page-builder-apps)
- EComposer: 4.9 stars with about 3,500 reviews, according to several sources — [section.store: GemPages alternatives](https://section.store/blogs/store-design-optimisation/gempages-alternatives); [inso.codes: PageFly alternatives](https://www.inso.codes/apps/alternatives/pagefly-landing-page-builder-alternatives)
- Instant: 4.9 with 309 reviews, or 338 reviews depending on the source — [futureproofmarketer: Instant review 2026](https://futureproofmarketer.com/blog/instant-review); [zekaiwork: Instant.so review](https://zekaiwork.com/ai-tools/instant-so/)
- Foxify: 4.8 with 326 reviews (one comparison) — [aliapopups: 14 best Shopify page builders](https://www.aliapopups.com/blog/best-shopify-page-builders)
- Zipify Pages (now "Zipify Landing Page Builder"): 4.6–4.7 — [zipify.com comparison](https://zipify.com/choosing-the-shopify-landing-page-builder-tools-that-are-right-for-your-business/); [tinyseo](https://tinyseo.com/best-shopify-apps/page-builders/)
- Section Store (App Store slug `section-factory`, so "Section Factory" is the old name of the same app): 4.9 stars with 3,000+ reviews. The current listing title is "Section Store: Theme Sections – Sections, Cart Drawer, Bundles & Quantity Breaks, AI Pages", with 700+ sections — [apps.shopify.com/section-factory reviews](https://apps.shopify.com/section-factory/reviews?ratings%5B%5D=1&page=1); [section.store](https://section.store/); [inso.codes Section Store review](https://www.inso.codes/apps/reviews/section-store-review)
- One operator survey warns that GemPages, Zipify, Shogun and Instant don't have enough reviews for robust comparison, so their ratings should be read as directional only — [appstoreresearch.com](https://appstoreresearch.com/blog/best-shopify-page-builder-apps)

**Install counts / market share:**
- StoreInspect studied 508,680 Shopify stores (published April 2026). 21,148 stores use PageFly, which is 4.16% of all stores studied, and PageFly accounts for **71.3% of detected users in the page builder category** — [storeinspect.com: Shopify App Market Share](https://storeinspect.com/blog/shopify-app-market-share)
- EComposer is installed on 28,025 Shopify stores as of Sept 2026, per StoreCensus. StoreCensus uses a different method from StoreInspect, so the two figures cannot be compared directly — [storecensus.com: EComposer](https://www.storecensus.com/shopify-stores-using/ecomposer)
- Around 6.8% of active Shopify stores run some page builder (unsourced claim) — [webtonic.io](https://www.webtonic.io/blog/best-shopify-development-tools)
- Context: Store Leads counted 3.06M Shopify stores in August 2026 — [mobiloud CMS market share](https://www.mobiloud.com/blog/cms-market-share/)

**Positioning (consensus across 2026 roundups):**
- PageFly: the "safe veteran", known for templates, integrations and pixel-precise layout control. GemPages: funnels, template variety and conversion tooling; one source counts about 400 templates vs. 120 for PageFly. EComposer: the budget/feature-value pick, with a smaller community. Shogun: analytics, enterprise and multi-store, and cited as "winning on exit". Replo: aimed at agencies and design teams, with analytics and split testing on every plan — [fudge.ai PageFly alternatives](https://www.fudge.ai/blog/pagefly-alternatives/); [earnifyhub PageFly vs GemPages](https://earnifyhub.com/blog/dropshipping/pagefly-vs-gempages-shopify); [section.store PageFly alternatives](https://section.store/blogs/store-design-optimisation/pagefly-alternatives)
- Instant: main differentiator is a Figma plugin with direct copy-paste from Figma into the editor. It outputs native Shopify Liquid instead of a JS overlay, so pages survive uninstall — [futureproofmarketer](https://futureproofmarketer.com/blog/instant-review); [hedrick.io Figma to Shopify](https://hedrick.io/post/figma-to-shopify-guide)
- Zipify: the usual choice for split testing at a low entry price; every paid plan includes page testing — [zipify.com](https://zipify.com/choosing-the-shopify-landing-page-builder-tools-that-are-right-for-your-business/)
- Foxify: a simple, lightweight editor with AI layout features — [aliapopups](https://www.aliapopups.com/blog/best-shopify-page-builders)
- Other section libraries in the App Store:
  - Oxify Section: 100+ sections, "Dawn, Horizon & all themes"
  - Kava Sections: 120+ sections at $14.99 per section, one-time payment
  - Puco Sections: 200+ sections, 33+ categories, one-time purchase, free plan
  - Flexi — Sections: 40+ presets, metafield support, sections maintained monthly
  - Section Kit: free sections plus one-time premium sections
  - Also: Sectionly, OT Section, Section Star

  Sources: [Oxify](https://apps.shopify.com/ia-sections-store); [Kava](https://apps.shopify.com/kava-sections-page-builder); [Puco](https://apps.shopify.com/pusher-sections-builder); [Flexi](https://apps.shopify.com/flexi-theme-section); [Section Kit](https://apps.shopify.com/sectionkit?locale=pl); [Sectionly](https://apps.shopify.com/rihify-section-library); [OT Section](https://apps.shopify.com/ot-theme-sections-store-page-builder); [Section Star](https://apps.shopify.com/sections-ai)

### Inferences
- PageFly's install dominance (about 71% of detected builder users), together with roughly 4.9-star ratings from GemPages and EComposer, means the merchant self-service market is saturated and competes on price.
- The section-library layer is crowded with near-identical "100–700 sections, one-time $5–$54" offers. Almost none of them address agencies directly, as opposed to merchants. That leaves room for an agency-focused, brand-consistent component kit.

### Gaps
- No live App Store numbers could be fetched (network block). Ratings and review counts for Shogun, GemPages (current), EComposer and Foxify could not be verified as of November 2026.
- I found no product called "Sections Hub", and "Booster" (Booster Theme / Booster apps) did not come up as a section library. I found no GemPages install count.

## 2. What does each cost, and what agency / partner / white-label / handoff offers exist?

### Takeaway
Almost every builder charges **per store** (a Shopify app subscription is tied to one shop). None of the vendors I researched has a real **white-label** or **per-agency multi-client licence**. Agency monetisation runs through **affiliate/referral commissions** (PageFly 50%/30%, GemPages 40%/25%), free development-store use, multi-store discounts (GemPages) or enterprise multi-store plans (Shogun Advanced, PageFly Enterprise, Replo Custom). Section libraries sell one-time per-section licences per store.

### Cited Findings
**Prices (2026, USD/month, conflicting where noted):**
- **PageFly** (prices checked Oct 13, 2026 by one comparison). App Store plans are Free, Builder, Accelerate and Enterprise; the website also shows Optimize and Power.
  - Free: 1 published slot, 10 AI credits per month
  - Builder: $24 for 5 published slots, plus $5 per 5 extra slots
  - Optimize: $39 (A/B tests, funnels, AI Translator)
  - Accelerate: $99 or $990/year (unlimited pages, per one source)
  - Power: $199 (unlimited pages, more AI credits)
  - Enterprise: Scale $299, Dominate $499, Empire $999 for multi-store and Plus brands
  - Older plan names ("Pay as you go", "Unlimited" at $18) are outdated.

  Sources: [inso.codes PageFly review](https://www.inso.codes/apps/reviews/pagefly-landing-page-builder-review); [trygodmode PageFly 2026](https://www.trygodmode.com/blog/who-should-use-pagefly-2026); [dodropshipping PageFly review](https://dodropshipping.com/pagefly-review/); [fudge.ai PageFly vs Replo](https://www.fudge.ai/blog/pagefly-vs-replo/)
- **GemPages:** Free (1 published page); Build $29; Optimize $59; Enterprise $199. All paid plans include unlimited published pages. One source says plans are monthly only, with no annual option for new customers (unverified third-party claim) — [inso.codes GemPages pricing](https://www.inso.codes/apps/pricing/gempages-landing-page-builder-pricing); [getlandra: Landing Page Builders for Agencies](https://www.getlandra.com/blog/landing-page-builder-for-agencies); [capterra GemPages](https://www.capterra.com/p/228368/GemPages/)
- **EComposer:** a free tier that publishes 1 page. Paid entry is $19 or $25 for 15 pages, depending on the source. Mid tier is $39 or $49 for 50 pages; one source lists $129 for unlimited — [section.store GemPages alternatives](https://section.store/blogs/store-design-optimisation/gempages-alternatives); [inso.codes](https://www.inso.codes/apps/alternatives/pagefly-landing-page-builder-alternatives)
- **Shogun:**
  - Draft Mode: $0 (cannot publish)
  - Build: $39 for 25 published pages
  - Grow: $199, or $249 in some sources (disputed)
  - Advanced: $499, which includes multi-store content syncing and custom CMS collections
  - Annual billing: Build $31, Grow $159, Advanced $399
  - A/B testing is a separate add-on, from free (1 active test) up to $499 per month

  Sources: [blinto Shogun review](https://blinto.co/app-reviews/shogun-shopify-page-builder-review/); [section.store Shogun alternatives](https://section.store/blogs/store-design-optimisation/shogun-alternatives); [dropinblog Shogun review](https://dropinblog.com/blog/shogun-page-builder-review/); [attnagency Shogun review](https://www.attnagency.com/blog/shogun-shopify-review)
- **Replo:**
  - Starter: $119 per month, or $99 effective with annual billing; one July 2026 snapshot lists 400 AI chats and 15 published items
  - Pro: $599 per month, or $499 annual, with unlimited items
  - Custom / Enterprise: custom credit and visitor limits, volume pricing and implementation support
  - Additional store: $99 per month (one source)
  - Free plan: limited live publishing
  - An outlier "Growth $199" plan appears in one source only
  - Billing now meters **agent credits** and **visitor sessions**

  Sources: [fudge.ai Replo alternatives](https://www.fudge.ai/blog/replo-alternatives/); [smartcreatorhub Replo review](https://www.smartcreatorhub.blog/en/replo-review); [ecomwize vs Replo](https://ecomwize.io/blog/ecomwize-vs-replo); [buildyourstore.ai Replo review](https://www.buildyourstore.ai/blog/replo-review-and-alternatives/)
- **Instant:** $39 / $99 / $249 per month, or $31 / $79 / $199 billed yearly (20% off). The free plan is disputed: the App Store listing reportedly limits it to development stores, while Instant's blog describes a free tier with 1 page, 1 section and 1 blog post. Instant also sells a **done-for-you landing page for a flat $499, delivered in 2 days** — [futureproofmarketer](https://futureproofmarketer.com/blog/instant-review); [instant.so: landing page agency](https://instant.so/blog/landing-page-agency); [zekaiwork](https://zekaiwork.com/ai-tools/instant-so/)
- **Zipify Pages:** $19 Starter (5 landing pages, 1 product page, 1 blog article, 1 custom homepage, 1 split test); $39 Basic; $99 Advanced (unlimited). The free plan may be limited to development and partner stores (sources conflict) — [zipify.com](https://zipify.com/choosing-the-shopify-landing-page-builder-tools-that-are-right-for-your-business/); [shopthemedetector](https://shopthemedetector.com/blog/shopify-page-builders/)
- **Foxify:** pricing is very inconsistent across sources ("from $1", or "free plan, paid from $19"); 150 AI credits per month — [aliapopups](https://www.aliapopups.com/blog/best-shopify-page-builders); [outfy](https://www.outfy.com/blog/best-page-builder-apps-shopify/)
- **Section Store:** free app with one-time per-section purchases. The vendor quotes $9–19 per premium section; other sources quote $5 or $9–$54. "Section Store Plus" costs $15 per month flat, with no revenue share and a 14-day trial — [section.store/pages/plus](https://section.store/pages/plus); [inso.codes Section Store review](https://www.inso.codes/apps/reviews/section-store-review); [cartcoders](https://cartcoders.com/blog/shopify-apps/top-shopify-section-store-apps/)

**Agency / partner / white-label / handoff:**
- **GemPages:** each subscription is tied to one store. Multi-store discounts are 10% off the 2nd store, 15% the 3rd, 20% the 4th and 25% from the 5th onward. **Subscriptions cannot be transferred to another Shopify user**, so a client needs their own subscription to keep editing. A theme-partner offer gives 6 months free on Standard for partner themes. The affiliate programme pays 40% on the first transaction and 25% recurring for the account's lifetime (single-source; verify) — [getlandra: Landing Page Builders for Agencies](https://www.getlandra.com/blog/landing-page-builder-for-agencies); [gempages.net: Shopify Partner Program](https://gempages.net/blogs/shopify/shopify-partner-program)
- **PageFly:** affiliate/agency partner programme paying **50% of the first paid month and 30% of later months** (after Shopify's fee deduction). Commission ends if the merchant uninstalls or closes the store. Partners get a dashboard showing clicks, installs and commission, paid monthly via PayPal. Agencies can use the top plan free on development stores (blog post from 2020, may be outdated). PageFly runs a partner directory of independent agencies, where clients pay the agency directly. **I found no white-label offer** — [PageFly affiliate agreement](https://pagefly.io/pages/pagefly-affiliate-agreement); [partners.pagefly.io](https://partners.pagefly.io/register); [PageFly blog: make money via PageFly](https://pagefly.io/blogs/shopify/how-to-make-money-in-the-shopify-partner-program-through-pagefly-freelancers-agencies); [pagefly.io/pages/our-partners](https://pagefly.io/pages/our-partners); [xamplify PageFly partner program](https://xamplify.com/partner-programs/pagefly/)
- **Shogun:** Advanced at $499 is the multi-store/team plan with content syncing. **I found no agency partner, reseller or agency-pricing programme** in search results — [section.store Shogun alternatives](https://section.store/blogs/store-design-optimisation/shogun-alternatives); [blinto](https://blinto.co/app-reviews/shogun-shopify-page-builder-review/)
- **Replo:** no plan labelled "agency"; Pro and Custom serve agency needs. Replo is positioned as built for agencies and design teams — [fudge.ai Replo alternatives](https://www.fudge.ai/blog/replo-alternatives/); [ecomwize vs Replo](https://ecomwize.io/blog/ecomwize-vs-replo)
- **Instant:** a weak single source mentions an "Enterprise/Agency" plan for Plus stores and agencies, with no price found. Instant's own $499 done-for-you service competes directly with agencies — [instant.so landing page agency](https://instant.so/blog/landing-page-agency)
- **Shopify platform rules relevant to handoff:**
  - Agencies build "client transfer stores" and hand ownership to the client. Development stores cannot be transferred to clients or converted to live stores.
  - Collaborator accounts reach only the permissions granted, and do not count toward staff limits.
  - Collaborator access can be kept after transfer, but lapses after 90 days without a login.

  Sources: [shopify.dev: About stores](https://shopify.dev/docs/apps/build/stores); [shopify.dev: Collaborations](https://shopify.dev/docs/apps/build/stores/collaborations); [Shopify Help: client transfer stores](https://help.shopify.com/en/partners/manage-clients-stores/client-transfer-stores)

### Inferences
- Agencies today must either pass app subscriptions on to each client (per-store billing, non-transferable in GemPages' case) or build natively in the theme. **No vendor I found offers an agency-owned, reusable, brand-specific component library across clients with white-label.** This is the clearest whitespace for an agency "Baukasten".
- Pricing spreads widely: about $19–$29 entry (EComposer, Zipify, GemPages, PageFly) vs. $99–$599 (Replo, Instant upper tiers, Shogun Grow/Advanced). Section libraries sit at one-time $5–$54 per section or about $15 per month flat.

### Gaps
- Current official agency/partner pages for Shogun, Replo, EComposer, Instant and Foxify could not be fetched. Their partner or affiliate commission terms are unknown.
- I could not verify whether any vendor offers per-agency licences (one fee covering N client stores). None was found in search results.

## 3. What weaknesses do agencies and merchants complain about?

### Takeaway
The recurring complaints are:
- **lock-in and broken or disappearing pages after uninstall**
- **leftover code** (snippets, assets, settings_data entries)
- **extra JavaScript runtime and performance cost** (roughly 260–340 KB, unverified)
- **costly migrations off builders to native sections**
- **non-transferable per-store subscriptions**
- **generic template design**, where cheap section libraries sometimes don't work properly

Native-Liquid output (Instant, Section Store) is now marketed explicitly as the antidote.

### Cited Findings
- Uninstalling builders can leave code that clutters the theme and breaks layouts, and cleanup is manual — [bigeyedeers: PageFly vs Shogun](https://www.bigeyedeers.co.uk/pagefly-vs-shogun/)
- Builder apps leave snippet files, asset files and `config/settings_data.json` entries. The guide suggests searching snippets for builder prefixes before deleting anything; Shopify's help centre also warns that app code isn't automatically removed on uninstall — [kaspianfuad: leftover Shopify app code](https://kaspianfuad.com/blog/shopify-leftover-app-code/)
- Page builder apps inject their own rendering runtime. Estimates are about 340 KB of JS for PageFly and about 260–300 KB each for Shogun and GemPages. These figures are unsourced and unverified — [kaspianfuad: page builder alternatives](https://kaspianfuad.com/blog/shopify-page-builder-alternatives/); [coreppc](https://coreppc.com/shopify/shopify-landing-page-builder/)
- What happens to pages after cancelling is **contested**:
  - one blog says pages stay as frozen HTML that can't be edited
  - another says PageFly removes pages on uninstall and GemPages live pages can break
  - EComposer pages reportedly go away 48 hours after uninstall
  - Zipify pages stop working after cancel
  - Shogun is cited as "winning on exit" (pages remain)

  Sources: [kaspianfuad alternatives](https://kaspianfuad.com/blog/shopify-page-builder-alternatives/); [section.store AI store builders](https://section.store/blogs/store-design-optimisation/shopify-ai-store-builders); [section.store GemPages alternatives](https://section.store/blogs/store-design-optimisation/gempages-alternatives); [fudge.ai PageFly alternatives](https://www.fudge.ai/blog/pagefly-alternatives/)
- Individual App Store reviews: an uninstall that "bricked my site" (2023), and a 2020 reviewer saying uninstalling would "undo everything we made on PageFly" — [PageFly App Store reviews](https://apps.shopify.com/pagefly?page=21)
- Migration cost anecdote: 30 PageFly pages migrated to native theme sections took **4 weeks of developer time and $12k** of agency cost (unverified single data point from an interested party) — [kaspianfuad alternatives](https://kaspianfuad.com/blog/shopify-page-builder-alternatives/)
- Section Store complaints: "I bought 3 sections from them, 2 of which doesn't work!", and $9 per section seen as "a bit high". Section Store claims sections stay in the theme after uninstall because they are native .liquid files (vendor/affiliate claim) — [Section Store 1-star reviews](https://apps.shopify.com/section-factory/reviews?ratings%5B%5D=1&page=1); [inso.codes Section Store review](https://www.inso.codes/apps/reviews/section-store-review)
- GemPages works outside the Shopify admin (separate editor) — [earnifyhub](https://earnifyhub.com/blog/dropshipping/pagefly-vs-gempages-shopify). EComposer has a smaller community and fewer tutorials — [fudge.ai PageFly alternatives](https://www.fudge.ai/blog/pagefly-alternatives/)
- Replo's real cost can grow through usage overages (credits, visitors) and Theme Editor publishing limits — [ecomwize vs Replo](https://ecomwize.io/blog/ecomwize-vs-replo)

### Inferences
- An agency kit that outputs **native, theme-owned Liquid sections/blocks built on Horizon theme blocks, with no runtime JS and no lock-in**, while staying brand-consistent through design tokens or theme settings, directly addresses the top documented pain points.
- "Survives uninstall" and "no runtime" are already sales claims for Instant and Section Store, so they work as baseline expectations rather than differentiators.

### Gaps
- **I found no Reddit (r/shopify, r/ShopifyeCommerce) threads in search results**, so I have no direct agency voices from Reddit. G2 and Capterra review text was not retrieved.
- The JS payload figures and the uninstall behaviour have no independent measurement. They need a test-store benchmark.
- I found nothing specific about "lack of brand-consistent components" as an agency complaint. It is plausible but unsourced.

## 4. How has AI page generation changed the market in 2025–2026?

### Takeaway
AI is now standard in every builder (AI credits in PageFly, Foxify and Replo). Replo moved to an **agent-based AI Builder** with credit- and visitor-metered billing that can even host pages outside the Shopify theme. Most disruptive, **Shopify itself (Winter '26 Edition, Dec 10, 2025)** lets Sidekick and the Theme Editor generate theme blocks or sections and edit themes from natural language. This weakens simple section libraries and entry-level builders, but practitioners report about 80% visual accuracy and code-governance problems, which leaves room for curated, quality-controlled components.

### Cited Findings
- Shopify Winter '26 Edition ("RenAIssance") launched **December 10, 2025**. Sidekick can generate custom admin apps (Polaris + Admin GraphQL), make theme edits via natural language and generate custom blocks; some write-ups say "it generates theme sections" — [shopify.com/news Winter '26](https://www.shopify.com/news/winter-26-edition-renaissance); [nebulab Winter 2026](https://www.nebulab.com/blog/shopify-winter-2026-edition); [Shopify Community: Winter Editions 2026 highlights](https://community.shopify.com/t/winter-editions-2026-is-now-out-highlights-for-merchants/579120)
- Sidekick availability by plan is disputed. One source says custom apps are limited to Grow, Advanced and Plus; another says Sidekick is on all plans — [what.digital](https://what.digital/shopify-winter-edition-2026-new-features/); [coalitiontechnologies](https://coalitiontechnologies.com/blog/shopify-editions-winter-26)
- Theme Editor "Add block > Generate" only works in sections that accept theme blocks. One guide says it has worked across Theme Store themes with theme-block support since December 2025. Anatta says the output is a nested theme block, which needs a block-based theme such as Horizon. Horizon supports nesting up to 8 levels deep — [anatta.io: AI theme blocks](https://anatta.io/horizon/ai-theme-blocks/); [ecomm.design: customize theme with AI](https://ecomm.design/how-to-customize-shopify-theme/)
- Practitioner critique:
  - "Useful for scaffolding, unreliable for anything precise" — [anatta.io](https://anatta.io/horizon/ai-theme-blocks/)
  - Sidekick gets to about 80% visual accuracy fast, but produces isolated CSS/JS that doesn't follow existing patterns, so it needs governance — [digismoothie: Sidekick AI vibe coding](https://www.digismoothie.com/blog/sidekick-ai-vibe-coding)
  - No versioning or feature freeze for Sidekick — [Shopify Community](https://community.shopify.com/t/winter-editions-2026-is-now-out-highlights-for-merchants/579120)
- Summer '26 Edition reportedly shipped June 17, 2026; one source calls Horizon part of it. Dating is inconsistent and not verified against Shopify's release notes — [adsx: Summer '26 Edition](https://www.adsx.com/blog/shopify-summer-26-edition-horizons); [100xelevate Horizon review](https://100xelevate.com/insights/shopify-horizon-theme-review/)
- **Replo** now runs two product lines: the classic Theme Builder, which publishes into the Shopify theme, and an **AI Builder**. The AI Builder uses an agent workflow to generate pages from prompts, images and ad creative, can build before a store is connected, and in one description hosts pages on a subdomain. Billing is by agent credits plus visitor sessions. Funding: a $4.2M seed (Y Combinator, Figma Ventures, Guillermo Rauch), with total raised reported at $8.2M+; Tracxn shows only $125K, which looks incomplete. No 2026 round was found — [smartcreatorhub Replo review](https://www.smartcreatorhub.blog/en/replo-review); [fabric.so Replo review](https://fabric.so/comparison/replo-review); [tracxn Replo](https://tracxn.com/d/companies/replo/__UhqKXYhzsYQcLTIgT0GNIYxH9a9HOhAqogodJ0KYJts); [fudge.ai Replo alternatives](https://www.fudge.ai/blog/replo-alternatives/)
- PageFly plans scale by published pages **and monthly AI credits** (10 on Free) — [buildyourstore.ai PageFly review](https://www.buildyourstore.ai/blog/pagefly-review-and-alternatives/); [inso.codes PageFly review](https://www.inso.codes/apps/reviews/pagefly-landing-page-builder-review)
- Foxify: 150 AI credits per month — [aliapopups](https://www.aliapopups.com/blog/best-shopify-page-builders). Section Store now advertises "AI Pages" in its listing title — [apps.shopify.com/section-factory](https://apps.shopify.com/section-factory/reviews?ratings%5B%5D=1&page=1)
- New AI-native entrants positioned against classic builders: Fudge.ai, EcomWize ("AI agent vs agency-grade editor"), Landra — [fudge.ai compared](https://www.fudge.ai/blog/shopify-page-builders-compared/); [ecomwize vs Replo](https://ecomwize.io/blog/ecomwize-vs-replo); [getlandra Replo alternatives](https://www.getlandra.com/compare/replo-alternatives)
- Instant pairs AI with human experts in its $499, 2-day done-for-you pages, which is a direct substitute for agency landing-page work — [instant.so landing page agency](https://instant.so/blog/landing-page-agency)

### Inferences
- Commodity sections (hero, FAQ, testimonials) are becoming free to generate natively. Value is shifting to **curation, brand consistency, conversion-proven patterns, governance/QA and reusable cross-client systems**, which suits an agency kit.
- Building on **Horizon/theme blocks** is strategically necessary, since that is where Shopify's own AI generation and the theme editor are converging.
- Pricing is moving to usage-based models (AI credits, visitor sessions), which makes costs less predictable for agencies managing many client stores.

### Gaps
- I could not access the primary Shopify Editions page or changelog to confirm exact Sidekick/section-generation scope and plan availability.
- No GemPages AI-specific 2026 launch details were found (GemPages AI exists per roundups, but no primary source was retrieved).

## Appendix-style notes on DACH / German specifics (within scope of Q1–Q4)

### Takeaway
I found no reliable source on GDPR/DSGVO features, DPAs (AVV) or EU hosting for any Shopify page builder, and no German-language agency-focused competitor.

### Cited Findings
- The PageFly App Store listing is available in German locale (listing translation; this says nothing about German editor UI or support) — [apps.shopify.com/pagefly?locale=de](https://apps.shopify.com/pagefly?locale=de)
- PageFly's Optimize plan includes an "AI Translator", relevant for multilingual (e.g. DE/EN) stores — [inso.codes PageFly review](https://www.inso.codes/apps/reviews/pagefly-landing-page-builder-review)

### Inferences
- GDPR documentation (DPA, data residency, which third-party scripts a builder's runtime loads) is an underserved angle and a potential differentiator for a DACH-focused agency kit. Native Liquid with no external runtime also simplifies cookie-consent concerns.

### Gaps
- No sources found on DSGVO/AVV, server location, or German-language support for PageFly, GemPages, Shogun, Replo, EComposer or Instant. Check each vendor's privacy policy and DPA directly.
