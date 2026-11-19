# Websites von Shopify-/E-Commerce-Agenturen: gemeinsames Muster, Unterschiede, Bausteine für „Fokuspage“

**Methodik und Kennzeichnung (Stand 19.11.2026)**
- Zuerst gab es nur Websuche (Snippets). Nach der Netzwerkfreigabe habe ich **52 Agentur-Startseiten live abgerufen** (curl, bei JS-lastigen Seiten Playwright/Chromium), dazu 14 Sitemaps und 8 Unterseiten. Ausgewertet habe ich `<title>`, Meta-Description, H1–H3 in Seitenreihenfolge (als Näherung für die Sektionsreihenfolge), Navigations- und Header-Links, CTA-Texte, %-Kennzahlen und das CMS bzw. Hosting.
- **[live]** heißt: auf der live abgerufenen Seite am 19.11.2026 gesehen. **[Snippet]** heißt: nur aus Suchergebnis-Zusammenfassungen, nicht selbst geprüft.
- Die Häufigkeiten stammen aus einer **Keyword-Heuristik auf dem Startseiten-HTML** (inkl. Mega-Menü) und sind keine visuelle Einzelprüfung. Sie sind als grobe Größenordnung zu lesen. Seiten mit viel clientseitigem Rendering (shopnative, Moving Primates, Oskar Studio, AthariCommerce, Hyghstreet, 5pm) liefern wenig Text, ihre Werte sind also eher zu niedrig.
- Nicht auswertbar:
  - wemakewebsites.com liefert 403 (Bot-Schutz, auch mit Headless-Chrome).
  - finer.digital führt zu einem italienischen Finanz-Forschungsinstitut, ist also die falsche Domain. Die URL der Agentur „Finer Digital“ blieb unbekannt.
  - systra-studios.de war nicht erreichbar.
  - halbstark.de habe ich wegen des Webflow-Fokus als Generalist eingeordnet.

**Stichprobe**
- **A) DACH, Shopify-fokussiert (n=27):** Latori, Eshop Guide, tante-e, 14agency, Codext, Uplifts, NICCOS, Schaltwerk Digital, Shopfabrik, Neuzeitwerber (Shopify-Landingpage), digitalsprung, apoio, tzn Digital, 5pm (AT), Rankist (CH), Onlineshop Experts (CH), NETSHAKE, NextPercent, Oskar Studio, applepie, Hyghstreet, Kombinat, shopnative, ABxpert, Moving Primates (DE/AT), Acceleratiq, AthariCommerce.
- **B) International (n=8):** Eastside Co (UK), Swanky (UK/AU/FR), Charle (UK), Fuel Made (US), Anatta (US), Electric Eye (US), Ask Phill (NL), craftberry (EU).
- **C) Vergleichsgruppe DACH-Generalisten mit Shopify als einem von mehreren Systemen (n=17):** eBakery, ONEDOT, TechDivision, OPEN, 7thSENSE, TOWA, ECONSOR, Halbstark, Friendventure, BRANDUNG, Webstra, clickpuls, Ostend Digital, huks, arboro, 4TFM, Golden Web Age.
- Quellen für die Auswahl: [Dr. Web Vergleich (117 Anbieter)](https://www.drweb.de/shopify-agentur-vergleich/), [Golden Web Age Vergleich (25 Anbieter)](https://www.goldenwebage.de/shopify/shopify-agenturen-vergleich/), [OMR Reviews Shopify-Agenturen](https://omr.com/de/reviews/service-category/shopify-agencies), [wortfilter Top 25](https://wortfilter.de/shopify-agentur/), [Eastside Co Top-Agencies 2026](https://eastsideco.com/blog/top-shopify-and-shopify-plus-agencies-2026), [qikify EU-Liste](https://qikify.com/blogs/all-articles/best-shopify-agencies-in-eu) sowie die Websuche.

---

## 1. Was ist pro Agentur beobachtbar? (Stichprobe)

### Takeaway
Fast alle Shopify-fokussierten Agenturseiten in DACH folgen derselben Grammatik:
- Die H1 nennt „Shopify (Plus) Agentur“.
- Partner-Status, Kundenlogos, Case-Teaser mit %-KPIs, ein Leistungsblock (Setup/Neu, Migration, Plus/B2B, Optimierung/Betreuung), ein Prozess in 3–5 Schritten, Testimonials, Team, FAQ.
- Der zentrale CTA lautet „(kostenloses) Erstgespräch buchen/anfragen“, oft kombiniert mit einem Gratis-Audit/Check.

Unterschiede zeigen sich vor allem in Positionierung, Tonalität und Tiefe der Unterseiten, kaum in der Struktur.

### Cited Findings — DACH, Shopify-fokussiert (alle [live] auf der verlinkten Startseite, sofern nicht anders markiert)
- **Latori** – Title „Shopify Agentur: Offizieller Shopify Platinum Partner“, H1 „Shopify Agentur“.
  - Nav: Leistungen, Referenzen, Partners, Zertifikate, Use Cases, Apps, Über Uns, Blog, Kontakt.
  - Sektionen: Referenzen & Projekte → „Welche Marken vertrauen auf uns“ → Partner → Auszeichnungen → „Das sagen unsere Kunden“ → Blog → „Lassen Sie uns sprechen!“ → FAQ.
  - CTA: „Unverbindlich Kontakt aufnehmen“, „Zum Lamy/Asphaltgold/Micasa Projekt“. Gebaut mit Gatsby und Storyblok. — [latori.com](https://www.latori.com/)
- **Eshop Guide** – H1 „Kein Schnickschnack, kein Ghosting: Die Shopify-Agentur für wirklich abgeschlossene Projekte.“
  - Mega-Menü: Migration zu Shopify, Neuer Shop, Optimierung, B2B, Internationalisierung, A/B Testing, Shopify Plus, „Shopify in der Schweiz“, eigene Apps (Lexware Office, sevdesk, idealo, DHL Packstation, B2B, Widerruf-Button), Preise, Referenzen nach Branche (Fashion, Beauty, Essen & Trinken …), Wissens-Hub.
  - KPIs: „98 % Weiterempfehlungen | 700+ Unternehmen“, „AniForte … 50 % mehr Conversions“, „65 % deiner laufenden Lizenz- und Agenturkosten“ sparen.
  - CTAs: „Projekt besprechen“, „Einfach Termin buchen.“ Die Seite läuft selbst auf Shopify. — [eshop-guide.de](https://www.eshop-guide.de/)
  - Sitemap: Seiten für Preise, Kostenrechner, Stadt-LPs (Berlin-Kreuzberg, Hannover, Schweiz), Migrationsguide und Checklisten. — [Sitemap](https://www.eshop-guide.de/sitemap.xml)
- **tante-e** – H1 „Die Shopify Agentur, die von Top Brands empfohlen wird“.
  - Nav: Referenzen, Shopify Setup, Migration, Relaunch, Growth Retainer, Shopify Audit, A/B Testing, Team, Jobs, Blog, Podcast, Shopify Kurs.
  - Case-Teaser mit KPIs: „Von Shopware zu Shopify Plus: … 10x Umsatzsteigerung“, „+100% Conversion Rate nach Relaunch“. Dazu „82% unserer Neukunden kommen über Empfehlungen“.
  - Phasenmodell: Fundament legen → Shop optimieren → Umsatz skalieren. Team-Grid mit Vornamen.
  - CTA: „Gespräch vereinbaren“, „Shopify Audit“. Läuft selbst auf Shopify. — [tante-e.com](https://tante-e.com/)
- **14agency** – H1 „Dein Partner für Migrationen im E-Commerce“, eine reine Migrationsnische.
  - Nav: Migrationscheck, je eine Seite „Shopware/WooCommerce/Magento/Gambio/OXID/PrestaShop auf Shopify“, Wartungs- & Pflegepakete, Case Studies, Karriere.
  - CTAs: „Migrationscheck“, „Jetzt Termin sichern“, „Shop Skalierungscheck“, WhatsApp. — [14agency.de](https://14agency.de/); Sitemap mit 11 Case-Study-Seiten [14agency.de/sitemap.xml](https://14agency.de/sitemap.xml)
- **Codext** – H1 „Der Wechsel zu Shopify ist erst der Anfang.“ Title „Shopify-Agentur für Migration und Wachstum“, Meta „Shopify Premier Partner … 100+ Shops migriert“.
  - Sektionen: Zielgruppe („Für Konzerne und Mittelstand“) → 4 Leistungen → Projekte mit KPIs („Conversion Rate +30 %“) → Testimonials → Migrations-USPs → „Wie lange dauert Ihr Umzug?“ → KI → Prozess in 5 Schritten → OMR Festival → FAQ → „Sprechen wir über Ihr Projekt.“
  - CTAs: „Erstgespräch buchen“, „Kostenlose Analyse anfragen“, „Migration Audit“, „BFSG-Check für Shops“. — [codext.de](https://codext.de/)
- **Uplifts** – H1 „4x ausgezeichnete Shopify Agentur“, Title „Shopify Plus zertifiziert | 4x ausgezeichnet“, „Offizieller Shopify Premier Partner“.
  - Cases in der Nav mit KPI im Linktext: „Wholey +26 % CR“, „Hunderunde +2.375 %“.
  - „83 % unserer Kunden kommen über Empfehlungen“, „Shopify Agentur. Sonst nichts. Wir glauben an Spezialisierung.“, FAQ.
  - CTA: „Jetzt Erstgespräch anfragen“. — [uplifts.de](https://uplifts.de/)
- **NICCOS** – H1 „Deine Shopify Agentur für Wechsel und Wachstum“. Meta: „Shopify Plus Partner seit April 2022, 13 Case Studies“.
  - Zieleinstieg „Was möchtest Du mit Shopify erreichen?“ (wechseln / Plus aufbauen / B2B / Conversion) → „Projekte, die wir mit Zahlen belegen“ (+120 % Umsatz, +45 % CR) → 5-Schritte-Migrationsprozess → D2C/B2B/Retail-POS → Logos → 10 FAQ, darunter „Wann ist NICCOS nicht die richtige Agentur?“.
  - CTA: „Kostenlose Ersteinschätzung anfragen“, „Projekt anfragen“. — [niccos.com](https://www.niccos.com/)
- **Schaltwerk Digital** – H1 „Wir bauen deinen Onlineshop, als wär's unser eigener.“ Nav: Branchen-LPs (Fahrrad, Fashion & Textil), Shopify, Shopware, „Termin buchen“.
  - „In 10 Schritten zu deinem umsatzstarken Onlineshop“, Kundenbewertungen, Team, FAQ.
  - Meta: „Festpreis nach Erstgespräch“. KPIs: „+500 % Umsatzsteigerung seit Go-Live“, „50+ erfolgreiche Shops“. — [schaltwerkdigital.de](https://www.schaltwerkdigital.de/)
- **Shopfabrik** – H1 „Shopify Plus Agentur für E-Commerce-Erfolg.“
  - Sektionen: Problem („Viele Shops lassen Umsatz auf der Straße liegen.“) → Leistungen → „Discovery → Konzept → Build → Launch“ → „Shopify Plus Partner mit nachweisbarem Track Record“ → „Echte Marken. Echte Ergebnisse.“ (+34 % Ø Conversion-Steigerung) → Standort Berlin-Mitte → Testimonials → „Bereit für mehr Umsatz?“.
  - Eigene Apps (DisCart, Skonto Pay), Stadt-LPs (Hamburg, Frankfurt, Köln, Leipzig, Mainz). — [shop-fabrik.net](https://shop-fabrik.net/), [Sitemap](https://shop-fabrik.net/sitemap.xml)
  - Plus-Budgets von 15.000–60.000 €+ nur als [Snippet] — [shop-fabrik.net/shopify-agentur](https://shop-fabrik.net/shopify-agentur)
- **Neuzeitwerber** (Shopify-Unterseite einer Generalisten-Agentur) – Title „Shopify Agentur: Shop erstellen lassen ab 4000 €“, H1 „Shopify Agentur für Onlineshops, die verkaufen“. Leistungsblöcke: Shop-Setup, Theme, Migration, Plus, Apps, „Zahlung & Recht DE“, Tracking/GA4. „98 % unserer Kunden empfehlen uns weiter“ (ProvenExpert). — [neuzeitwerber.de/shopify-agentur](https://www.neuzeitwerber.de/shopify-agentur/)
- **digitalsprung** – H1 „Shopify Shops, die verkaufen“, Meta „Über 100 Projekte, 200 Mio. € betreuter Umsatz. Shopify Partner & Meta Business Partner“.
  - Nav kombiniert Shopify (Shop erstellen, Redesign, Theme, Plus, Checkout, Headless, Apps, Migration) und Marketing (Ads, SEO, Klaviyo).
  - „94% Empfehlungsrate“. CTAs: „Erstgespräch vereinbaren“, „Projekt besprechen“. — [digitalsprung.de](https://digitalsprung.de/)
- **apoio** – H1 „E-Commerce Agentur für starke Marken“ (Shopify plus PlentyONE). Fallstudien mit KPIs: „+34% Conversion Rate +41% Bestellungen“. „Arbeite mit uns in 3, 2, 1...“, FAQ.
  - CTA „Kostenloses Erstgespräch buchen“ (eigene Seite /erstgespraech-buchen). Gebaut in Webflow. — [apoio-digital.com](https://www.apoio-digital.com/)
  - Über-uns-Seite als Gründungs-Timeline („Wie unsere Agentur entstand“ → Rebranding → Gründung) → Crew → Standorte. — [apoio Über uns](https://www.apoio-digital.com/unternehmen/ueber-uns)
- **tzn Digital** – H1 „Deine Shopify Agentur für Onlineshops und erfolgreiche Vermarktung“, „6 Gründe, warum Unternehmen uns … wählen“, Video, Vergleich „Spezialisten statt Full-Service – Typische Agenturen vs. Hier bei tzn Digital“.
  - Ablauf in 5 Schritten. KPIs: „+340% Umsatzwachstum“, „+220% …“. CTAs: „Buche jetzt dein Erstgespräch“, Trustpilot. — [tzn-digital.com](https://tzn-digital.com/)
- **5pm (Wien)** – H1 „5pm Shopify Plus Agentur“, Zahlen-Hero „25.000+ A/B-Tests umgesetzt, 700+ Onlineshops analysiert, 300+ Projekte“. CTA „Kostenlose 25 Minuten Analyse“, „Kostenloses Erstgespräch buchen“. Läuft selbst auf Shopify. — [5pm.at](https://5pm.at/)
- **Rankist (CH)** – H1 „Die Shopify Plus Agentur, die Shops skaliert.“ Danach sofort ein Case als H2: „Von 9 auf 34,7 Millionen Euro in zwölf Monaten.“
  - Sektionen: 4 Nutzenversprechen → „Wer für dich arbeitet“ → „Bauen. Betreiben. Skalieren.“ → „Was nach deiner Anfrage passiert“ → „30 Minuten mit Robert von Rankist buchen“ → „293 Shops in 11 Jahren“ → „Was Kunden sagen“.
  - Sitemap: Migrations-LPs je Quellsystem (Shopware/WooCommerce/Magento/JTL/Wix/PrestaShop/Gambio zu Shopify), Stadt-LPs (Zürich, Basel, Bern, Luzern, St. Gallen, Winterthur), Shopify POS, Growth-Audit. — [rankist.ch](https://rankist.ch/), [Sitemap](https://rankist.ch/sitemap.xml)
- **Onlineshop Experts (CH)** – zwei H1-Einstiege nach Situation: „Sie planen einen Onlineshop“ / „Umzug von einem anderen Shopsystem“. Leistungen: Shop Setup, Apps, Schnittstellen, Migration, Schulungen & Support, Store Check, „Official Galaxus App“, „Retail POS Anbindung“. Großes Team-Raster mit Namen. — [onlineshop-experts.ch](https://www.onlineshop-experts.ch/)
- **NETSHAKE** – H1 nur der Markenname, H2 „Deutschlands #1 E-Commerce Inkubator“, „Launch. Grow. Scale.“
  - Werte-Sektion mit Kurze Wege, E-Commerce-Wurzeln, Technische Kompetenz, Erfahrung, Klarer Fahrplan. CTA „Sprich jetzt mit deiner Spezialagentur für Shopify.“ — [netshake.de](https://netshake.de/)
- **NextPercent** – H1 „Shops, die mehr verkaufen. Und wirken wie Marktführer.“
  - Nav: Plus, B2B, **16 Branchenseiten** (Sport, Mode & Schmuck, Beauty, Nahrungsergänzung, Lebensmittel, Tierbedarf, Industrie …), Bewertungen.
  - Sektionen: Cases → 3 Leistungen → „Dutzende 5-Sterne-Bewertungen auf Google und Trustpilot“ → Awards → „Freelancer oder Agentur?“ → „In vier Schritten …“ → USPs („Kein Template“, „Shopify & Klaviyo Partner“) → FAQ → CTA.
  - CTAs: „Projekt anfragen“, „Shop-Check“, „In einer Minute Projekt anfragen“. — [nextpercent.de](https://nextpercent.de/)
  - Sitemap: Stadt-LPs (Ulm, Augsburg, München, Stuttgart), Migration je Quellsystem. — [Sitemap](https://nextpercent.de/sitemap.xml)
- **Oskar Studio** – minimal: H1 Markenname → „Ausgewählte Shopify Projekte“ → „Dein Weg zu unserer Zusammenarbeit“ → „3 Gründe warum Oskar Studio dein Partner ist“. CTA „Kostenlose Shopanalyse“, „Jetzt anfragen“. „95% unserer Kunden kommen durch Empfehlungen“. Läuft auf Shopify. — [oskarstudio.de](https://oskarstudio.de/)
- **applepie** – Title „Die Shopify Agentur und offizieller Shopify Partner“, „Shopify price calculator“, 8 Leistungskacheln (Custom Feature, Klaviyo, Page Speed, Audit, Redesign, Migration, Entwicklung), Case-Logos, über 15 Kurz-Testimonials, Team. — [applepie.berlin](https://applepie.berlin/)
- **Hyghstreet** – H1 „Hy, wir sind Hyghstreet – dein Shopify Platinum Partner“, Projekte & Erfolgsstories, Services, FAQ, Kontakt-CTA „Say Hy!“. Läuft auf Shopify. — [hyghstreet.com](https://hyghstreet.com/)
- **Kombinat (Berlin)** – H1 „Sorgenfreier Shop-Umzug zu Shopify.“
  - „Vier Anzeichen, dass dein Shop dich ausbremst“, Vergleichstabelle „Standard-Umzug vs. KOMBINAT-Umzug“, „Einen Shop-Umzug macht man genau EINMAL“.
  - Dieselben Werte-Überschriften wie bei NETSHAKE: Kurze Wege, E-Commerce-Wurzeln, Technische Kompetenz, Klarer Fahrplan, Erfahrung.
  - CTA „Kostenlose Einschätzung anfragen“. — [kombinat-berlin.de](https://kombinat-berlin.de/)
- **shopnative** – Meta „Die Shopify Plus Agentur für komplexe E-Commerce-Projekte im DACH-Raum … 100 % Shopify“. Startseite stark FAQ-lastig (12 Shopify-Grundlagenfragen), läuft auf Shopify. — [shopnative.io](https://shopnative.io/)
- **ABxpert** – H1 „Mehr Profit durch A/B-Testing“, Meta „Deutschlands einziger CRO spezialisierter Shopify-Plus-Agentur … 2.500+ A/B-Tests … 110 Mio. Mehrumsatz“. CTA „Shop-Analyse vereinbaren“.
  - In den Case-Karten steht vierfach derselbe Platzhalter „78% … Lectus enim lectus volutpat …“, also Lorem-ipsum-Reste einer Webflow-Vorlage. — [abxpert.de](https://www.abxpert.de/)
- **Moving Primates (München/Tirol)** – H1 „Shopify Agentur für Headless Commerce und Shopify Plus“. Meta mit Marken (BORA, Bruker, air up, Porsche eBike). Services: Headless Build, Plus Setup, Sanity-CMS, ERP/PIM, Migration, „Shopify Change Log“. — [movingprimates.de](https://www.movingprimates.de/)
- **Acceleratiq (München)** – H1 „Dein Shopify Partner, von Basic zu Plus.“ Wechsel zu Shopify (WooCommerce, SAP, Xentral, Magento, Shopware, JTL, SFCC), Theme- und App-Entwicklung. KPI „227% Umsatzwachstum in den ersten 24 Monaten“. — [acceleratiq.com](https://acceleratiq.com/)
- **AthariCommerce (Köln)** – H2 „Die führenden Food, Fashion & Lifestyle Brands vertrauen uns.“ (Branchennische). Nav: Über, Leistung, Referenzen, Erstgespräch. Läuft auf Shopify. — [atharicommerce.com](https://atharicommerce.com/)

### Cited Findings — International ([live])
- **Eastside Co** – H1 „Shopify Platinum Partner Agency“, Meta „15 Years' Experience and 50+ Experts“. Leistungen: Web Design, Development, Marketing, Ongoing Support („Shopify Priority Support“), Discovery Audit, App Development. CTAs: „Get In Touch“, „Shopify SEO Audit“. — [eastsideco.com](https://eastsideco.com/)
- **Swanky** – H1 „Compelling digital experiences for international brands on Shopify Plus.“
  - Nav in zwei Säulen: **Launch** (Migrations, Development, Design, Subscription, Integrations, Internationalisation, B2B, Branding, Retail & POS, Agentic Commerce) und **Grow** (CRO, Marketing, Data, Email, PPC, SEO, Loyalty).
  - Etwa 25 Case-Kacheln auf der Startseite, Ebooks. — [swankyagency.com](https://swankyagency.com/)
- **Charle** – H1 „Leading Shopify Agency, UK“.
  - Services: SEO & GEO, New Stores, Migrations, CRO, Theme Dev, Support & Maintenance, UI/UX, Email & SMS, „Shopify Monthly Support Agency“, Audits, Podcast.
  - Eigener Report-/Monitoring-Ansatz („Most agencies tell you what happened last month“ → Track/Recommend/Deliver/Measure). — [charle.co.uk](https://www.charle.co.uk/)
- **Fuel Made** – H1 „We improve conversion rate, average order value, and lifetime value for ecommerce brands.“ Ergebnisorientiert, Shopify und Klaviyo („Klaviyo Master Elite Partner“). Case-Teaser mit Vorher/Nachher-%. CTA „Hire Us“. — [fuelmade.com](https://fuelmade.com/)
- **Anatta** – H1 „Shopify innovation at the speed of enterprise vision“, Meta „Shopify consultancy for enterprise brands ($50M-$2B)“.
  - Success Stories (AG1, Vuori, Dollar Shave Club) und viele Lead-Magnet-Tools: Migration Value Calculator, Replatform Risk Report, Benchmark Scorecard, „5-Day Horizon Readiness Audit“.
  - CTA „Talk to an Architect“. — [anatta.io](https://anatta.io/)
- **Electric Eye** – H1 „Your Shopify Optimization Agency.“ Sektionen: Featured Cases → Core Services → Optimization Process (1. Onboard → 2. Audit → 3. Test → 4. Report) → „Why We're Different“ (u. a. „Simple, predictable pricing“) → CTA „Schedule a Call“. — [electriceye.io](https://electriceye.io/)
- **Ask Phill** – H1 „The Shopify Plus Platinum Partner for Europe's leading fashion, lifestyle, and beauty brands.“ Dazu „Europe's leading Shopify Migration Agency“, „Clients 200+“ und 14 FAQ (Plus vs. SFCC, Shopware→Shopify, Hydrogen, Migrationskosten). — [askphill.com](https://askphill.com/)
- **craftberry** – H1 „The Shopify Agency Behind Leading Ecommerce Brands“, Meta „for $2M+ ecommerce brands … 800+ projects since 2015“. 8 Branchenseiten, Migrations-LPs je Quellsystem, „Maintenance & Support Retainers“, FAQ. — [craftberry.co](https://craftberry.co/)
- **We Make Websites** – nicht abrufbar (403). Laut Roundups London/New York, Shopify-Partner seit 2011 [Snippet]. — [qikify UK-Liste](https://qikify.com/blogs/all-articles/best-shopify-agencies-in-uk)

### Inferences
- Bei den Shopify-Spezialisten ist die Startseite fast eine SEO-Landingpage für „Shopify Agentur“: Title und H1 tragen das Keyword (24/27). Bei den Generalisten trifft das nur auf 3/17 zu.
- Mehrere DACH-Spezialisten (8/27) und internationale Leader (3/8) hosten die eigene Agenturseite auf Shopify (Eshop Guide, tante-e, 5pm, Oskar Studio, Hyghstreet, NETSHAKE, shopnative, AthariCommerce; Ask Phill, Electric Eye, Fuel Made; per `Shopify.shop`-Marker [live]). Das ist ein Signal „wir nutzen, was wir verkaufen“, und für Fokuspage ein Wettbewerbsrisiko: Shopify-Agenturen können ihre Seite mit eigenem Know-how als Shopify-Theme bauen.

### Gaps
- Partner-Tier-Angaben sind Selbstauskünfte. Ein Abgleich mit dem Shopify Partner Directory war nicht Teil der Prüfung. Sekundärquellen widersprechen sich teils, z. B. bei Electric Eye (Premier / Platinum / Plus) [Snippet] — [kirkbyconsulting](https://kirkbyconsulting.com/blog/best-shopify-plus-agencies).
- Logos sind meist Bilder ohne Text, die Heuristik erkennt sie nur über Überschriften („Marken, die uns vertrauen“). Die tatsächliche Logoleisten-Quote ist vermutlich höher.

---

## 2. Was ist gleich (Häufigkeit), was unterscheidet sich, was zeichnet die Besten aus?

### Takeaway
Die Kernelemente kommen jeweils auf 70–90 % der DACH-Shopify-Seiten vor: Shopify-H1, Partner-Status, Logos, Cases, Team, Prozess, Migration, Erstgespräch-CTA.

Wer heraussticht, tut das über drei Dinge:
- **Positionierung:** Nische nach Leistung (Migration, CRO, Headless), Branche (Food/Fashion/Beauty, B2B) oder Kundengröße (Mittelstand, Enterprise).
- **Beweis-Dichte:** konkrete Marken plus Zahlen plus Zeitrahmen.
- **Tonalität bzw. Haltung**, und zwar nicht über Layout.

### Cited Findings — Häufigkeiten (Heuristik auf Startseiten-HTML, [live], 19.11.2026)

| Element | DACH Shopify-Spezialisten (n=27) | International (n=8) | DACH Generalisten (n=17) |
|---|---|---|---|
| H1/Title nennt „Shopify“ | 24 (89 %) | 8 (100 %) | 3 (18 %) |
| Partner-Status genannt (Partner/Plus/Premier/Platinum) | 21 (78 %) | 8 (100 %) | 6 (35 %) |
| Case Studies/Referenzen auf Startseite | 23 (85 %) | 8 (100 %) | 15 (88 %) |
| Team-Sektion oder -Seite in Nav | 22 (81 %) | 8 (100 %) | 12 (71 %) |
| Kundenlogos / „Marken, die uns vertrauen“ (als Überschrift) | 21 (78 %) | 8 (100 %) | 11 (65 %) |
| Migration (Nav/Sektion) | 19 (70 %) | 8 (100 %) | 4 (24 %) |
| Prozess-/Ablauf-Sektion | 19 (70 %) | 3 (38 %) | 10 (59 %) |
| CTA mit „Erstgespräch/Gespräch/Termin/Call“ | 18 (67 %) | 1 (12 %) – dort „Get in touch/Contact“ | 5 (29 %) |
| Review-Plattform (Google/Trustpilot/ProvenExpert/Clutch) | 18 (67 %) | 3 (38 %) | 7 (41 %) |
| Wartung/Retainer/Betreuung | 16 (59 %) | 5 (62 %) | 8 (47 %) |
| Blog/Wissen/Insights in Nav | 16 (59 %) | 7 (88 %) | 11 (65 %) |
| Testimonials-Sektion | 15 (56 %) | 3 (38 %) | 4 (24 %) |
| CRO/A-B-Testing | 15 (56 %) | 6 (75 %) | 8 (47 %) |
| Shopify-Plus-Seite/-Leistung | 14 (52 %) | 6 (75 %) | 5 (29 %) |
| FAQ auf Startseite | 14 (52 %) | 2 (25 %) | 6 (35 %) |
| Gratis-Audit/Analyse/Check als CTA | 13 (48 %) | 5 (62 %) | 10 (59 %) |
| %-KPIs in Case-Teasern | 12 (44 %) | 4 (50 %) | 4 (24 %) |
| Apps (eigene/Entwicklung) | 11 (41 %) | 2 (25 %) | 2 (12 %) |
| Karriere/Jobs in Nav | 11 (41 %) | 3 (38 %) | 10 (59 %) |
| Preise/Festpreis/Kostenrechner sichtbar | 9 (33 %) | 5 (62 %) | 6 (35 %) |
| Branchenseiten/-filter | 9 (33 %) | 5 (62 %) | 8 (47 %) |
| B2B | 7 (26 %) | 2 (25 %) | 7 (41 %) |
| Awards | 6 (22 %) | 3 (38 %) | 7 (41 %) |
| KI/AI/GEO/Agentic prominent in Nav/Sektionen | 5 (19 %) | 4 (50 %) | 11 (65 %) |
| Headless/Hydrogen | 4 (15 %) | 3 (38 %) | 3 (18 %) |
| Shopify POS/Retail | 3 (11 %) | 1 (12 %) | 1 (6 %) |

(Quellen: die unter Frage 1 verlinkten Startseiten. Zuordnung pro Agentur im Arbeitsprotokoll.)

### Cited Findings — wiederkehrende Trust-Elemente (Beispiele [live])
- **Partner-Tier als Headline:**
  - „Offizieller Shopify Platinum Partner“ — [Latori](https://www.latori.com/)
  - „dein Shopify Platinum Partner“ — [Hyghstreet](https://hyghstreet.com/)
  - „Shopify Platinum Partner Agency“ — [Eastside](https://eastsideco.com/)
  - „Offizieller Shopify Premier Partner“ — [Uplifts](https://uplifts.de/)
  - „Shopify Plus Partner seit April 2022“ — [NICCOS](https://www.niccos.com/)
- **Projekt-/Mengenzahlen:**
  - „293 Shops in 11 Jahren“ — [Rankist](https://rankist.ch/)
  - „700+ Unternehmen“ — [Eshop Guide](https://www.eshop-guide.de/)
  - „25.000+ A/B-Tests“ — [5pm](https://5pm.at/)
  - „Mehr als 2.000 erfolgreiche Projekte“ (Generalist) — [eBakery](https://ebakery.de/)
  - „800+ projects since 2015“ — [craftberry](https://craftberry.co/)
  - „Clients 200+“ — [Ask Phill](https://askphill.com/)
- **Empfehlungsquote als Claim:**
  - „83 % … über Empfehlungen“ — [Uplifts](https://uplifts.de/)
  - „82% unserer Neukunden kommen über Empfehlungen“ — [tante-e](https://tante-e.com/)
  - „95% … durch Empfehlungen“ — [Oskar Studio](https://oskarstudio.de/)
  - „94% Empfehlungsrate“ — [digitalsprung](https://digitalsprung.de/)
  - „98 % Weiterempfehlungen“ — [Eshop Guide](https://www.eshop-guide.de/)
- **KPI-Formeln in Case-Teasern („+X % [Metrik]“):**
  - „+120 % Umsatz über alle Kanäle“, „+45% Conversion Rate“ — [NICCOS](https://www.niccos.com/)
  - „Conversion Rate +30 %“ — [Codext](https://codext.de/)
  - „+2.375 % Abo-Kunden“ — [Uplifts](https://uplifts.de/)
  - „+500 % Umsatzsteigerung seit Go-Live“ — [Schaltwerk](https://www.schaltwerkdigital.de/)
  - „+340% Umsatzwachstum“ — [tzn](https://tzn-digital.com/)
  - „Von 9 auf 34,7 Millionen Euro in zwölf Monaten“ — [Rankist](https://rankist.ch/)
  - Snippet-Belege: Eshop Guide VOSSEN „Umsatz … um 50 Prozent erhöht“ [Snippet] — [eshop-guide.de/blogs/referenzen/vossen](https://www.eshop-guide.de/blogs/referenzen/vossen); Codext „+12 % Conversion-Lift Ø“ [Snippet] — [codext.de](https://codext.de/)
- **CTA-Vokabular DACH:**
  - „Erstgespräch buchen/anfragen/vereinbaren“ (Codext, apoio, Uplifts, tzn, 5pm, Shopfabrik, digitalsprung)
  - „Projekt anfragen/besprechen“ (NICCOS, Eshop Guide, NextPercent, Halbstark)
  - „Termin buchen“ (Schaltwerk, NextPercent)
  - Gratis-Diagnose: „Migrationscheck“ (14agency), „Kostenlose 25 Minuten Analyse“ (5pm), „Kostenlose Shopanalyse“ (Oskar), „Shop-Check“ (NextPercent), „Shopify Audit“ (tante-e), „Migration Audit“ (Codext/NICCOS), „Kostenlose Einschätzung“ (Kombinat)
  - Alle [live], URLs siehe Frage 1.
- **Ablauf des Erstgesprächs:** etwa 30 Minuten per Videocall oder Telefon, danach ein Angebot, „auf Wunsch zum Festpreis“ [Snippet] — [Suche: neuzeitwerber](https://www.neuzeitwerber.de/shopify-agentur/). Bestätigt [live] u. a. bei Rankist: „Erstgespräch, 30 Minuten, kostenlos → Schriftlicher Umfang → Festes Team“ — [rankist.ch/shopware-zu-shopify](https://rankist.ch/shopware-zu-shopify)
- **International steht der CTA weniger auf „Gespräch“** („Get in touch“, „Contact Us“, „Hire Us“, „Talk to an Architect“), dafür häufiger auf Audit oder Diagnostic und Lead-Magnet-Tools (Anatta: 8 Tools; Charle: Audits; Eastside: Discovery Audit) — [anatta.io](https://anatta.io/), [charle.co.uk](https://www.charle.co.uk/), [eastsideco.com](https://eastsideco.com/)

### Cited Findings — Differenzierung (was die Besten anders machen, [live])
- **Leistungsnische:**
  - Migration: „Dein Partner für Migrationen im E-Commerce“ — [14agency](https://14agency.de/); „Sorgenfreier Shop-Umzug zu Shopify.“ — [Kombinat](https://kombinat-berlin.de/); „Europe's leading Shopify Migration Agency“ — [Ask Phill](https://askphill.com/)
  - CRO: „Mehr Profit durch A/B-Testing“ — [ABxpert](https://www.abxpert.de/); „Your Shopify Optimization Agency.“ — [Electric Eye](https://electriceye.io/)
  - Headless: [Moving Primates](https://www.movingprimates.de/)
- **Branchen-/Zielgruppennische:**
  - „Europe's leading fashion, lifestyle, and beauty brands“ — [Ask Phill](https://askphill.com/)
  - „Food, Fashion & Lifestyle Brands“ — [AthariCommerce](https://atharicommerce.com/)
  - „Die beste Shopify-Agentur für den Mittelstand“ (Title) — [Eshop Guide](https://www.eshop-guide.de/)
  - „enterprise brands ($50M-$2B)“ — [Anatta](https://anatta.io/)
  - „$2M+ ecommerce brands“ — [craftberry](https://craftberry.co/)
  - B2B/Industrie: TOWA „Go-To-Market Transformation for B2B Champions“ — [towa-digital.com](https://www.towa-digital.com/en/)
- **Branchen-Unterseiten mit echtem Branchen-Know-how:** NextPercent „Shopify-Agentur für Lebensmittel & Getränke“ mit Versandtagen für Frische, Grundpreis/Pflichtangaben, Probierbox und Beispiel-Produktseite — [nextpercent.de/branchen/lebensmittel-getraenke](https://nextpercent.de/branchen/lebensmittel-getraenke)
- **Haltung/Tonalität statt Floskel:**
  - „Kein Schnickschnack, kein Ghosting“ — [Eshop Guide](https://www.eshop-guide.de/)
  - „Wann ist NICCOS nicht die richtige Agentur?“ (FAQ) — [NICCOS](https://www.niccos.com/)
  - „Spezialisten statt Full-Service“-Vergleichstabelle — [tzn](https://tzn-digital.com/)
  - „Shopify Agentur. Sonst nichts.“ — [Uplifts](https://uplifts.de/)
- **Personalisierter CTA:** „30 Minuten mit Robert von Rankist buchen“ — [Rankist](https://rankist.ch/)
- **Programmatische SEO-Tiefe:**
  - Migrations-LP je Quellsystem: Rankist (7), 14agency (6), NextPercent (6), Codext/NICCOS (4), craftberry (5)
  - Stadt-LPs: Rankist (7 CH-Städte), Shopfabrik (5), NextPercent (4), Eshop Guide (3), Uplifts (3)
  - Quellen: [Sitemaps](https://rankist.ch/sitemap.xml), [14agency](https://14agency.de/sitemap.xml), [NextPercent](https://nextpercent.de/sitemap.xml), [Shopfabrik](https://shop-fabrik.net/sitemap.xml), [Uplifts](https://uplifts.de/sitemap.xml)
- **Eigene Produkte als Differenzierung:**
  - Eshop Guide: 7+ eigene Shopify-Apps — [eshop-guide.de](https://www.eshop-guide.de/)
  - Shopfabrik: DisCart, Skonto Pay — [shop-fabrik.net](https://shop-fabrik.net/)
  - tante-e: Podcast und Shopify-Kurs — [tante-e.com](https://tante-e.com/)
  - Charle: Podcast — [charle.co.uk](https://www.charle.co.uk/)

### Inferences
- Was alle gemeinsam haben, ist in der Kategorie Pflicht und differenziert niemanden. Unterscheiden kann sich eine Agentur über (a) die Wahl der Nische, (b) die Beweisführung (Marke, Ausgangslage, Zahl, Zeitraum, Zitat) und (c) Ton und Persönlichkeit (Gründer-Gesicht, Haltungs-Claims, „wann wir nicht passen“).
- Der DACH-Markt ist CTA-seitig deutlich „Erstgespräch-zentriert“, der angloamerikanische eher „Audit/Tool-zentriert“. Für eine neu gegründete Agentur ohne Cases ist ein Gratis-Check oder Audit als Einstieg plausibel, weil er keine Referenzen voraussetzt.
- Junge Agenturen (z. B. Oskar Studio, Hyghstreet, AthariCommerce) haben sichtbar schlankere Seiten: wenige Sektionen, Cases als Logos oder Bilder, kaum KPIs. Fokuspage könnte gerade den „Beweis ohne viele Referenzen“ adressieren, etwa mit Prozess-Transparenz, Gründerprofil, Audit-Angebot oder Beispiel-Mockups.

### Gaps
- Keine belastbaren Daten dazu, welche Elemente tatsächlich konvertieren, etwa A/B-Tests von Agenturseiten. Die Häufigkeit sagt nichts über Wirkung.
- Keine Prüfung der Unterseiten bei allen Agenturen. Die Sitemaps habe ich nur bei 14 Agenturen ausgewertet (tzn, Uplifts und Kombinat lieferten nur Teil-Sitemaps).

---

## 3. Typisches Seitenset und Sektionsreihenfolge → Bausteine und Seiten-Templates für Fokuspage

### Takeaway
**Typische Startseiten-Reihenfolge** (Konsens aus den H-Strukturen von Codext, NICCOS, tante-e, Uplifts, Rankist, NextPercent, Shopfabrik, Schaltwerk, tzn, Electric Eye):

Hero (Shopify-Claim + Partner-Badge + CTA) → Logo-Leiste → Leistungen (3–4 Karten) → Case-Teaser mit KPI → Warum wir/USPs (optional Vergleich „wir vs. typische Agentur“) → Prozess (3–5 Schritte) → Testimonials/Bewertungen → Team → FAQ → Abschluss-CTA (Erstgespräch).

**Typisches Seitenset:** Startseite, Leistungen (+ je eine Leistungs-LP), Migration (+ je Quellsystem), Shopify Plus, Referenzen/Case Studies (+ Detail), Über uns/Team, Kontakt/Erstgespräch, Blog/Wissen. Optional: B2B, Branchen, Karriere, Preise, Stadt-LPs, Apps.

### Cited Findings — Sektionsreihenfolge (H-Struktur [live])
- Codext: H1 → Zielgruppe → „Was wir machen“ (4) → „Ausgewählte Projekte“ → „Was Kunden … sagen“ → Migrations-USPs → Dauer → KI → Prozess (5) → Event → „Häufige Fragen“ → „Sprechen wir über Ihr Projekt.“ — [codext.de](https://codext.de/)
- NICCOS: H1 → Zielauswahl (4) → „Projekte, die wir mit Zahlen belegen“ → Prozess (5) → „Wir sagen Dir, was zuerst dran ist“ → D2C/B2B/POS → Logos → FAQ (10). — [niccos.com](https://www.niccos.com/)
- Uplifts: H1 → Claim → Logos → Benefits (CR, Page Speed, UX, Award, Prozess, Premier Partner) → Cases → Daten → Empfehlungsquote → Leistungen (3) → Beratung → Spezialisierung → Über uns → FAQ → CTA. — [uplifts.de](https://uplifts.de/)
- NextPercent: H1 → Claim → Cases → Leistungen (3) → Bewertungen → Awards → „Freelancer oder Agentur?“ → 4 Schritte → USPs → Case → FAQ → CTA. — [nextpercent.de](https://nextpercent.de/)
- Shopfabrik: H1 → Problem → Leistungen → Prozess (Discovery→Konzept→Build→Launch) → Partner-Track-Record → Cases → Standort → Testimonials → CTA. — [shop-fabrik.net](https://shop-fabrik.net/)
- Electric Eye (international): H1 → Featured Cases → Core Services → Process (4) → Trusted By → Why Different → CTA. — [electriceye.io](https://electriceye.io/)
- Framer-Agenturvorlage „Agenceia“ als Gegencheck aus dem Template-Markt [live]:
  - Home = „hero, services, project list …, expertise, facts, testimonials“
  - 10 Seiten: Home, Agency, Work, Project (CMS), Expertise, Contact, Blog, Blog Post, Getting Started, 404
  - CMS-Collections: Projects, Team, Clients, Services, Process, Blog
  - [framer.com/marketplace/templates/agenceia](https://www.framer.com/marketplace/templates/agenceia/)
- Weitere Vorlagen [Snippet]: Morphe (Framer) mit CMS-Cases, 4-Schritt-Prozess, Pricing-Toggle, Testimonials, FAQ — [framer.com/marketplace/templates/morphe](https://www.framer.com/marketplace/templates/morphe/); Montix (Webflow) mit 17 Seiten inkl. Services, Case-Details, Team, Pricing, Blog — [contra.com](https://contra.com/products/1NzVHgYI-montix-professional-services-website-template)

### Cited Findings — Unterseiten-Templates ([live])
- **Migrations-LP je Quellsystem:**
  - Rankist „Shopware zu Shopify: in 4 Wochen umziehen, ohne ein Ranking zu verlieren.“ → „Kommt dir das bekannt vor?“ (4 Pain Points) → Vergleich „Shopware vs Shopify im Alltag“ → „Alles zieht mit“ → Wochenplan (Woche 1 Analyse & Redirect-Map, Woche 2–3 Import, Woche 4 Go-live, 30 Tage Monitoring) → „Was sich … verändert“ → FAQ → CTA — [rankist.ch/shopware-zu-shopify](https://rankist.ch/shopware-zu-shopify)
  - NextPercent: „Kennst du das?“ → „So läuft dein Wechsel“ → „Was kommt mit, was nicht?“ → „Was wird in Shopify zu was?“ → „Migrations-App oder Agentur?“ → Dauer → Kosten (Datenmenge, Design-Tiefe, Anbindungen) → Rankings → FAQ → „Du kommst von einem anderen System?“ — [nextpercent.de/shopify-migration/shopware](https://nextpercent.de/shopify-migration/shopware)
  - 14agency: Produkt-, Kunden-, Blogdaten, Passwort-Mailing, Ranking-Migration → Referenzen → Roadmap — [14agency.de/migration-von-shopware-auf-shopify](https://14agency.de/migration-von-shopware-auf-shopify)
- **Case-Study-Detail:**
  - tante-e/fritz-kola: Ausgangssituation → Herausforderung → Lösungsansatz → Umsetzung → Ergebnisse → Lessons Learned → Formular „Termin vereinbaren“ — [tante-e.com/pages/case-study-fritz-kola](https://tante-e.com/pages/case-study-fritz-kola)
  - Shopfabrik/HOLY: Kunde → Entwicklung über Jahre → Features (Mix-&-Match, CRO, international) → „Ähnliche Ergebnisse für Deinen Shop?“ — [shop-fabrik.net/case-studies/holy](https://shop-fabrik.net/case-studies/holy)
- **Shopify-Plus-LP:** Eshop Guide mit Hook-H1 („Bye Bye, Performance-Nieten …“) → Warum Plus → Case mit KPIs („31 % mehr Conversions, 8 Wochen bis zum Go-live“) → „Warum wir die beste Shopify Plus Agentur sind“ → Testimonials → FAQ — [eshop-guide.de/pages/shopify-plus-agentur](https://www.eshop-guide.de/pages/shopify-plus-agentur)
- **Branchen-LP:** NextPercent Food (siehe Frage 2) — [nextpercent.de/branchen/lebensmittel-getraenke](https://nextpercent.de/branchen/lebensmittel-getraenke)
- **Über uns:** apoio mit Gründungsgeschichte als Timeline → Crew → Standorte — [apoio-digital.com/unternehmen/ueber-uns](https://www.apoio-digital.com/unternehmen/ueber-uns)
- **Preis-/Kalkulator-Seiten:** Eshop Guide /pages/angebot-preise und /pages/shopify-kostenrechner, tante-e /pages/package-calculator-2 (Sitemaps) — [eshop-guide.de/sitemap.xml](https://www.eshop-guide.de/sitemap.xml), [tante-e.com/sitemap.xml](https://tante-e.com/sitemap.xml); applepie „Shopify price calculator“ — [applepie.berlin](https://applepie.berlin/)

### Inferences — Bausteinliste für Fokuspage (abgeleitet)

**A. Sektionsbausteine (Startseite und LPs)**
1. **Hero „Shopify-Agentur“**, Varianten: (a) Kategorie + Status, (b) Ergebnis-Claim, (c) Nischen-Claim, (d) Haltungs-Claim, (e) Zielauswahl („Was möchtest du erreichen?“ mit 3–4 Pfaden), (f) Zahlen-Hero (3 Kennzahlen). Pflichtfelder: Partner-Badge (Tier-Auswahl: Partner / Plus Partner / Select / Plus / Premier / Platinum), Primär-CTA „Erstgespräch“, Sekundär-CTA „Referenzen/Gratis-Check“, Bewertungs-Badge.
2. **Logo-Leiste** „Marken, die uns vertrauen“ mit Fallback für Neugründer (Tool-/Partner-Logos wie Klaviyo, Recharge, JTL, Xentral oder „Erfahrung aus Projekten bei …“).
3. **Leistungskarten (3–4)** mit vorbefüllten Shopify-Leistungen: Shop-Setup/Neuer Shop, Migration/Relaunch, Shopify Plus & B2B, CRO/A-B-Testing, Betreuung/Retainer, App- & Schnittstellen-Entwicklung, Klaviyo/E-Mail, SEO/GEO, Headless/Hydrogen, POS.
4. **Case-Teaser-Karte** mit Feldern: Marke, Branche, Ausgangssystem → Shopify (Plus), KPI 1–3 („+X % CR“, „+X % AOV“, „X Wochen bis Go-live“), Screenshot, Link. Dazu ein **Case-Grid mit Filtern** (Branche, Service, Feature), wie bei tante-e.
5. **Zahlen-/Fakten-Leiste**: Projekte, Jahre, Shops migriert, A/B-Tests, Empfehlungsquote, Google-Bewertung.
6. **Warum wir / USPs** (3–6 Kacheln) plus Variante **Vergleichstabelle** „Typische Agentur vs. wir“ / „Freelancer vs. Agentur“ / „Standard-Umzug vs. unser Umzug“.
7. **Prozess/Ablauf** (3–5 Schritte; Presets wie „Erstgespräch → Konzept → Umsetzung → Go-live → Betreuung“ oder „Woche 1–4“), Variante Phasenmodell „Launch / Grow / Scale“ bzw. „Bauen / Betreiben / Skalieren“.
8. **„Was nach deiner Anfrage passiert“** (3 Schritte mit Dauer, Kosten, Verbindlichkeit) – senkt die Hemmschwelle vor dem CTA.
9. **Testimonials** (Zitat, Name, Rolle, Marke, Foto) plus **Bewertungs-Widget** (Google/Trustpilot/ProvenExpert/Clutch).
10. **Team-Grid** (Foto, Vorname, Rolle) und Variante **Gründer-Spotlight** mit persönlichem Kalender-CTA („30 Minuten mit [Name] buchen“).
11. **Partner & Zertifikate / Awards** (Shopify-Tier, Klaviyo, Meta, Google, „4x ausgezeichnet“).
12. **FAQ** mit Shopify-typischen Fragen vorbefüllt: Dauer, Kosten, Plus ja/nein, SEO bei Migration, ERP-Anbindung, Betreuung nach Go-live, „Wann sind wir nicht die richtige Agentur?“.
13. **Problem-/Pain-Block** „Kennst du das?“ / „Vier Anzeichen, dass dein Shop dich ausbremst“.
14. **Abschluss-CTA** mit Kalender-Embed (Calendly/Cal.com/HubSpot) oder Kurzformular („In einer Minute Projekt anfragen“), optional mit Qualifizierungsfragen (Budget, Zeitplan, aktuelles System).
15. **Lead-Magnet-Block**: Gratis-Shop-Check/Audit, Migrations-Checkliste, Kostenrechner (Eshop Guide, tante-e, Anatta).
16. **Blog/Wissen-Teaser** und **Branchen-Teaser**.

**B. Seiten-Templates**
- Startseite
- Leistungsübersicht und Leistungs-LP (Setup, Plus, B2B, CRO, Betreuung/Retainer, Apps/Integrationen, Headless, POS)
- **Migrations-LP je Quellsystem** (Shopware, WooCommerce, Magento, JTL, Gambio, OXID, PrestaShop, Wix, plentymarkets)
- Case-Übersicht und Case-Detail (Ausgangslage → Herausforderung → Lösung → Umsetzung → Ergebnisse → Zitat → CTA)
- Branchen-LP (Fashion, Food & Getränke, Beauty, Supplements, Home & Living, B2B/Industrie)
- **Stadt-/Regions-LP** („Shopify Agentur [Stadt]“)
- Über uns (Story/Timeline, Team, Werte, Standort)
- Karriere/Jobs
- Kontakt/Erstgespräch
- Preise/Pakete und Kostenrechner
- Audit-/Check-LP
- Blog-Artikel
- Impressum/Datenschutz
- Für DE: Barrierefreiheitserklärung. Eshop Guide und Kombinat haben solche Seiten laut Sitemap; das deutet auf BFSG-Relevanz hin. — [eshop-guide.de/sitemap.xml](https://www.eshop-guide.de/sitemap.xml), [kombinat-berlin.de/sitemap.xml](https://kombinat-berlin.de/sitemap.xml)

**C. Headline-Formeln (DE), abgeleitet aus den beobachteten H1**
- *Kategorie + Status:* „[Name] – deine Shopify [Plus] Agentur aus [Stadt]“ / „Offizieller Shopify [Tier] Partner für [Zielgruppe]“. Vorbilder: Latori, Hyghstreet, 5pm, Shopfabrik.
- *Ergebnis:* „Shopify-Shops, die verkaufen.“ / „Shops, die mehr verkaufen. Und wirken wie Marktführer.“ / „Die Shopify Plus Agentur, die Shops skaliert.“ Vorbilder: digitalsprung, NextPercent, Rankist.
- *Nische Leistung:* „Sorgenfreier Umzug von [System] zu Shopify.“ / „[System] zu Shopify: in [X] Wochen umziehen, ohne ein Ranking zu verlieren.“ / „Mehr Profit durch A/B-Testing.“ Vorbilder: Kombinat, Rankist, ABxpert.
- *Nische Zielgruppe/Branche:* „Die Shopify-Agentur für [Food-/Fashion-/Beauty-]Marken“ / „Shopify für den Mittelstand – ohne Agentur-Overhead.“ Vorbilder: Ask Phill, AthariCommerce, Eshop Guide.
- *Social Proof:* „Die Shopify Agentur, die von Top-Brands empfohlen wird.“ / „[N]x ausgezeichnete Shopify Agentur.“ Vorbilder: tante-e, Uplifts.
- *Haltung:* „Kein Schnickschnack, kein Ghosting: …“ / „Wir bauen deinen Onlineshop, als wär's unser eigener.“ / „Der Wechsel zu Shopify ist erst der Anfang.“ Vorbilder: Eshop Guide, Schaltwerk, Codext.
- *KPI-Case als H2 direkt nach Hero:* „Von [X] auf [Y] Mio. € in [Z] Monaten.“ Vorbild: Rankist.
- *CTA-Formeln:* „Kostenloses Erstgespräch buchen“, „Projekt anfragen“, „Kostenlosen Shop-Check anfordern“, „Migrationscheck starten“, „30 Minuten mit [Vorname] buchen“, „In einer Minute Projekt anfragen“.

### Gaps
- Die Heuristik erfasst keine visuellen Layoutmuster wie Bento-Grids, Video-Hero oder Animationen. Ein Screenshot-Vergleich fehlt.
- Ob Stadt-LPs oder Migrations-LPs messbar Leads bringen, ist nicht belegt. Belegt ist nur, dass sie verbreitet sind.

---

## 4. Artikel und Analysen, die das Muster bestätigen

### Takeaway
Template-Marktplätze (Framer/Webflow) und Inspirationslisten bestätigen dasselbe Standardgerüst für Agenturseiten: Hero, Services, Cases, Testimonials, Prozess, Team, FAQ, Pricing. Shopify-spezifische Inspiration ist dünn und stammt vor allem aus Agentur-Listicles.

### Cited Findings
- Die Framer-Vorlage Agenceia beschreibt den Standard selbst: „Most agency websites look the same: a centred headline, a stock photo, three icons.“ Sie bietet trotzdem dieselbe Informationsarchitektur (Home, Agency, Work, Expertise, Contact, Blog; CMS: Projects, Team, Clients, Services, Process, Blog) [live] — [framer.com/marketplace/templates/agenceia](https://www.framer.com/marketplace/templates/agenceia/)
- Weitere Framer/Webflow-Agenturvorlagen (Morphe, Montix, Agenflux, Brandt, Motive) enthalten Hero, Services, Case Studies (CMS), Prozess in 4 Schritten, Testimonials, Team, Pricing und FAQ [Snippet] — [Morphe](https://www.framer.com/marketplace/templates/morphe/), [Brandt](https://www.framer.com/marketplace/templates/brandt/), [Agenflux](https://www.framer.com/marketplace/templates/agenflux/), [Montix](https://contra.com/products/1NzVHgYI-montix-professional-services-website-template)
- Inspirationslisten nennen Shopify-Agenturen mit Fokus auf Case-Präsentation: Eastside Co mit „strong case study presentations and results-driven portfolio“, Charle, Lustre („80+ brand launches and 140+ ecommerce builds“), Conspire. Wiederkehrende Trends sind minimalistische Schwarz-Weiß- und Editorial-Layouts [Snippet] — [Colorlib Digital Agency Examples](https://colorlib.com/wp/digital-agency-website-examples/), [Colorlib Branding Agency Examples](https://colorlib.com/wp/branding-agency-website-examples/)
- Weitere Inspirationssammlungen: [99designs Agency](https://99designs.com/inspiration/websites/agency), [createtoday 681 Agency Examples](https://createtoday.io/examples?category=agency), [Wix Studio](https://www.wix.com/studio/blog/examples-of-agency-websites), [sitebuilderreport](https://www.sitebuilderreport.com/inspiration/agency-websites) [Snippet, nicht im Detail ausgewertet].
- Der Ratgeber von Dr. Web zur Agenturwahl strukturiert nach Kosten, Projektablauf, Partner vs. Plus Partner, Migration, Dauer und Datenhoheit. Das sind genau die Fragen, die Agentur-FAQs beantworten [live, Überschriften] — [drweb.de/shopify-agentur-vergleich](https://www.drweb.de/shopify-agentur-vergleich/). Laut Dr. Web ist ein Standardshop „meist in 6 bis 14 Wochen live“, komplexe Plus/B2B-Projekte brauchen 12–24 Wochen [Snippet].
- Golden Web Age rät Käufern: dasselbe Briefing an alle, konkretes Projektteam erfragen, Weg bis zur Abnahme klären, Zeit nach dem Start planen, Zugänge und Übergabe klären [live, Überschriften] — [goldenwebage.de/shopify/shopify-agenturen-vergleich](https://www.goldenwebage.de/shopify/shopify-agenturen-vergleich/). Daraus ergeben sich Inhalte, die die Agenturseite proaktiv liefern sollte (Team, Abnahmeprozess, Betreuung, Datenhoheit).

### Inferences
- Das Muster ist nicht Shopify-spezifisch. Es ist das generische Agentur-Gerüst plus Shopify-Layer: Partner-Tier, Migration je System, Plus/B2B, Apps/Integrationen, KPI-Cases mit E-Commerce-Metriken (CR, AOV, Umsatz).
- Fokuspages Mehrwert gegenüber Framer- oder Webflow-Vorlagen müsste genau dieser Shopify-Layer sein, also vorgefertigte Inhalte (Copy, FAQ, Migrations-LPs, KPI-Case-Felder, Partner-Badges, Branchen-LPs) und nicht das Layout.

### Gaps
- Keine Awwwards- oder Dribbble-Analyse speziell zu Shopify-Agenturen gefunden.
- Keine unabhängige Studie (z. B. Nielsen Norman) zu Agenturseiten speziell. Aella verweist nur allgemein auf NN/g zum schnellen Scannen von Seiten — [aellacreativeforce.com](https://aellacreativeforce.com/why-most-agency-websites-feel-the-same-in-2026/)

---

## 5. Sind Agenturseiten „alle gleich“? Belege dafür und dagegen, Risiko der Uniformität

### Takeaway
**Ja, strukturell.** Die Sektionsfolge und das Trust-Vokabular sind hochgradig standardisiert. Es gibt sogar Fälle nahezu identischer Navigation bzw. Überschriften zwischen verschiedenen Agenturen und Template-Reste.

**Nein, in der Positionierung.** Die stärksten Seiten unterscheiden sich über Nische, Beweise und Ton.

Ein Builder mit vorgefertigter Copy verschärft die Gleichförmigkeit, wenn er nur Layouts und generische Texte liefert. Er muss deshalb **Positionierung erzwingen und differenzierende Inhalte abfragen**.

### Cited Findings — Belege für „gleich“
- Die Häufigkeiten aus Frage 2 zeigen 70–90 % Abdeckung der Kernelemente bei DACH-Spezialisten [live].
- **Nahezu identische Navigation:** Codext und NICCOS haben fast deckungsgleiche Mega-Menüs („Shopify B2B | Internationalisierung | Shopify GEO | Shopify POS | Personalisierung & Suche | Abo-Commerce | … | SAP-Integration | Dynamics 365 Business Central | Oracle NetSuite | Xentral | JTL-Wawi“, „Migration Audit“). Auch die Titles sind fast identisch: „Shopify-Agentur für Migration und Wachstum – Codext GmbH“ und „Shopify Agentur für Migration und Wachstum | NICCOS“. Ob es eine Verbindung oder ein gemeinsames Template gibt, ist nicht geprüft; auf den Startseiten verweist keine Seite auf die andere [live] — [codext.de](https://codext.de/), [niccos.com](https://www.niccos.com/)
- **Identische Werte-Überschriften:** NETSHAKE und Kombinat nutzen dieselben Überschriften („Kurze Wege“, „E-Commerce-Wurzeln“, „Technische Kompetenz“, „Klarer Fahrplan“, „Erfahrung“). Eine Beziehung ist nicht geprüft [live] — [netshake.de](https://netshake.de/), [kombinat-berlin.de](https://kombinat-berlin.de/)
- **Template-Reste:** ABxpert zeigt in vier Case-Karten denselben Lorem-ipsum-Platzhalter („Lectus enim lectus volutpat …“) mit „78%“ [live] — [abxpert.de](https://www.abxpert.de/)
- **Branchenanalysen:**
  - RSW/US-Umfrage 2026: über 80 % der Agenturen halten sich für differenziert, über 75 % halten die Branche für undifferenziert. 85 % entwickeln ihre Positionierung nur intern, 20 % testen sie mit Interessenten. „many other … agency sites say these same things, often in nearly identical words“ [live] — [rswus.com](https://www.rswus.com/agency-positioning-differentiation/)
  - Aella (April 2026): „Everyone is copying everyone … It all looks modern. It all sounds identical … The problem is not design. The problem is positioning.“ [live] — [aellacreativeforce.com](https://aellacreativeforce.com/why-most-agency-websites-feel-the-same-in-2026/)
  - Campaign: Agenturseiten kreisen um „us, us, us“ statt „them, them, them“ [Snippet] — [campaignlive.com](https://www.campaignlive.com/article/agency-websites-look-same-heres-differentiate/1964728)
  - Schmidt Consulting: Floskeln wie „full-service agency“, „results-driven team“ sind kein Differenzierungsmerkmal, wenn fünf Agenturen sie sagen können [Snippet] — [schmidtconsulting.group](https://www.schmidtconsulting.group/blog/agency-positioning-differentiation/)
  - Branding Strategy Insider: Wenn alle Awards gewinnen, wirkt das nicht mehr als Differenzierung [Snippet] — [brandingstrategyinsider.com](https://brandingstrategyinsider.com/2015/07/counter-agency-positioning-dilemma/)

### Cited Findings — Belege für „nicht gleich“
- Klare Nischen- und Haltungs-Claims bei Eshop Guide, 14agency, Kombinat, ABxpert, Ask Phill, Anatta, Electric Eye, AthariCommerce [live] (URLs siehe Frage 1/2).
- Tiefe, branchenspezifische Inhalte (NextPercent Food-LP mit Grundpreis, Frische-Versand, Probierbox) [live] — [nextpercent.de/branchen/lebensmittel-getraenke](https://nextpercent.de/branchen/lebensmittel-getraenke)
- Eigene Produkte, Formate und Tools als Unterscheidungsmerkmal: Apps (Eshop Guide, Shopfabrik), Podcast/Kurs (tante-e, Charle), Diagnose-Tools (Anatta) [live].
- Auch der Template-Markt verkauft „Andersartigkeit“ als Feature: Agenceia wirbt mit „for studios that refuse to blend in“ [live] — [framer.com](https://www.framer.com/marketplace/templates/agenceia/)

### Inferences — Konsequenzen für Fokuspage
- **Die Hypothese ist bestätigt.** Die Bausteine sind sehr ähnlich und gut vorfertigbar. Das gilt vor allem für den Shopify-Layer (Partner-Badge, Migration je System, Plus/B2B, KPI-Cases, FAQ, Erstgespräch-Flow).
- **Das Risiko ist real.** Wenn viele Neugründer dieselben vorgefertigten Headlines und FAQ nutzen, entstehen genau die „nearly identical words“, die RSW kritisiert. Die Codext/NICCOS- und NETSHAKE/Kombinat-Funde und der ABxpert-Lorem-ipsum zeigen, dass Kopieren oder Template-Nutzung schon heute sichtbar wird. Duplicate Content schadet außerdem SEO und GEO.
- **Gegenmaßnahmen im Produkt (Vorschläge, nicht belegt):**
  - Ein Pflicht-Onboarding zur Positionierung (Nische: Leistung, Branche, Kundengröße oder Region; Haltung/Anti-Positionierung „wann wir nicht passen“), aus dem Headlines generiert werden statt aus festen Texten.
  - Copy-Varianten mit Variationspflicht.
  - Platzhalter-Linting (kein Lorem ipsum und keine Platzhalter-KPIs bei Veröffentlichung).
  - Beweis-Bausteine, die auch ohne Referenzen funktionieren (Gründer-Spotlight mit Vorerfahrung, transparenter Prozess und Preise, Gratis-Audit, Demo-Shop).
  - Design-Themes, die sich deutlich unterscheiden.
- **Wettbewerbsrisiko:** Viele Shopify-Agenturen bauen ihre eigene Seite als Shopify-Store (8/27 DACH, 3/8 international [live]). Für sie ist ein externer Builder weniger naheliegend. Zielgruppe sind eher Neugründer ohne Zeit oder Design-Ressourcen, die nicht „Schuster ohne Schuhe“ sein wollen. Diese Abgrenzung ist eine Inferenz und müsste per Interviews validiert werden.

### Gaps
- Unklar, ob Käufer (Shop-Betreiber) Gleichförmigkeit überhaupt negativ wahrnehmen. Es fehlen Nutzerstudien speziell zur Auswahl von E-Commerce-Agenturen.
- Ob die Ähnlichkeiten Codext/NICCOS und NETSHAKE/Kombinat auf gemeinsame Eigentümer, Dienstleister oder Kopie zurückgehen, ist ungeklärt (Impressum nicht geprüft).
- We Make Websites (403) und Finer Digital (falsche Domain) fehlen in der Stichprobe.
