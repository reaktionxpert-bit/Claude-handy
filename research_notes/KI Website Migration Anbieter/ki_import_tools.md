# AI tools for automatic website migration and recreation from a URL (as of Nov 2026)

**How this was researched:** I could only use web search. Every page fetch was blocked by the session's network allowlist, including 10web.io, repaint.com and hostinger.com (each returned ENOTFOUND). So **every fact below comes from search-result snippets or search-tool summaries, not from pages I read in full.** Most of the sources are vendor marketing or help pages. I found almost no independent user reviews, and I could not reach Reddit or Product Hunt in a useful way. Dates are given where the snippets showed them. Search date: 2026-11-19.

---

## 1. Which website builders / AI builders offer "import/clone/recreate from URL" with AI, and what exactly do they migrate (design, content, URLs/301s, SEO meta, blog/CMS), quality, price?

### Takeaway
Recreating a site from a URL with AI is now a standard feature in 2025–2026. 10Web, Hostinger AI Builder/Horizons, Wix (Harmony "Create from URL" and Wix Vibe), Framer (AI agents / "AI site migration"), GoDaddy Airo, Repaint, Same.new, Zarla, Relume (structure only), Elementor AI (one container or page at a time), Duda (content only) and Webflow Marketplace apps all offer some version of it. In nearly every case the tool copies the visible front end: layout, styles, text and images. Some also bring over blog or CMS items. **None of the sources I found says that URL structure, 301 redirects or SEO meta are transferred.** Redirects and SEO are left to the user. Vendors themselves describe the output as a starting point that needs manual cleanup.

### Cited Findings

**10Web (WordPress/Elementor-based AI builder)**
- Marketing claim: 10Web can recreate or redesign any existing website from a URL and gives you an editable copy — [10Web AI Website Builder](https://10web.io/ai-website-builder/) (snippet)
- The help center describes a page-by-page process. You paste the URL of one page (homepage, contact page and so on), and you have to recreate one page at a time. The output is a ready-to-customize WordPress template built with Elementor pro widgets — [10Web Help: AI Website Builder](https://help.10web.io/hc/en-us/articles/7952757255186-AI-Website-Builder-Fully-Automated-WordPress-Website-Creation-in-a-Few-Minutes); [help.10web.io](https://help.10web.io/hc/en-us/articles/4413393256210) (snippets; these help articles may be older)
- A newer flow called "Clone site from URL" on the homepage can clone any publicly accessible URL on any platform. The vendor says the agents rebuild the structure without copying the original code — [10Web blog: clone website with 10Web](https://10web.io/blog/clone-website-with-10web/) (snippet)
- Clone is one of four ways to start a site, next to prompt, Figma and redesign. A "cloning agent" recreates any page from a URL. Editing options are a "Simple Visual Editor" and an "Advanced AI Editor". I found no clear description of a chat co-pilot — [10Web for agencies](https://10web.io/ai-website-builder/for-agencies/) (snippet)
- A third-party tester copied a Wix site into WordPress/Elementor in under a minute. The tool "replicates the design of your existing website, rather than generating a brand new one" — summarized in the [Repaint 2026 builders guide](https://repaint.com/blog/best-ai-website-builders-2026) / [Tooltester AI builder test](https://www.tooltester.com/en/blog/ai-website-builder/) (snippet; the attribution between these two sources was not clear in the summary)
- Price: agency plans start "at $42.50/month for ten sites" according to one pricing page. Another tab lists billing transaction fees of 8% and 7% — [10Web pricing (agency tab)](https://10web.io/pricing-platform/?tab=agency) (snippet; the sources conflict, so verify)

**Hostinger AI Builder / Hostinger Horizons, "Website cloner"**
- The cloner reads a single page at a publicly accessible URL and produces a working version of it inside an AI project. It captures structure, styles and content as an editable project — [Hostinger blog: "Rebuilding a website just became as easy as copy-pasting a link"](https://www.hostinger.com/blog/?p=9754); [Hostinger website cloner](https://www.hostinger.com/ai-builder/website-cloner) (snippets)
- It copies public front-end content only. Backend, databases, user accounts, dynamic functionality and integrations are **not** copied. Results depend on how complex the original site is — [Hostinger Horizons website cloner](https://www.hostinger.com/horizons/website-cloner) (snippet)
- For Wix sources it reads layout, colors, typography, navigation, text and products — summarized in [Hostinger Wix-to-WordPress tutorial / cloner page](https://www.hostinger.com/tutorials/wix-to-wordpress/) (snippet)
- After cloning, you can edit copy, colors, images, layout and components by selecting elements or **by describing the change in the AI chat**. Chat edits use credits — [Hostinger website cloner](https://www.hostinger.com/ai-builder/website-cloner) (snippet)
- Price: available on all plans including the free trial, and you can start without a credit card. AI credits can be topped up. I saw no specific euro or dollar figure in the snippets — [Hostinger Horizons cloner](https://www.hostinger.com/horizons/website-cloner) (snippet). Launch date not found.
- Hostinger says to clone only sites you own or have permission to use — [Hostinger cloner](https://www.hostinger.com/horizons/website-cloner) (snippet)

**Wix: Harmony editor (AI agent "Aria") and Wix Vibe**
- Wix Harmony, a hybrid drag-and-drop editor with the AI agent Aria, was released in January 2026. It offers "Create from URL": Aria scans the source site's structure, content and visual style and generates a new Harmony site that you keep customizing — [Wix Help: Harmony – creating a site from a URL](https://support.wix.com/en/article/wix-harmony-editor-creating-a-site-from-a-url) (snippet; the January 2026 release date comes from the search summary)
- Wix says you cannot migrate an existing Wix Editor site to Harmony, or move a Harmony site to the Wix Editor or Studio — [Wix Help](https://support.wix.com/en/article/wix-harmony-editor-creating-a-site-from-a-url); [Wix Dev: About Wix Harmony](https://dev.wix.com/docs/develop-websites-sdk/get-started/overview/about-wix-harmony) (snippets)
- Wix Vibe can also start from a URL and "recreates the look and feel… matching the page's design, text, and images as closely as possible" — [Wix Help: Wix Vibe – creating a site from a design or URL](https://support.wix.com/en/article/wix-vibe-creating-a-site-from-a-design-or-url) (snippet)
- I found no Wix statement on whether Create from URL carries over URLs, metadata or redirects. Wix's general SEO guidance says you must set up redirects yourself if URLs change — [Wix SEO Hub: site migration fundamentals](https://www.wix.com/seo/learn/resource/site-migrations-fundamentals) (snippet)
- Wix also has a developer-facing Site Import API for moving a store or site from another platform into Wix. A full import typically takes 15–60 minutes — [Wix Dev: Site Import](https://dev.wix.com/docs/api-reference/account-level/sites/skills/site-import) (snippet)

**Framer**
- Framer's own glossary describes "AI site migration": an agent recreates pages, structure, styles **and CMS content** from an existing site, an export or a reference — [Framer dictionary: AI Site Migration](https://www.framer.com/dictionary/ai-site-migration) (snippet)
- Framer's agents page uses this example prompt: "Here's a URL of our current site. Rebuild its structure and visual style in Framer, using our existing brand colors." — [Framer Agents](https://www.framer.com/agents?via=framax) (snippet)
- Framer launched AI agents for website creation and editing in June 2026 — [eCommerceNews AU](https://ecommercenews.com.au/story/framer-launches-ai-agents-for-website-creation-editing); [CMOtech](https://cmotech.news/story/framer-launches-ai-agents-for-website-creation-editing) (snippets; the URL-import details were not in the snippet)
- Conflict: a competitor's comparison page (Revamp) says Framer does not take a URL natively and that sites are rebuilt by hand. This source is biased — [Revamp vs Framer](https://revamp-73e.pages.dev/compare/revamp-vs-framer/) (snippet; it may predate the June 2026 agents)
- Older or other routes: the "Webflow Import" plugin in the Framer Marketplace — [Framer Marketplace: Webflow Import](https://www.framer.com/marketplace/plugins/webflow-import/); CSV import of Webflow CMS collections — [Framer guide: Webflow to Framer](https://www.framer.com/guides/webflow-to-framer-step-by-step/); a Chrome extension that copies elements from WP or Webflow one by one — [Framer University](https://framer.university/blog/how-to-move-your-site-from-wordpress-to-framer) (snippets)
- Framer's SEO migration guide recommends keeping the platform change separate from URL and content changes. That is manual guidance, not an automated feature — [Framer: Webflow to Framer SEO](https://www.framer.com/guides/webflow-to-framer-seo/) (snippet)
- A community hackathon project called "Blueprint AI" (third-party, not a Framer feature) takes a URL, maps CMS collections and design tokens, and produces a rebuild plan — [Framer community submission](https://www.framer.com/community/contests/agents-hackathon/submissions/5fcb74Y1Q7s6pYE9tgKJD7/) (snippet)

**Webflow**
- Webflow has no native AI URL import in the sources I found. Webflow's own help says no automated conversion exists from Framer to Webflow. Pages are rebuilt by hand, and CMS content comes in via CSV — [Webflow Help: Migrate from Framer](https://help.webflow.com/hc/en-us/articles/48246102456083-Migrate-your-site-from-Framer-to-Webflow) (snippet)
- "Website Importer" is a third-party app in the Webflow Marketplace. You give it a URL and it analyzes the site and rebuilds it in Webflow, whatever the source stack (WordPress, React, Vue, Next.js) — [DEV Community launch post](https://dev.to/elvisans/we-just-launched-website-importer-on-the-webflow-marketplace-57e1) (snippet; developer's own claim, date unknown)
- "WP to Webflow" is a free Marketplace app that moves WordPress posts, categories and tags into the Webflow CMS. You enter the live WP URL, and it needs a CMS plan — [Webflow Apps: WP to Webflow](https://webflow.com/apps/detail/wp-to-webflow) (snippet)
- A do-it-yourself AI route: in a case study, an agency moved about 1,000 WP posts into Webflow through the Webflow MCP plus an AI agent, which created missing fields as it went (June 2025) — [Magnet.co](https://magnet.co/articles/moving-1-000-posts-from-wordpress-to-webflow-with-mcp) (snippet)

**Repaint (AI-only builder, redesign/migration focus)**
- You paste a public URL and describe the changes. It imports text, images and pages, including blog collections. You don't need code, hosting or admin access. It can rebuild custom-coded sites too — [Repaint: Website redesign](https://repaint.com/website-redesign); [Repaint: AI website migration](https://repaint.com/features/ai-website-migration); [Repaint: modernize outdated site](https://repaint.com/blog/how-to-modernize-an-outdated-website-with-ai) (snippets, vendor claims)
- Edits happen by chatting with the AI ("Redesign your website by chatting with AI") — [Repaint](https://repaint.com/website-redesign) (snippet title)
- Limits: animations are the main thing it struggles to import. Sites with hundreds of pages are imported in stages. Repaint itself notes that "some [tools] import your full site, while others skim your homepage and improvise the rest" — [Repaint blog: best AI redesign tools 2026](https://repaint.com/blog/best-ai-website-redesign-tools-2026) (snippet; Repaint's own blog, so biased)
- Price: Premium is $25/month ($20/month billed annually) and adds a custom domain, removes branding and raises limits. There is a 14-day trial. Large redesigns may need extra credits, and refunds are generally not given once the AI allowance is used — [Repaint WordPress redesign page](https://repaint.com/features/wordpress-website-redesign); [Gappsy](https://www.gappsy.com/tools/repaint/) (snippets). Capterra lists "$24/year flat", which conflicts with this and is probably outdated — [Capterra](https://www.capterra.com/p/10036783/Repaint/reviews/)
- I found no independent user reviews with ratings — [Gappsy](https://www.gappsy.com/tools/repaint/) ("not yet verified") (snippet)

**GoDaddy Airo AI Builder**
- You paste a URL, and Airo builds a new site as a separate project. The current site is not touched — [GoDaddy Airo: How to rebuild a website without starting over](https://airo-builder.godaddy.com/discover/learn/how-to-rebuild-a-website-without-starting-over) (snippet)
- A third-party review says the rebuild is a fresh design, not a copy, and that integrations such as payments and stores do not carry over — [Figment: GoDaddy website builder](https://figment.so/blog/godaddy-website-builder) (snippet)

**Same.new / Lovable / Bolt / v0 (AI app builders)**
- Same.new copies a site's layout, styling and visual structure from a URL and generates React/Next.js code that you then change through chat. One source says it also infers a data model (React + Supabase) — [bestaitools: Same](https://www.bestaitools.com/tool/same/); [aitoolery: Same.new review](https://aitoolery.pages.dev/reviews/coding-assistants/same-new) (snippets, low-quality aggregators)
- I found no source confirming a built-in URL-cloning feature in Lovable. "Open Lovable" is an unrelated open-source tool by Mendable (the Firecrawl team) that turns any URL into a React app — [OpenReplay blog](https://blog.openreplay.com/clone-website-react-app-open-lovable/) (snippet)
- Bolt is described as a full-stack browser IDE (StackBlitz WebContainers), not a dedicated cloner. One aggregator notes that edits made through chat prompts can be fragile — [directory comparison Bolt vs Same](https://directory-website01.pages.dev/comparisons/bolt-vs-same-dev) (snippet, low-quality source)
- The output is code (React/Next.js), not a CMS a marketing user can edit. Any SEO or redirect handling would have to be built by hand (inference from the above).

**Duda (agency/white-label builder)**
- An "Import Content" button pulls text, images and the business name from any existing site into the content library (Editor 2.0 only). It does not clone layouts — [Duda product update](https://www.duda.co/product-updates/import-content-from-any-site-to-speed-up-your-build) (snippet)
- Duda's 2025 year-in-review says you can import content from an existing site or file and then refine or rewrite it with AI — [Duda year in review 2025](https://www.duda.co/product-updates/year-in-review-2025) (snippet)
- WordPress blog posts come in through an RSS feed URL. Duda's agency page mentions a dedicated migration tool plus optional managed manual migration — [Duda blog: migrate WP blog](https://blog.duda.co/migrate-wordpress-blog-duda-how-to); [Duda agency migration page](https://agency.duda.co/website-migration); [migration.duda.co](https://migration.duda.co) (snippets; parts may be older)
- A third-party guide says formatting, galleries and embeds usually need manual cleanup — [eSEOspace: WordPress to Duda](https://eseospace.com/blog/migrate-wordpress-to-duda/) (snippet; the page carries an implausible date, so treat with caution)

**Relume (sitemap/wireframe planning for Webflow/Figma/React)**
- You enter a URL in the dashboard and Relume rebuilds the page structure as a sitemap in its Site Builder (up to 50 pages). Optionally it uses titles and meta descriptions as page prompts. Its own crawler is used, not sitemap.xml — [Relume docs: Import an existing site](https://resources.relume.io/resources/docs/import-an-existing-site-into-the-relume-site-builder); [Relume community](https://community.relume.io/oh-you-mean-when-you-enter-the-url-and-it-builds-a-sitemap-based-on-the-existing-website-LsbKdTkjQxml) (snippets; the feature launched in May 2024 — [Relume what's new](https://www.relume.io/whats-new/may-2024-component-day))
- Users report it "falls a bit short… especially if the existing site has any kind of repeated content like a blog" and that imports fail on some sites. It is best for a few pages — [Relume community thread](https://community.relume.io/import-website-via-url-nRQfCCrppJFd) (snippet)
- It migrates structure and wireframes, not the finished design or content.

**Elementor AI**
- The AI Site Planner creates a new sitemap and wireframe. It does not import from a URL. Entering an existing WP domain only checks which plugins the site needs — [Elementor Help: Site Planner](https://elementor.com/help/build-an-entire-website-from-scratch-with-elementor-ai/) (snippet)
- A separate feature generates containers from a reference URL. It works only on "traditional" (non-React) sites and reproduces best when the source is built with Elementor — [Elementor Help: create containers based on an existing page](https://elementor.com/help/use-ai-to-create-containers-based-on-an-existing-page) (snippet)

**Other and newer entrants found**
- Zarla offers a free AI redesign or import of an existing website, including from Wix — [Zarla: Website import](https://www.zarla.com/features/website-import) (snippet)
- Revamp (pages.dev) does AI redesign from a URL with code export. It positions itself against Wix and Framer — [Revamp vs Wix](https://revamp-73e.pages.dev/compare/revamp-vs-wix/) (snippet)
- Fimo.ai has an experimental `fimo migrate <url>` CLI pipeline (init → inspect → apply → refine) that produces an "agent-ready migration draft". Its changelog entry is dated 2026-08-25, and the feature is labeled experimental — [Fimo docs: migration overview](https://fimo.ai/docs/migration/overview); [Fimo changelog 2026-08-25](https://fimo.ai/docs/changelog/2026-08-25-migration) (snippets)
- FocusReactive (an agency) describes AI migration of Webflow, Framer and static sites into Sanity or Payload CMS from a single URL — [FocusReactive blog](https://focusreactive.com/blog/ai-website-migration-moving-webflow-framer-and-static-sites-to-sanity-and-payload-from-a-single-url/) (snippet)
- Odoo's AI website builder can import an existing site — [SmartTek: Odoo AI website builder import](https://smarttek.solutions/blog/odoo-ai-website-builder-import-existing-site/) (snippet title only)
- Durable: I found no documented URL-import feature. Sources describe generating a new site in about 30 seconds — [Durable](https://durable.com); [SoftwareTestingHelp review](https://www.softwaretestinghelp.com/durable-ai-website-builder-review/) (snippets)
- B12: there is a guide on "how to migrate your existing website to an AI website builder", but I could not confirm a specific URL-import tool — [B12 resource center](https://www.b12.io/resource-center/ai-how-to-guides/how-to-migrate-your-existing-website-to-an-ai-website-builder/) (snippet)

### Inferences
- In 2026 the technical step "paste a URL, get an editable AI rebuild" is a commodity. Hostinger offers it even on its free trial, and Wix, Framer, 10Web and GoDaddy all ship it. A €300 migration therefore cannot be justified by the cloning step alone. It would have to be justified by what these tools leave out: a full multi-page migration, 1:1 URL mapping and 301 redirects, transfer of meta titles, descriptions and schema, migration of blog and case-study CMS items into structured collections, and quality assurance by a human.
- Several tools work page by page (the 10Web help docs, the Hostinger cloner reading "a single web page", Elementor containers). Others skim the homepage and improvise the rest (Repaint's own characterization of competitors). Fidelity on multi-page sites is the main weak point.
- SEO preservation (redirects, meta, canonicals) is the clearest gap. No vendor snippet claimed to automate it.

### Gaps
- Full page content could not be checked because fetching was blocked. There are no hands-on quality tests apart from one tester snippet on 10Web.
- I could not access user sentiment on Reddit or Product Hunt in this session.
- Squarespace: I found no information on a URL-import or AI rebuild feature (not covered by the searches).
- Exact pricing for Hostinger credits, Wix Harmony and Framer agents is not in the snippets.
- Whether Framer's AI site migration preserves slugs or redirects is unknown.
- Launch dates for the Hostinger cloner and the 10Web "Clone site from URL" flow were not found.

---

## 2. Do any of them combine migration with chat-based AI editing afterwards ("live changes per KI")?

### Takeaway
Yes, several already do. Hostinger (cloner, then AI chat edits), Wix Harmony (Create from URL, then the Aria agent), Framer (URL rebuild through agents, which also edit the site), Repaint (URL import, then "redesign by chatting with AI") and Same.new (clone, then chat edits on the code) all combine the two. 10Web pairs cloning with an "Advanced AI Editor". So migration followed by AI-chat editing is not a differentiator in itself.

### Cited Findings
- Hostinger: after cloning, you can edit "by selecting elements directly or describing the change in AI chat", and chat edits use credits — [Hostinger website cloner](https://www.hostinger.com/ai-builder/website-cloner) (snippet)
- Wix Harmony combines drag-and-drop with the AI agent Aria, and a site created from a URL is generated and then further customized there — [Wix Help: Harmony creating a site from a URL](https://support.wix.com/en/article/wix-harmony-editor-creating-a-site-from-a-url); [Wix Studio forum: Harmony & Aria](https://forum.wixstudio.com/t/wix-harmony-aria/76193) (snippets)
- Framer: "AI agents for designing, updating, and improving sites", with a URL-rebuild example prompt. Agents launched in June 2026 — [Framer Agents](https://www.framer.com/agents?via=framax); [CMOtech](https://cmotech.news/story/framer-launches-ai-agents-for-website-creation-editing) (snippets)
- Repaint: "Redesign your website by chatting with AI" after URL import — [Repaint website redesign](https://repaint.com/website-redesign) (snippet)
- Same.new generates React code from a URL that "you then change through chat" — [bestaitools: Same](https://www.bestaitools.com/tool/same/) (snippet)
- 10Web: clone, redesign and Figma agents, plus an "Advanced AI Editor". I could not confirm a chat co-pilot — [10Web for agencies](https://10web.io/ai-website-builder/for-agencies/) (snippet)
- Duda: import content, then refine or rewrite it with AI. This is content-level AI, not full chat site editing — [Duda year in review 2025](https://www.duda.co/product-updates/year-in-review-2025) (snippet)

### Inferences
- The idea's core loop (migrate, then edit live with AI) is already available from large and inexpensive players (Hostinger, Wix, Framer). For the agency builder to differ, it would need things those tools lack: agency-specific blocks, SEO/GEO built into the editing loop, and a migration that guarantees SEO equity (redirects and meta), not just a visual clone.
- Hostinger and Repaint bill AI chat edits as credits. A "live edits via AI" promise usually comes with usage-based cost for the vendor, which a pricing model has to account for.

### Gaps
- I found no independent reviews of how reliable chat editing is on cloned sites. One aggregator says chat-prompt edits can be "fragile" for Bolt/Same-type tools — [directory comparison](https://directory-website01.pages.dev/comparisons/bolt-vs-same-dev) (low-quality source).

---

## 3. Is any of them positioned specifically for agencies' OWN websites (not client sites)? Is there any agency-vertical builder at all?

### Takeaway
I found **no** builder that pairs migration with AI editing and is positioned for agencies' own websites. Agency-facing products (10Web Agency/Reseller, Duda, Brizy) are white-label tools for building **client** sites. A few AI builders have landing pages or templates for "marketing agency websites" (Landingsite.ai, Readdy, Frontdesk, Yola, 10Web templates). These are generic builders with an agency vertical page, not agency-specific block libraries, and none mentions importing the agency's existing site. I found nothing for Shopify or e-commerce agencies' own sites.

### Cited Findings
- 10Web Agency plans and Reseller Suite: Agency Core includes 20 websites, a branded dashboard and builder, client billing via Stripe or PayPal, and the Redesign, Clone and Figma agents. Agency Pro covers 50+ sites. This is aimed at agencies, freelancers and MSPs reselling to clients — [10Web for agencies](https://10web.io/ai-website-builder/for-agencies/); [10Web Help: Agency Pro Plan](https://help.10web.io/hc/en-us/articles/13002165862930-Agency-Pro-Plan) (snippets)
- 10Web announced a white-label reseller dashboard for MSPs and agencies on 2025-11-05 (about a year old) — [10Web press release](https://10web.io/press-kit/press-release-white-label-website-builder-reseller-dashboard/) (snippet)
- Duda positions migration ("move your sites to Duda and cut maintenance costs") for agencies moving **client portfolios**. Example: a webinar on "migrating 3,000 websites" — [migration.duda.co](https://migration.duda.co); [Duda webinar](https://www.duda.co/webinars/migrating-3000-websites) (snippets)
- Landingsite.ai has an "AI website builder for agencies" page pitching an AI "that understands marketing agencies", with a white-label FAQ. It is ambiguous whether this targets the agency's own site or client sites — [Landingsite.ai](https://www.landingsite.ai/marketing-agency-website-builder) (snippet)
- Readdy offers "Website Builder for Marketing Agency" pages and digital-marketing templates — [Readdy](https://readdy.ai/website-builder/marketing-agency-website) (snippet)
- Frontdesk: an "AI website builder for agencies" page that generates pages, copy, design and SEO from a prompt — [Frontdesk](https://www.myaifrontdesk.com/ai-website-builder/agencies) (snippet)
- Yola agency templates — [Yola](https://yolacms.yolasite.com/website-builder/digital-marketing-agency); 10Web "digital marketing agency" template — [10Web templates](https://10web.io/website-templates/digital-marketing-agency); Brizy white-label for agencies — [Brizy](https://www.brizy.io/solutions-for-agencies) (snippets)
- A search for Shopify-agency, SEO and GEO tools returned only agencies **selling** Shopify migration and GEO/AEO services to clients, not a builder for the agency's own site — e.g. [1Digital](https://www.1digitalagency.com/shopify-custom-design); [eSEOspace: top Shopify migration experts 2026](https://eseospace.com/blog/top-shopify-migration-experts-2026/) (snippets)

### Inferences
- The specific positioning in the idea (a builder only for agencies' own sites, with agency blocks such as case studies, services, team, partner badges like Shopify Partner, and GEO) seems unoccupied as of these searches. The adjacent products are horizontal AI builders with agency landing pages, and white-label "agency" tools for client work.
- One risk: the horizontal players already give agencies a free or cheap "paste URL, get an editable rebuild, edit with chat" path (Hostinger, Wix, Framer agents). The vertical product has to win on agency-specific depth and SEO/GEO, not on the migration mechanism.

### Gaps
- Search coverage of small or niche tools (for example Product Hunt launches in 2026) is incomplete. I could not browse Product Hunt.
- I could not confirm Landingsite.ai's exact positioning or whether it has import features.

---

## 4. Reference: SEO-relevant migration elements (URLs/301s, meta, CMS) across tools

### Takeaway
Of the URL-import tools, only Framer (CMS content, per its glossary), Repaint (blog collections) and Relume (titles and meta descriptions used as page prompts) say anything about content beyond the visual page. None claims automatic 301 redirect mapping or URL-slug preservation. For WP-to-Webflow there are separate CMS-only importers. SEO-safe migration is still mostly manual.

### Cited Findings
- Framer: AI site migration covers "pages, structure, styles, and CMS content" — [Framer dictionary](https://www.framer.com/dictionary/ai-site-migration) (snippet)
- Repaint imports "pages, including groups of pages like blog posts" — [Repaint AI website migration](https://repaint.com/features/ai-website-migration) (snippet)
- Relume can optionally include title and meta description as page prompts during URL import — [Relume docs](https://resources.relume.io/resources/docs/import-an-existing-site-into-the-relume-site-builder) (snippet)
- Hostinger copies the front end only. Backend, integrations and dynamic functions are excluded — [Hostinger cloner](https://www.hostinger.com/horizons/website-cloner) (snippet)
- Wix: "if your URLs are changing… you will need to set up the redirects" (general guidance, not specific to Harmony) — [Wix SEO Hub](https://www.wix.com/seo/learn/resource/site-migrations-fundamentals) (snippet)
- Shopify migration buyer guides list URL mapping, 301 redirect architecture, canonical tags, sitemaps and GEO/AEO as the criteria that matter — [eSEOspace 2026](https://eseospace.com/blog/top-shopify-migration-experts-2026/) (snippet). One agency says "most migration failures aren't data failures — they're SEO failures" — [1Digital migration services](https://www.1digitalagency.com/shopify-migration-services/) (snippet)

### Inferences
- An automated migration that also guarantees redirects, keeps meta, transfers structured CMS content and checks the result for GEO would address a real, documented gap. This is the most defensible part of the €300 migration offer.

### Gaps
- None of the snippets showed whether any tool automatically creates a redirect map or keeps slugs. Confirming this would need hands-on testing or full documentation pages, which were blocked here.
