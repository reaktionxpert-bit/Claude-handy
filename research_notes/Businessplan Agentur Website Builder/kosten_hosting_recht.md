# Kosten, Hosting/Betrieb und Recht – Solo-Gründer, Nischen-Website-Builder-SaaS für Agenturen (DACH)

Stand der Recherche: 19.11.2026. Methodik: Websuche; Seitenabrufe waren größtenteils nicht möglich (www.hostinger.com war im Netzwerk dieser Session gesperrt; die Domain müsste in den Netzwerkeinstellungen der Session freigegeben werden). Viele Fakten stammen deshalb **nur aus Such-Snippets bzw. Drittquellen** – markiert mit [Snippet]. Eigene Rechnungen sind mit [SCHÄTZUNG] markiert. USD→EUR wird grob mit 1 USD ≈ 0,90 EUR gerechnet [SCHÄTZUNG, Wechselkurs nicht recherchiert].

---

## 1. Hosting-Optionen und Kosten (Hostinger VPS vs. Managed/Static) inkl. Betrieb, Custom Domains, DSGVO/AVV

### Takeaway
Ein Hostinger-VPS (KVM 2) ist mit ca. 9–15 USD/Monat billig, bedeutet aber volle Eigenverantwortung für Patches, Backups, Monitoring und SSL für viele Kundendomains. Hostinger sieht die wöchentlichen VPS-Backups nur als Kulanzleistung, und einen AVV haben wir nicht gefunden. Für einen Solo-Gründer in Teilzeit ist ein Hybrid wahrscheinlich robuster: generierte Seiten statisch ausliefern und Custom Domains/SSL über Cloudflare for SaaS (100 Hostnamen gratis, danach 0,10 USD pro Hostname und Monat) abwickeln. Nur Editor/API laufen auf einem kleinen VPS. Bei Hetzner sind die Preise 2026 deutlich gestiegen.

### Cited Findings
**Hostinger VPS**
- Hostinger KVM 2: 2 vCPU, 8 GB RAM, 100 GB Speicher, 8 TB Traffic, 8,99 USD/Monat bei 24 Monaten Laufzeit. Der zweite Preis von 14,99 USD/Monat ist vermutlich der Verlängerungspreis (Spaltenkopf im Snippet nicht sichtbar) [Snippet] — [Hostinger vps-hosting.md](https://www.hostinger.com/vps-hosting.md)
- VPSBenchmarks (Test April 2026): KVM 2 kostet 24,49 USD bei monatlicher Zahlung und 16,99 USD/Monat bei mindestens 1 Jahr Laufzeit (−30 %) [Snippet] — [VPSBenchmarks Trial Apr 2026](https://www.vpsbenchmarks.com/trials/hostinger_performance_trial_13Apr2026)
- Einen EUR-Preis von Hostinger selbst haben wir nicht gefunden. Laut einem Review liegt KVM 2 bei langer Laufzeit im Bereich 7–9 USD [Snippet] — [Desking Review 2026](https://desking.app/review/hostinger-vps)
- Laut Hostinger-Hostingvertrag läuft das Backup einmal pro Woche und überschreibt ältere Backups. Auf dem Remote-Server werden nur zwei Wochen aufbewahrt. Für VPS-Konten gilt der Backup-Dienst als **Kulanz** und kann nach Ermessen von Hostinger geändert werden [Snippet] — [Hostinger Hosting-Vertrag (DE)](https://www.hostinger.com/de/legal/hosting-vertrag)
- Die deutsche VPS-Seite wirbt mit „kostenlosen automatischen wöchentlichen Backups“ und hat eine eigene Seite für den Standort Deutschland [Snippet] — [Hostinger VPS Germany](https://www.hostinger.com/vps/servers/germany)
- Einen Hostinger-AVV haben wir nicht gefunden. Die Datenschutzerklärung verweist nur allgemein auf die DSGVO [Snippet] — [Hostinger Datenschutz](https://www.hostinger.com/de/privacy-policy)
- Allgemeiner Hinweis: Eine Serveradresse in Frankfurt erledigt Kapitel V DSGVO (Drittlandübermittlung) nicht automatisch, wenn der Anbieter außerhalb der EU sitzt oder Unterauftragsverarbeiter dort nutzt. Ein AVV ist vor dem ersten Upload nötig [Snippet] — [SSD Nodes: VPS und DSGVO](https://www.ssdnodes.com/learn/lang/de/storage-vps-and-gdpr-what-to-check)

**Hetzner Cloud (deutscher Anbieter)**
- Hetzner hat die Preise 2026 zweimal angepasst. Die zweite Anpassung gilt ab 15.06.2026 für Neubestellungen und Rescales [Snippet] — [Hetzner Docs: Price adjustment](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/)
- CX23 (2 vCPU / 4 GB / 40 GB) kostet nach Juni 2026 5,49 €/Monat (EU). Beim Vorpreis widersprechen sich die Quellen (3,99 € bzw. 2,99 €) [Snippet] — [Bitdoze Hetzner Preise 2026](https://www.bitdoze.com/de/hetzner-cloud-guenstige-tarife/); [Findstack](https://findstack.com/resources/hetzner-price-increase-2026)
- CPX22 stieg von 7,99 € auf 19,49 €/Monat (ohne USt./IPv4). Die CPX/CCX-Linien legten um 113–175 % zu, die ARM-/Intel-Shared-Linien um ca. 30 % [Snippet] — [WZ-IT: Hetzner-Preiserhöhung Juni 2026](https://wz-it.com/blog/hetzner-preiserhoehung-juni-2026-cpx-ccx-alternativen/); [webhosting.today](https://webhosting.today/2026/06/18/hetzners-price-increases-reached-209-the-30-headline-applied-to-a-different-tier/)
- Die Quellen widersprechen sich, ob CX23 zeitweise nicht bestellbar war [Snippet] — [vincentschmalbach.com](https://www.vincentschmalbach.com/hetzner-cheap-cloud-unavailable-price-increases/); contradicted by [Bitdoze](https://www.bitdoze.com/hetzner-cloud-cost-optimized-plans/)
- Bei der Preisanpassung vom 1. April 2026 waren auch Bestandskunden betroffen [Snippet] — [Tom's Hardware](https://www.tomshardware.com/tech-industry/hetzner-to-raise-prices-by-up-to-37-percent-from-april-1)

**Cloudflare for SaaS (Custom Domains + SSL für viele Kundendomains)**
- Die Pläne Free, Pro und Business enthalten je 100 Custom Hostnames. Jeder weitere kostet 0,10 USD/Monat, maximal sind 50.000 möglich [Snippet] — [Cloudflare Docs: Cloudflare for SaaS Plans](https://developers.cloudflare.com/cloudflare-for-platforms/cloudflare-for-saas/plans/)
- Ältere Drittquellen nennen 200 USD Basispreis und 2 USD pro Hostname. Das ist veraltet: Laut Cloudflare wurde der Hostname-Preis von 2 USD auf 0,10 USD gesenkt — [Cloudflare Blog WAF for SaaS](https://blog.cloudflare.com/waf-for-saas/); [Cloudflare Changelog](https://developers.cloudflare.com/changelog/product/cloudflare-for-saas/)

**Vercel / Netlify**
- Vercel Pro kostet 20 USD pro Nutzer/Seat und Monat inkl. 20 USD Nutzungsguthaben [Snippet] — [Vercel Docs Pro Plan](https://vercel.com/docs/plans/pro-plan); [Vendr](https://www.vendr.com/marketplace/vercel)
- Für Netlify Pro nennen die Quellen 19 bzw. 20 USD pro Nutzer/Monat (widersprüchlich). Netlify Pro hat laut einer Quelle unbegrenzt viele Mitglieder [Snippet] — [apicalculators Vercel vs Netlify](https://apicalculators.com/compare/vercel-vs-netlify); [getpricepulse](https://www.getpricepulse.com/companies/netlify-vs-vercel-pricing.html)
- Ein offizielles Limit für Custom Domains pro Projekt haben wir nicht gefunden. Eine Drittquelle nennt „unbegrenzt“ [Snippet] — [apicalculators](https://apicalculators.com/compare/vercel-vs-netlify)

### Inferences
- **Betriebslast VPS (Hostinger/Hetzner):** Der Gründer ist selbst für OS-Updates, Firewall, TLS-Automatik (z. B. Caddy/Traefik mit Let's Encrypt on-demand), Backups außerhalb des Servers, Monitoring und Restore-Tests verantwortlich. Weil Hostinger das VPS-Backup nur als Kulanz und mit 2 Wochen Aufbewahrung anbietet, sollte man zusätzlich ein externes Backup einplanen [SCHÄTZUNG: +3–10 €/Monat].
- **Empfohlene Architektur für Solo/Teilzeit [SCHÄTZUNG]:** Kundenseiten werden statisch generiert und über ein CDN ausgeliefert, Custom Domains/SSL laufen über Cloudflare for SaaS. Ein kleiner VPS (Hetzner CX23 ~5,49 € oder Hostinger KVM 2 ~9–15 USD) betreibt nur Editor, API und DB. Fällt der VPS aus, bleiben die Kundenseiten online. Das senkt das Uptime-Risiko deutlich.
- **Hostnamen-Rechnung:** Bei 100 Kunden mit je Apex + www werden es eventuell ~200 Hostnamen. Das ergibt ~10 USD/Monat Überschreitung (100 × 0,10 USD), je nachdem, ob der Apex als eigener Hostname zählt [SCHÄTZUNG].
- **DSGVO-Abwägung:** Hetzner (deutsches Unternehmen) ist datenschutzrechtlich am einfachsten. Hostinger (Sitz Litauen, EU), Cloudflare, Vercel und Netlify (US-Unternehmen) brauchen AVV/DPA und, bei den US-Anbietern, eine Prüfung der Drittlandübermittlung (DPF/SCC). Diese Prüfung muss man in die eigene Unterauftragsverarbeiter-Liste übernehmen. [Inferenz – rechtlich prüfen lassen]
- Vercel/Netlify werden pro Seat abgerechnet und sind eher für die eigene App gedacht. Für hunderte Kundendomains sind sie weniger attraktiv als Cloudflare for SaaS [Inferenz].

### Gaps
- Offizielle Hostinger-EUR-Preise und Verlängerungspreise: Seitenabruf blockiert (Domain www.hostinger.com nicht freigegeben). Ob der Hostinger-VPS-Standort wirklich in Frankfurt liegt, ist nicht bestätigt. Laut PCWelt-Snippet gibt es auch Standorte in FR/NL/LT/UK ([PCWelt](https://www.pcwelt.de/?p=2237321)).
- Hostinger-AVV/DPA nicht gefunden: im hPanel prüfen bzw. anfordern.
- Cloudflare Pages/Workers-Preise, Bunny.net-Preise und Coolify (Self-hosted/Cloud) wurden mangels Recherchebudget nicht recherchiert. Auch DPA-Details zu Cloudflare/Vercel/Netlify fehlen.
- Uptime-SLAs der Anbieter wurden nicht recherchiert.

---

## 2. KI-Kosten pro Kunde (LLM-API-Preise, Kosten pro Website-Generierung und pro Chat-Edit, EU-Datenverarbeitung)

### Takeaway
Die KI-Kosten sind bei einem Premium-Abo vernachlässigbar. Eine komplette Agentur-Website (8–10 Seiten) kostet mit einem Mittelklassemodell (Claude Sonnet 5.5, Mistral Medium 3.5) etwa 0,40–0,60 USD, mit Billigmodellen (Claude Haiku 5.5, GPT-5 mini, Mistral Small) nur wenige Cent. Ein Chat-Edit kostet etwa 0,003–0,11 USD [SCHÄTZUNG]. Engpass ist eher die EU-Datenverarbeitung: Die direkte Anthropic-API bietet laut den gefundenen Quellen keine garantierte EU-Inferenz. Mistral (EU-Anbieter) oder Claude über AWS Bedrock/Vertex in EU-Regionen sind die Alternativen.

### Cited Findings
**Preise (pro 1 Mio. Tokens, Input/Output)**
- Anthropic: Claude Opus 5.5 4 $/20 $, Claude Sonnet 5.5 2 $/10 $ (Cache-Reads 0,10 $), Claude Haiku 5.5 0,10 $/0,50 $ (bis 100K Prompt-Tokens, darüber 0,50 $/2,50 $). Ältere Modelle: Sonnet 4.6 3 $/15 $, Haiku 4.5 1 $/5 $ (Stand des Preis-Caches: 03.11.2026, aus der Claude-API-Referenz; Seite nicht direkt abgerufen) — [Anthropic Pricing](https://platform.claude.com/docs/en/about-claude/pricing)
- OpenAI GPT-5 mini: 0,25 $ Input / 2,00 $ Output, Cached Input 0,025 $, Batch 0,125 $/1,00 $. GPT-5.4 mini: 0,75 $/4,50 $ (Tracker-Stand Aug.–Okt. 2026; offizielle Seite im Snippet abgeschnitten) [Snippet] — [OpenAI Pricing](https://developers.openai.com/api/docs/pricing); [getdeploying GPT-5 mini](https://getdeploying.com/llms/gpt-5-mini); [pricepertoken GPT-5.4 mini](https://pricepertoken.com/pricing-page/model/openai-gpt-5.4-mini)
- Mistral Medium 3.5: 1,50 $/7,50 $ (Stand 03.11.2026, Release 30.04.2026) [Snippet] — [pricepertoken Mistral Medium 3.5](https://pricepertoken.com/pricing-page/model/mistral-ai-mistral-medium-3.5)
- Mistral Small: 0,20 $/0,60 $ (Stand 25.08.2026). Eine andere Quelle nennt für Small 3.1 Base 0,10 $/0,30 $. Für Mistral Large 3 widersprechen sich die Angaben (0,50 $/1,50 $ vs. 2 $/5 $) [Snippet] — [anotherwrapper Mistral Small](https://anotherwrapper.com/llm-pricing/mistral-small-2409); [cloudzero](https://cloudzero.com/blog/mistral-api-pricing); [anotherwrapper Large](https://anotherwrapper.com/tools/llm-pricing/mistral-large)

**EU-Datenverarbeitung**
- Anthropic: Der Parameter `inference_geo` steuert pro Request, wo die Inferenz läuft (ab Claude 4.6). Als Workspace-Geo ist derzeit nur „us“ verfügbar [Snippet] — [Anthropic Docs: Data residency](https://platform.claude.com/docs/en/build-with-claude/data-residency)
- Laut einer GDPR-Übersicht vom Juni 2026 bietet die direkte Anthropic-API nur die Geos „us“ und „global“. Bei „global“ kann die Inferenz in Europa laufen, das ist aber nicht garantiert. Eine EU-Region war laut Community-Quellen geplant bzw. auf Warteliste, ein Launch ist nicht bestätigt [Snippet] — [Sonomos: Claude EU Data Residency 2026](https://sonomos.ai/blog/claude-eu-data-residency-2026/); [Claude's Daily Diary Feb 2026](https://gsp4dcs2.github.io/claudes-daily-diary/articles/2026/02/2026-02-02.html)
- Als Workaround wird Claude über AWS Bedrock in eu-central-1 (Frankfurt), eu-west-1 oder eu-west-3 bzw. über Google Vertex AI in EU-Regionen empfohlen [Snippet] — [cloudmagazin 22.04.2026](https://www.cloudmagazin.com/en/2026/04/22/aws-bedrock-anthropic-api-or-self-hosted-ai-inference/); [Omnifact](https://omnifact.ai/blog/feature-drop-eu-data-residency-vertex-ai)
- Bedrock/Vertex haben eine eigene Preisgestaltung, die von den Anthropic-Listenpreisen abweichen kann — [AWS Bedrock Pricing](https://aws.amazon.com/bedrock/pricing/)

### Inferences (Kostenmodell) [SCHÄTZUNG]
**Token-Annahmen Website-Generierung (8–10 Seiten Copy + Struktur-JSON):**
- 10 Calls × ~8.000 Input-Tokens (System-Prompt, Agentur-Briefing, Seitenschema, Stilvorgaben) = **~80.000 Input**
- 10 × ~2.500 Output (Copy + JSON) + ~50 % Reasoning/Thinking-Aufschlag = **~40.000 Output**

| Modell | Input-Kosten | Output-Kosten | **Pro Website** |
|---|---|---|---|
| Claude Opus 5.5 | 0,32 $ | 0,80 $ | **~1,12 $** |
| Claude Sonnet 5.5 | 0,16 $ | 0,40 $ | **~0,56 $** |
| Mistral Medium 3.5 | 0,12 $ | 0,30 $ | **~0,42 $** |
| GPT-5 mini | 0,02 $ | 0,08 $ | **~0,10 $** |
| Mistral Small | 0,016 $ | 0,024 $ | **~0,04 $** |
| Claude Haiku 5.5 | 0,008 $ | 0,02 $ | **~0,03 $** |

Auch mit 3 Neugenerierungen pro Kunde bleiben es unter 2 $ (Sonnet-Klasse) einmalig.

**Token-Annahmen Chat-Edit:** ~15.000 Input (aktuelle Seite als JSON + Chatverlauf + System-Prompt) und ~2.500 Output (geänderte Sektion + Thinking).

| Modell | Pro Edit | 50 Edits/Kunde/Monat |
|---|---|---|
| Claude Opus 5.5 | ~0,11 $ | ~5,50 $ |
| Claude Sonnet 5.5 | ~0,055 $ (mit Prompt-Caching eher ~0,03 $) | ~1,50–2,75 $ |
| Mistral Medium 3.5 | ~0,04 $ | ~2,05 $ |
| GPT-5 mini | ~0,009 $ | ~0,45 $ |
| Claude Haiku 5.5 | ~0,003 $ | ~0,14 $ |

- Hochgerechnet mit Sonnet-Klasse: 20 Kunden ≈ 30–55 $/Monat, 100 Kunden ≈ 150–275 $/Monat [SCHÄTZUNG]. Bei einem Abo von z. B. 99–199 €/Monat sind das <3 % des Umsatzes.
- Ausreißer (Power-User mit hunderten Edits, Bild-Inputs, lange Verläufe) lassen sich über Edit-Kontingente oder Fair-Use in den AGB begrenzen.
- Modell-Routing spart Kosten: Erstgenerierung mit Sonnet-/Medium-Klasse, kleine Edits mit Haiku/Small [Inferenz].
- DSGVO: Agentur-Website-Copy enthält kaum personenbezogene Daten (eventuell Teamnamen/Fotos). Das Risiko ist geringer als bei Kundendaten-Verarbeitung, ein DPA/AVV mit dem LLM-Anbieter und dessen Aufnahme in die Subprozessorliste sind trotzdem nötig [Inferenz – rechtlich prüfen lassen].

### Gaps
- Offizielle Mistral-Preisseite und Mistral-DPA/EU-Hosting-Details wurden nicht direkt verifiziert (nur Drittquellen).
- OpenAI EU-Data-Residency-Optionen wurden nicht recherchiert.
- Bedrock-/Vertex-EU-Preise für Claude wurden nicht konkret recherchiert.
- Bildgenerierung (Hero-Bilder etc.) ist in den Kosten nicht enthalten.

---

## 3. Sonstige laufende Kosten und monatliche Fixkosten bei 0 / 20 / 100 Kunden

### Takeaway
Die Fixkosten liegen bei 0 Kunden bei grob 60–200 €/Monat. Treiber sind Versicherung und Steuerberatung/Buchhaltung, nicht die Infrastruktur. Mit 20 bzw. 100 Kunden steigen vor allem die variablen Kosten: Zahlungsgebühren, KI und Hostnamen. Für reines B2B-DACH-Geschäft ist Stripe (1,5 % + 0,25 € für EWR-Karten, 0,35 € für SEPA) deutlich günstiger als ein Merchant of Record (Paddle/Lemon Squeezy: 5 % + 0,50 $). Den MoR-Vorteil (globale VAT-Abwicklung) braucht ein B2B-Geschäft mit Reverse Charge kaum.

### Cited Findings
- Stripe: 1,5 % + 0,25 € für europäische Standardkarten, 2,5 % + 0,25 € für UK-Karten — [Stripe (DE-LU) Kreditkartenzahlungen](https://stripe.com/de-lu/lp/payments/credit-card-processing)
- Stripe SEPA-Lastschrift: laut Drittquellen 0,35 € pro Transaktion. Premium- und internationale Karten werden je nach Quelle mit 1,9–2,8 % bzw. 3,15–3,25 % + 0,25 € angegeben, Währungsumrechnung +2 % [Snippet] — [Sellfy Stripe-Gebührenrechner](https://sellfy.com/de/tools/stripe-gebuehrenrechner/); [meetergo](https://meetergo.com/blog/stripe)
- Stripe Tax kostet etwa 0,5 % zusätzlich. Es berechnet Steuern, registriert und meldet aber nicht für den Händler [Snippet] — [dev.to Fee Comparison 2026](https://dev.to/jettfu/stripe-vs-paddle-vs-lemon-squeezy-fee-comparison-2026-2c77)
- Paddle und Lemon Squeezy sind Merchants of Record mit je 5 % + 0,50 $ pro Transaktion. Paddle bietet Custom Pricing ab 100K $ MRR [Snippet] — [Dodo Payments: Paddle vs Lemon Squeezy](https://dodopayments.com/blogs/paddle-vs-lemon-squeezy/); [apicalculators](https://apicalculators.com/compare/paddle-vs-lemonsqueezy)
- Lemon Squeezy gehört zu Stripe (Datum widersprüchlich: Ende 2023 vs. Juli 2024). Stripe Managed Payments (eigenes MoR-Produkt) ging laut einer Quelle im Februar 2026 in die Public Preview [Snippet] — [alexcloudstar MoR 2026](https://alexcloudstar.com/md/blog/merchant-of-record-indie-saas-2026/)
- Nachteil des MoR: Auf Belegen erscheint der Name des MoR, und man hat weniger Kontrolle über Preisdarstellung und Refunds [Snippet] — [dev.to devtoolpicks](https://dev.to/devtoolpicks/lemon-squeezy-vs-stripe-vs-paddle-which-should-solo-devs-use-in-2026-2jm9)
- IT-Haftpflicht (Vermögensschaden): exali nennt als kleinste Variante netto ca. 207 €/Jahr, Durchschnitt IT/Medien ca. 250 € [Snippet] — [exali: Berufshaftpflicht Kosten](https://exali.de/Info-Base/berufshaftpflicht-kosten)
- Vermögensschadenhaftpflicht inkl. Betriebshaftpflicht ab 476 €/Jahr. Reine Betriebshaftpflicht ab 89,25 € [Snippet] — [Gründerküche](https://www.gruenderkueche.de/fachartikel/die-4-wichtigsten-gewerbeversicherung-fuer-it-freelancer/)
- Hiscox gewährt Startups 15 % Rabatt im ersten Jahr [Snippet] — [für-gründer.de](https://www.fuer-gruender.de/blog/richtig-versichern/). Der Tarif „IT Freelancer“ gilt bis 125.000 € Umsatz [Snippet] — [it-daily](https://www.it-daily.net/?p=7835)
- Für Softwareprodukt-Unternehmen nennt eine US-Quelle Tech-E&O-Prämien von 1.000–5.000 USD/Jahr. US-Markt, daher nur eingeschränkt übertragbar [Snippet] — [beancount.io](https://beancount.io/de/blog/2026/09/19/tech-errors-omissions-insurance-developers-consultants-guide)

### Inferences – Fixkostenmodell [SCHÄTZUNG, Positionen ohne Quelle sind Erfahrungswerte und nicht recherchiert]

Annahme: Abo 149 €/Monat netto (nur Rechenbeispiel), Hybrid-Architektur (statisch + Cloudflare for SaaS + kleiner VPS), Sonnet-Klasse, Stripe mit SEPA/Karte gemischt (~1,2 € pro Zahlung).

| Posten (€/Monat) | 0 Kunden | 20 Kunden | 100 Kunden |
|---|---|---|---|
| VPS (Hostinger KVM 2 bzw. Hetzner CX23 → bei 100 eventuell größerer Plan) | 6–14 | 6–14 | 15–35 |
| Externes Backup/Storage | 3 | 3–5 | 5–10 |
| Cloudflare for SaaS (100 Hostnamen frei) | 0 | 0 | 0–9 |
| Eigene Domain(s) | 1–2 | 1–2 | 1–2 |
| Transaktionale E-Mail + Geschäfts-Postfach | 0–10 | 5–15 | 15–30 |
| KI-API (s. Abschnitt 2) | 0–5 (Tests) | 30–50 | 140–250 |
| Zahlungsgebühren Stripe (~1,2 €/Zahlung) | 0 | ~25 | ~120 |
| (Alternativ MoR 5 % + 0,50 $: ~7,90 €/Zahlung) | (0) | (~160) | (~790) |
| IT-Haftpflicht/Vermögensschaden (207–500 €/Jahr) | 17–42 | 17–42 | 25–60 |
| Buchhaltungssoftware | 10–20 | 10–20 | 10–20 |
| Steuerberater (eventuell nur Jahresabschluss) | 0–100 | 50–150 | 100–250 |
| Rechtstexte (AGB/AVV-Generator oder Anwalt, umgelegt) | 10–40 | 10–40 | 10–40 |
| Tools (Monitoring, Error-Tracking, Git, Design) | 0–30 | 20–50 | 30–80 |
| **Summe (mit Stripe)** | **~50–270** | **~180–420** | **~470–900** |
| Umsatz bei 149 €/Kunde | 0 | 2.980 | 14.900 |

- Die Infrastruktur bleibt bis 100 Kunden klein (<100 €/Monat). Versicherung, Steuerberater und Zahlungsgebühren dominieren.
- Bei B2B-Kunden in DE/AT/CH bringt ein MoR wenig: Innerhalb der EU gilt für B2B-Leistungen meist Reverse Charge, CH liegt außerhalb der EU. Er kostet bei 100 Kunden aber ~670 €/Monat mehr als Stripe [Inferenz – steuerlich prüfen lassen].
- Bei Premiumpreisen sollte man SEPA-Lastschrift oder Rechnung/Überweisung (Jahresabo) bevorzugen, um Gebühren zu senken [Inferenz].

### Gaps
- Stripe-Billing-Gebühr (prozentualer Aufschlag für Abos) wurde nicht gefunden: offizielle Seite stripe.com/de/pricing prüfen.
- Preise für transaktionale E-Mail (Postmark, Brevo, AWS SES), Buchhaltungssoftware (lexoffice/sevdesk), Steuerberater und Gewerbeanmeldung wurden nicht recherchiert, die Werte in der Tabelle sind Schätzungen.
- Konkrete Prämien für Cyber-/IT-Haftpflicht speziell für SaaS-Anbieter mit Hosting in DE fehlen. Ein Angebot einholen (Deckung inkl. Datenschutzverletzung/Betriebsunterbrechung beim Kunden).

---

## 4. Recht/Compliance in Deutschland (Gewerbe, USt., AGB, AVV, Impressum/Datenschutz, Cookies, BFSG, AI Act, Haftung für KI-Copy)

### Takeaway
Gewerbe anmelden und von Anfang an die Regelbesteuerung prüfen: Kunden sind Unternehmen, die die Vorsteuer abziehen. Die Kleinunternehmerregelung (25.000 € Vorjahr / 100.000 € laufendes Jahr, harte Grenze) bringt deshalb kaum einen Vorteil, und schon 20 Kunden × 149 € ≈ 35.800 €/Jahr liegen über 25.000 €. Pflicht-Dokumente sind B2B-AGB mit Haftungsbegrenzung, ein AVV nach Art. 28 DSGVO mit jeder Agentur (der Gründer hostet als Auftragsverarbeiter) und eine Subprozessorliste (VPS, CDN, LLM, Mail, Payment). Das BFSG greift für reine B2B-Leistungen grundsätzlich nicht, die Grauzone ist aber eng. AI-Act-Art.-50-Pflichten gelten seit 02.08.2026, mit Übergang bis 02.12.2026 für die maschinenlesbare Kennzeichnung bei Altsystemen. **Alles rechtlich prüfen lassen.**

### Cited Findings
**Umsatzsteuer/Kleinunternehmer**
- Seit 01.01.2025 gilt nach § 19 UStG: Der Vorjahresumsatz darf höchstens 25.000 € betragen (vorher 22.000 €), der Umsatz im laufenden Jahr höchstens 100.000 € — [IHK München: Grenzwerte beachten](https://www.ihk-muenchen.de/magazin/solo-selbststaendige/unternehmen-in-oberbayern/grenzwerte-beachten.html)
- Die 100.000-€-Grenze wirkt sofort: Schon der Umsatz, mit dem die Grenze überschritten wird, unterliegt der Regelbesteuerung. Die frühere Prognoseregel (50.000 €) ist entfallen [Snippet] — [Lexware: Kleinunternehmerregelung](https://www.lexware.de/wissen/buchhaltung-finanzen/kleinunternehmerregelung/)
- Im Gründungsjahr gilt laut Finanzverwaltung die 25.000-€-Grenze. Eine Hochrechnung auf 12 Monate gibt es seit 2025 laut Lexware nicht mehr. Eine andere Quelle widerspricht mit einer Hochrechnungsregel [Snippet] — [Lexware](https://www.lexware.de/wissen/buchhaltung-finanzen/kleinunternehmerregelung/); contradicted by [selbststaendigkeit.de](https://selbststaendigkeit.de/buchhaltung-fuer-gruender/wann-kleinunternehmer/)

**AVV / Datenschutz / Cookies**
- Hat ein Webhoster Zugriff auf Kundendaten, liegt Auftragsverarbeitung vor und ein AV-Vertrag ist nötig. Ist der Zugriff ausgeschlossen, liegt keine Auftragsverarbeitung vor [Snippet] — [IT-Recht-Kanzlei: AV-Vertrag Datendrittverarbeitung](https://www.it-recht-kanzlei.de/av-vertrag-datendrittverarbeitung.html)
- Den Mindestinhalt regelt Art. 28 DSGVO, elektronische Form genügt [Snippet] — [IT-Recht-Kanzlei](https://www.it-recht-kanzlei.de/av-vertrag-datendrittverarbeitung.html)
- Die Datenschutzaufsicht Niedersachsen bekommt regelmäßig Anfragen, weil AVV von Webhostern nicht DSGVO-konform sind, und stellt eine Checkliste bereit — [LfD Niedersachsen](https://lfd.niedersachsen.de/download/186200)
- Muster-AVV von Hostern als Vorlage: [Hostsharing](https://Hostsharing.net/downloads/hostsharing-besondere-bedingungen-zur-auftragsverarbeitung.pdf); [Hostweb](https://www.hostweb.de/media/AV_Hostweb_201805_final_web.pdf)
- Für unbedingt erforderliche Cookies ist keine Einwilligung nötig (§ 25 Abs. 2 S. 2 TDDDG). Für die anschließende Verarbeitung personenbezogener Daten braucht es aber eine DSGVO-Rechtsgrundlage. Ein Consent-Tool kann selbst Auftragsverarbeitung sein — [DFN Leitfaden Website-Cookies (08/2026)](https://recht.dfn.de/wp-content/uploads/2026/08/Website-Cookies-DSGVO.pdf); [IT-Recht-Kanzlei](https://www.it-recht-kanzlei.de/av-vertrag-datendrittverarbeitung.html)
- Die Datenschutzerklärung der Kundenseiten braucht einen Abschnitt „Externes Hosting“, in dem der Hoster genannt wird — [eRecht24: Externes Hosting](https://www.e-recht24.de/dsg/12643-externes-hosting.html); [eRecht24: Webhoster und Datenschutz](https://www.e-recht24.de/datenschutz/13053-webhoster-und-datenschutz.html)

**BFSG (Barrierefreiheit)**
- Das BFSG gilt nach § 1 Abs. 3 nur für Dienstleistungen im elektronischen Geschäftsverkehr, die für Verbraucher erbracht werden. Reine B2B-Angebote fallen nicht darunter, das B2B-Angebot muss aber klar erkennbar sein [Snippet] — [IHK Schwaben: BFSG](https://www.ihk.de/schwaben/produktmarken/beratung-und-service/recht-und-steuern/digitalisierung-und-e-commerce/barrierefreiheitsstaerkungsgesetz-6292836); [e-recht24 BFSG](https://www.e-recht24.de/ecommerce/13236-barrierefreiheitsstaerkungsgesetz.html)
- Im Zweifel wird B2C angenommen: Schon die bloße Möglichkeit, dass Verbraucher die Leistung nutzen, kann den Anwendungsbereich eröffnen [Snippet] — [BTL Rechtsanwälte](https://www.btl-recht.de/blog/bfsg-wer-ist-betroffen-websites-onlineshops/)
- Rein informative Websites ohne Bestell-, Buchungs- oder Vertragsschlussfunktion fallen nicht allein deshalb unter das BFSG [Snippet] — [ZDH: Barrierefreiheit von Webseiten](https://www.zdh.de/ueber-uns/fachbereich-organisation-und-recht/praxis-recht-/-leitfaeden/praxis-recht-barrierefreiheit-von-webseiten/)

**AI Act (KI-VO) Art. 50**
- Die meisten Transparenzpflichten nach Art. 50 gelten weiter ab 02.08.2026. Der Digital Omnibus verschiebt vor allem die Hochrisiko-Pflichten [Snippet] — [Jones Walker](https://www.joneswalker.com/en/insights/blogs/ai/yes-august-2-still-matters-the-eu-approved-a-high-risk-ai-delay-but-most-trans.html?id=102nbon)
- Für generative KI-Systeme, die vor dem 02.08.2026 auf dem Markt waren, gilt für die maschinenlesbare Kennzeichnung (Art. 50 Abs. 2) eine Frist bis 02.12.2026. Art. 50 Abs. 1, 3 und 4 bleiben unverändert [Snippet] — [Ropes & Gray 08/2026](https://www.ropesgray.com/en/insights/viewpoints/2026/08/102nfqm/you-talkin-to-me-operationalising-the-eu-ai-acts-transparency-obligations)
- Anbieter betten die Kennzeichnung bei der Erzeugung ein, Betreiber (Deployer) machen sie bei der Veröffentlichung sichtbar. Der Omnibus ist laut Quellen Verordnung (EU) 2026/1744 (Angaben zu Daten schwanken) [Snippet] — [compliancehub.wiki](https://compliancehub.wiki/eu-ai-act-article-50-transparency-digital-omnibus-2026/)
- Ältere Quellen (TÜV) nannten noch Vorschlagsfristen (02.11.2026 bzw. 02.02.2027). Diese sind durch das Ergebnis 02.12.2026 überholt — [TÜV Consulting](https://consulting.tuv.com/aktuelles/ki-im-fokus/transparenzpflichten-eu-ai-act-art-50)

### Inferences [alles rechtlich prüfen lassen]
- **Gewerbe:** Ein SaaS mit Hosting ist eine gewerbliche Tätigkeit (keine freiberufliche). Das heißt Gewerbeanmeldung, IHK-Mitgliedschaft und eventuell Gewerbesteuer über dem Freibetrag. Wer angestellt ist (Teilzeit-Gründung), sollte den Arbeitsvertrag auf Nebentätigkeitsregeln prüfen. Für beides wurde in dieser Recherche keine Quelle geprüft.
- **USt.:** Bei B2B-Kunden ist die Regelbesteuerung praktisch neutral (Kunde zieht Vorsteuer ab) und erlaubt den Vorsteuerabzug auf eigene Kosten (Server, Tools, Hardware). Für Kunden in AT gilt meist Reverse Charge, für CH-Kunden der Leistungsort-Grundsatz (§ 3a UStG). Mit Steuerberater klären.
- **AGB B2B-SaaS – Kernpunkte:** Leistungsbeschreibung und Verfügbarkeit (keine 99,9 %-Zusage ohne Infrastruktur dafür), Haftungsbegrenzung (B2B-AGB-Kontrolle beachten: Kardinalpflichten und Vorsatz/grobe Fahrlässigkeit lassen sich nicht ausschließen), Verantwortung des Kunden für Inhalte, Impressum und Rechtstexte seiner Seite, KI-Output als Entwurf mit Prüfpflicht des Kunden, Fair-Use bei KI-Edits, Kündigung/Datenexport, Domain-Übertragung bei Kündigung, Laufzeit/Zahlung, Gerichtsstand, deutsches Recht.
- **AVV:** Der Gründer ist Auftragsverarbeiter der Agenturen, z. B. für Kontaktformular-Daten und Server-Logs von Besuchern der Agentur-Website. Nötig sind ein eigener AVV, TOMs und eine Subprozessorliste (Hostinger/Hetzner, Cloudflare, LLM-Anbieter, E-Mail-Dienst). Der LLM-Anbieter ist nur dann Subprozessor, wenn personenbezogene Daten an ihn gehen.
- **Impressum/Datenschutz der Kundenseiten:** Verantwortlich ist die Agentur als Seitenbetreiberin (Impressumspflicht seit 2024 nach § 5 DDG statt TMG – nicht in dieser Recherche verifiziert). Der Builder sollte Pflichtseiten-Vorlagen und Felder anbieten, die Inhalte aber nicht rechtsverbindlich erstellen, oder auf eRecht24/IT-Recht-Kanzlei verweisen. Der Footer-Link zu Impressum/Datenschutz sollte erzwungen werden.
- **Cookies/Consent:** Der Builder sollte standardmäßig ohne einwilligungspflichtige Cookies und Tracker auskommen (keine Google Fonts von Google-Servern, kein Analytics ohne Consent, Fonts selbst hosten). Dann ist auf den Kundenseiten kein Consent-Banner nötig. Will eine Agentur Tracking einbauen, muss sie selbst ein Consent-Tool integrieren.
- **BFSG:** Agentur-Websites ohne Online-Vertragsschluss für Verbraucher fallen wahrscheinlich nicht unter das BFSG. Kommen Online-Buchung oder -Vertragsschluss mit Verbrauchern dazu, kann es anders aussehen. Der Builder selbst ist ein B2B-Dienst. Accessibility-Defaults (Kontraste, Alt-Texte, Semantik) sind trotzdem ein Verkaufsargument, weil die Agenturen für ihre Shop-Kunden BFSG-Kompetenz zeigen müssen.
- **AI Act:** Als Anbieter eines generativen KI-Systems (eigenes Produkt auf LLM-Basis) treffen den Gründer eventuell die Pflichten aus Art. 50 Abs. 2 zur maschinenlesbaren Kennzeichnung von KI-Output. Wie das bei Text in Websites umsetzbar ist und ob Ausnahmen gelten (z. B. assistierende Bearbeitung), ist offen. Art. 50 Abs. 4 (Kennzeichnung durch Betreiber) betrifft nach unserem Verständnis Texte zu Angelegenheiten von öffentlichem Interesse und entfällt bei menschlicher Prüfung bzw. redaktioneller Verantwortung. Marketing-Copy einer Agentur fällt vermutlich nicht darunter. Gesetzestext prüfen.
- **Haftung für KI-Copy:** Mögliche Risiken sind falsche Leistungsversprechen (UWG/Irreführung), erfundene Referenzen oder Kundenlogos, Marken- und Urheberrechtsverletzungen sowie unzulässige Werbeaussagen. Vertraglich sollte gelten: Der Kunde prüft und gibt frei, und er ist für die veröffentlichten Inhalte verantwortlich. Technisch sollte die KI keine Kundennamen, Zahlen oder Testimonials erfinden, sondern Platzhalter setzen. IT-Haftpflicht mit Deckung für Vermögensschäden Dritter abschließen.

### Gaps
- Für AGB-Muster für B2B-SaaS, Gewerbeanmeldungskosten, IHK-Beitrag und die DDG-Impressumsnorm haben wir keine Quelle geprüft.
- Ob die Pflichten aus Art. 50 Abs. 2 für Text-Output eines kleinen SaaS-Anbieters konkret gelten (Ausnahmen, KMU-Erleichterungen, technische Standards), ist nicht geklärt. Fachanwalt fragen.
- Umsatzsteuerliche Behandlung von CH-Kunden und Kleinunternehmer mit EU-B2B-Kunden: nicht recherchiert.

---

## 5. Realistischer Bauaufwand: Voll-MVP (Builder + KI + Hosting) vs. Concierge-MVP

### Takeaway
Indie-Gründer bringen schmale MVPs meist in 2–8 Wochen Teilzeit live. Ein Website-Builder mit KI-Generierung, Live-Chat-Edits, Multi-Tenant-Hosting, Custom Domains/SSL und Billing ist deutlich breiter und dürfte für einen Teilzeit-Solo-Gründer eher 3–6 Monate bis zur zahlungsfähigen Version brauchen [SCHÄTZUNG]. Damit ist ein großer Teil des 6-Monats-Fensters für 20 Kunden verbraucht. Ein Concierge-MVP (Seiten manuell mit Framer/Webflow/Astro-Templates plus KI-Assistenz bauen und als Premium-Abo verkaufen) kann in Wochen erste Zahlungen bringen und validiert Zahlungsbereitschaft und Bedarf, bevor das Produkt gebaut wird.

### Cited Findings
- Der Serien-Indie-Hacker Mubashar Iqbal begrenzt jedes Projekt auf 2–4 Wochen und verwirft es, wenn bis dahin kein Launch erfolgt ist [Snippet] — [Indie Hackers: $10k+/mo after 120 side hustles](https://www.indiehackers.com/post/starting-up/making-10k-mo-as-a-full-time-founder-after-building-120-side-hustles-FXnE02qqeOq385VtMxmq)
- Ein App-Builder-Gründer hatte die erste Version nach ca. 2 Wochen live und erreichte innerhalb eines Jahres 10k $ MRR [Snippet] — [Indie Hackers: Launching an app builder in 2 weeks](https://www.indiehackers.com/post/tech/launching-an-app-builder-in-2-weeks-and-hitting-10k-mrr-within-a-year-gRWT2S68TIQwMvb6Xxt4)
- Tigran Hakobyan brauchte fast 2 Monate Teilzeit für die erste Version von Cronhub [Snippet] — [freeCodeCamp: Reflections on being an indie hacker](https://www.freecodecamp.org/news/reflections-on-being-an-indie-hacker-95e19d2edb47/)
- Ausreißer: TypingMind-MVP in 2 Tagen, Audio Pen in 12 Stunden. Beides sind Ausnahmen [Snippet] — [app-dev-and-marketing](https://app-dev-and-marketing.pages.dev/the-app-i-built-in-12-hours-makes-15k-month)
- Ein Gründer sagt rückblickend, er habe zu viel Zeit in Features gesteckt und hätte früher auf Marketing und Nutzerfeedback setzen sollen [Snippet] — [slowsort: My solo founder experience](https://slowsort.github.io/2022/03/11/indie-hacker-journey)

### Inferences [SCHÄTZUNG]
- **Komponenten Voll-MVP:** Auth/Multi-Tenant, Seitenmodell/Templates (Block-System), KI-Generierung mit strukturiertem Output, Chat-Edit mit Diff/Undo, Rendering/Publishing (statisch), Custom-Domain-Onboarding (DNS-Anleitung, Verifizierung, SSL), Formulare und E-Mail, Billing (Stripe), Backups/Monitoring, Rechtstexte. Jede Komponente kostet einige Tage bis Wochen. Bei ~10–15 h/Woche sind 3–6 Monate realistisch, mit KI-Coding-Tools eventuell am unteren Ende.
- **Concierge-MVP:** Der Gründer baut für die ersten 3–10 Agenturen Seiten mit bestehenden Tools (Framer/Webflow/Astro-Templates + LLM für Copy) und verkauft dasselbe Premium-Abo (Hosting + Änderungen „per Chat“, anfangs z. B. per Slack/E-Mail, die der Gründer selbst umsetzt). Vorteile: Umsatz in Wochen, echte Anforderungen für das Produkt, Templates als Vorarbeit. Nachteil: Die Zeit pro Kunde skaliert nicht, und Lizenzbedingungen der Tools (Weiterverkauf, Client-Billing) müssen geprüft werden.
- **Empfehlung für das 6-Monats-Ziel:** Monate 1–2 Concierge mit 3–5 zahlenden Agenturen, parallel das Produkt schmal bauen (KI-Generierung + Chat-Edit + statisches Hosting + Cloudflare for SaaS). Ab Monat 3–4 Concierge-Kunden migrieren.

### Gaps
- Wir haben keine konkreten Fallstudien zu Solo-Gründern speziell von Website-Buildern mit KI und Custom-Domain-Hosting gefunden. Die Zeitangaben stammen aus allgemeinen App-/SaaS-Projekten.
- Framer- und Webflow-Preise und Lizenzbedingungen (Client-Billing, Weiterverkauf von Hosting) wurden nicht recherchiert.
