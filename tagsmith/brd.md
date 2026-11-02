---
client: Brand new
template: government-default-brd
---
# Business Requirements — Brand new

<!-- Managed by Tagsmith. Edit rows freely; keep each ID stable. IDs that are multiples of 100 are category headers. eVar / Event / prop hold the allocated Adobe variables (comma-separated). -->

| ID | Category | Requirement | Scope | Priority | Phase | Data Format | Data Example | Notes | Reserved | Report Populated | eVar | Event | prop |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 100 | Page Tagging |  |  |  |  |  |  |  |  |  |  |  |  |
| 101 | Page Tagging | Instrument Adobe Analytics across all website pages and key user interactions. |  | Medium | 1 |  |  | FR-AN-01 |  |  |  |  |  |
| 102 | Page Tagging | Capture all events required to measure the KPIs defined in Section 5. |  | Medium | 1 |  |  | FR-AN-02 |  |  |  |  |  |
| 103 | Page Tagging | Capture responsive, mobile-first page delivery across desktop and mobile viewports per approved wireframes. |  | Medium | 1 |  |  | FR-PW-01 |  |  |  |  |  |
| 104 | Page Tagging | Track display of festival programme and installation listings including title, description, venue, dates and times. |  | Medium | 1 |  |  | FR-PW-03 |  |  |  |  |  |
| 105 | Page Tagging | Track the Klook ticketing call-to-action directing visitors off-site; no ticketing built on the SNF website. |  | Medium | 1 |  |  | FR-PW-02 |  |  |  |  |  |
| 106 | Page Tagging | Track presence of the standard government disclaimer on all pages. |  | Medium | 1 |  |  | FR-PW-07; exact text provided by NHB / Heritage SG |  |  |  |  |  |
| 107 | Page Tagging | Track Privacy Policy page views documenting personal data collected, purpose, retention and visitor rights under PDPA. |  | Medium | 1 |  |  | FR-PW-05; distinct from Cookie Policy (NFR-PDPA-12) |  |  |  |  |  |
| 108 | Page Tagging | Track Terms of Use page views. |  | Medium | 1 |  |  | FR-PW-06; content provided and approved by NHB / Heritage SG |  |  |  |  |  |
| 109 | Page Tagging | Track compliance with Heritage SG brand guidelines across pages. |  | Medium | 1 |  |  | FR-PW-04; per 00_brand_guidelines_v1.md |  |  |  |  |  |
| 200 | User Identity |  |  |  |  |  |  |  |  |  |  |  |  |
| 201 | User Identity | Capture visitor email registration verified via one-time code or link sent to email. |  | Medium | 1 |  |  | FR-REG-01; mobile/SMS OTP out of scope (gov.sg approved sender required) |  |  |  |  |  |
| 202 | User Identity | Capture mobile-optimised email registration flow completion. |  | Medium | 1 |  |  | FR-REG-02 |  |  |  |  |  |
| 203 | User Identity | Track that registration is optional and unregistered visitors retain full unrestricted content access. |  | Medium | 1 |  |  | FR-REG-03; registration unlocks personalisation only, never gates content |  |  |  |  |  |
| 204 | User Identity | Capture visitor profile management via Adobe Experience Platform and Real-Time CDP. |  | Medium | 1 |  |  | Scope §6.1 |  |  |  |  |  |
| 300 | Consent |  |  |  |  |  |  |  |  |  |  |  |  |
| 301 | Consent | Capture the three-tier consent model (Tier 0 Functional, Tier 1 Festival Marketing, Tier 2 Year-Round NHB) at registration. |  | Medium | 1 |  |  | FR-REG-04 |  |  |  |  |  |
| 302 | Consent | Enforce unchecked-by-default consent checkboxes with separate, unbundled Tier 1 and Tier 2 statements requiring positive action. |  | Medium | 1 |  |  | FR-REG-05 |  |  |  |  |  |
| 303 | Consent | Capture consent withdrawal via self-service profile settings, effective immediately. |  | Medium | 1 |  |  | FR-REG-06 |  |  |  |  |  |
| 304 | Consent | Maintain a consent log capturing visitor ID, consent type, action, timestamp and hashed IP address. |  | Medium | 1 |  |  | FR-REG-07; PDPA audit evidence |  |  |  |  |  |
| 400 | Navigation & Map |  |  |  |  |  |  |  |  |  |  |  |  |
| 401 | Navigation & Map | Track the interactive Bras Basah–Bugis precinct map displaying all programme and installation locations. |  | Medium | 1 |  |  | FR-MAP-01 |  |  |  |  |  |
| 402 | Navigation & Map | Track map implementation by Adobe using MapBox. |  | Medium | 1 |  |  | FR-MAP-02; Accenture procures MapBox license and style system |  |  |  |  |  |
| 403 | Navigation & Map | Track proximity-based sorting of map and listings by walking distance when location permission is granted. |  | Medium | 1 |  |  | FR-MAP-03 |  |  |  |  |  |
| 404 | Navigation & Map | Track default listing behaviour without degradation when visitors deny location permission. |  | Medium | 1 |  |  | FR-MAP-04 |  |  |  |  |  |
| 405 | Navigation & Map | Display live per-venue crowd density indicators derived from Adobe Analytics real-time session data. |  | Medium | C |  |  | FR-MAP-05 / FR-PERS-08; no raw GPS stored server-side |  |  |  |  |  |
| 406 | Navigation & Map | Derive per-venue crowd density signals from real-time Adobe Analytics session data for live crowd indicators. |  | Medium | Phase C |  |  | FR-AN-04 |  |  |  |  |  |
| 500 | Trails & Itinerary |  |  |  |  |  |  |  |  |  |  |  |  |
| 501 | Trails & Itinerary | Track presentation of curated self-guided trails for selection and navigation. |  | Medium | 1 |  |  | FR-TRAIL-01 |  |  |  |  |  |
| 502 | Trails & Itinerary | Capture registered visitors saving and following a trail with progress tracked via QR check-ins. |  | Medium | 1 |  |  | FR-TRAIL-02 |  |  |  |  |  |
| 503 | Trails & Itinerary | Capture creation of custom itineraries by adding chosen programmes and installations. |  | Medium | 1 |  |  | FR-TRAIL-03 |  |  |  |  |  |
| 504 | Trails & Itinerary | Detect itinerary conflicts and inefficiencies and surface dismissible, non-blocking inline optimisation suggestions. |  | Medium | 1 |  |  | FR-TRAIL-04 |  |  |  |  |  |
| 505 | Trails & Itinerary | Capture itinerary sharing via native device share without social platform OAuth. |  | Medium | 1 |  |  | FR-TRAIL-05 |  |  |  |  |  |
| 506 | Trails & Itinerary | Capture shared itineraries viewable without authentication and one-tap adoption triggering a light registration prompt. |  | Medium | 1 |  |  | FR-TRAIL-06 |  |  |  |  |  |
| 507 | Trails & Itinerary | Surface itineraries with 10 or more unique festival-window adoptions as Community Picks on the Trails page. |  | Medium | 1 |  |  | FR-TRAIL-07 |  |  |  |  |  |
| 600 | QR Check-in |  |  |  |  |  |  |  |  |  |  |  |  |
| 601 | QR Check-in | Assign a unique QR code to each festival installation and programme. |  | Medium | 1 |  |  | FR-QR-01 |  |  |  |  |  |
| 602 | QR Check-in | Load the programme detail page on QR scan including unlocked content visible only to physically scanned-in visitors. |  | Medium | 1 |  |  | FR-QR-02 |  |  |  |  |  |
| 603 | QR Check-in | Trigger a dismissible email registration prompt on the first QR scan by an unauthenticated visitor. |  | Medium | 1 |  |  | FR-QR-03 / FR-PERS-02 |  |  |  |  |  |
| 604 | QR Check-in | Record QR scan events against the registered visitor's profile as confirmed check-ins capturing installation ID and timestamp. |  | Medium | 1 |  |  | FR-QR-04 |  |  |  |  |  |
| 605 | QR Check-in | Author optional unlocked content per installation in AEMaaCS with no empty state when absent. |  | Medium | 1 |  |  | FR-QR-05 / FR-PERS-03 |  |  |  |  |  |
| 700 | Personalisation |  |  |  |  |  |  |  |  |  |  |  |  |
| 701 | Personalisation | Auto-sort programme listing to surface current-night programmes with urgency labels and a post-9pm last-chance section. |  | Medium | 1 |  |  | FR-PERS-01 (A-01); Journey: Plan; Auth: No |  |  |  |  |  |
| 702 | Personalisation | Show a 'Your picks tonight' bookmark-based feed with up to 3 affinity-matched recommendations for registered visitors. |  | Medium | 2 |  |  | FR-PERS-04 (K-01); Journey: Plan → Arrive; Auth: Yes |  |  |  |  |  |
| 703 | Personalisation | Show a 'Trending with your circle' chip using session hash clustering when shared programmes are viewed or bookmarked in the same loop. |  | Medium | 2 |  |  | FR-PERS-05 (K-04); Advocate; Auth: Yes; no cross-visitor PII linkage |  |  |  |  |  |
| 704 | Personalisation | Show returning visitors a contextual banner for unvisited bookmarks or incomplete trail stops linking to remaining itinerary. |  | Medium | 2 |  |  | FR-PERS-06 (K-06); Finale → Plan; Auth: Yes |  |  |  |  |  |
| 705 | Personalisation | Enable native-share itinerary sharing, login-free viewing, one-tap adoption and Community Picks surfacing at ≥10 adoptions. |  | Medium | 2 |  |  | FR-PERS-07 (I-03); Advocate; Auth: Yes |  |  |  |  |  |
| 706 | Personalisation | Track Adobe Target personalisation use cases implemented via Adobe Target, AEP and RT-CDP. |  | Medium | 1 |  |  | 8 selected use cases; defined in 00_personalizations_v1.md |  |  |  |  |  |
| 800 | SEO |  |  |  |  |  |  |  |  |  |  |  |  |
| 801 | SEO | Make all public pages and programme/installation listings indexable with a current sitemap.xml and robots.txt. |  | Medium | 1 |  |  | FR-SEO-01 |  |  |  |  |  |
| 802 | SEO | Implement unique descriptive title and meta description tags, derived dynamically from AEMaaCS for detail pages. |  | Medium | 1 |  |  | FR-SEO-02 |  |  |  |  |  |
| 803 | SEO | Mark up programme and installation listings with Schema.org structured data (Event, Place, ImageObject) using JSON-LD. |  | Medium | 1 |  |  | FR-SEO-03 |  |  |  |  |  |
| 900 | GEO |  |  |  |  |  |  |  |  |  |  |  |  |
| 901 | GEO | Structure the site for visibility in AI-powered and agentic search using semantic HTML, headings and structured data. |  | Medium | 1 |  |  | FR-GEO-01; LLMO is primary optimisation tool |  |  |  |  |  |
| 902 | GEO | Implement an /llms.txt file communicating site structure and permitted content use to AI crawlers and agents. |  | Medium | 1 |  |  | FR-GEO-02 |  |  |  |  |  |
| 1000 | Social Sharing |  |  |  |  |  |  |  |  |  |  |  |  |
| 1001 | Social Sharing | Implement Open Graph meta tags on programme detail and shareable itinerary pages. |  | Medium | 1 |  |  | FR-SOCIAL-01 |  |  |  |  |  |
| 1002 | Social Sharing | Implement Twitter Card meta tags on programme detail and shareable itinerary pages. |  | Medium | 1 |  |  | FR-SOCIAL-02 |  |  |  |  |  |
| 1100 | Content Management |  |  |  |  |  |  |  |  |  |  |  |  |
| 1101 | Content Management | Manage all website content via AEMaaCS delivered using Edge Delivery Services for peak-traffic performance. |  | Medium | 1 |  |  | FR-CM-01 / Scope §6.1 |  |  |  |  |  |
| 1102 | Content Management | Enable Heritage SG authors to update and publish content independently without developer involvement. |  | Medium | 1 |  |  | FR-CM-02 |  |  |  |  |  |
| 1103 | Content Management | Deliver a one-time bulk, high-speed content migration from existing Heritage SG content. |  | Medium | 1 |  |  | FR-CM-03 |  |  |  |  |  |
| 1104 | Content Management | Include optional unlockedContent and firstFestivalYear fields in the AEMaaCS programme/installation content model. |  | Medium | 1 |  |  | FR-CM-04 |  |  |  |  |  |
| 1200 | Reporting |  |  |  |  |  |  |  |  |  |  |  |  |
| 1201 | Reporting | Configure Adobe Analytics workspaces and dashboards covering real-time activity, engagement, QR rates, registration funnel and map interaction. |  | Medium | 1 |  |  | FR-RPT-01; provisioned before go-live |  |  |  |  |  |
| 1202 | Reporting | Provide a real-time operational dashboard throughout the festival window for active sessions, venue engagement and registration activity. |  | Medium | 1 |  |  | FR-RPT-02; 21 Aug – 5 Sep |  |  |  |  |  |
| 1203 | Reporting | Configure Adobe Target activity reporting surfacing lift, confidence and conversion rates per active use case. |  | Medium | 1 |  |  | FR-RPT-03 |  |  |  |  |  |
| 1204 | Reporting | Provide AEP profile and segment reporting on registered visitor counts, consent tier distribution and key RT-CDP segment sizes. |  | Medium | 1 |  |  | FR-RPT-04 |  |  |  |  |  |
| 1205 | Reporting | Report registration and consent funnel performance by registration trigger moment. |  | Medium | 1 |  |  | FR-RPT-05 |  |  |  |  |  |
| 1206 | Reporting | Produce a comprehensive post-festival analytics report against all KPIs, use case outcomes and secondary KPIs. |  | Medium | 1 |  |  | FR-RPT-07; after 5 Sep 2026 |  |  |  |  |  |
| 1207 | Reporting | Enable export of aggregated metrics and raw event data in standard formats such as CSV and Excel. |  | Medium | 1 |  |  | FR-RPT-08 |  |  |  |  |  |
| 1208 | Reporting | Ensure all reporting dashboards and exports comply with PDPA, restricting PII to authorised NHB personnel. |  | Medium | 1 |  |  | FR-RPT-09 |  |  |  |  |  |
| 1300 | LLM Optimizer |  |  |  |  |  |  |  |  |  |  |  |  |
| 1301 | LLM Optimizer | Configure Adobe LLM Optimizer live on the SNF website before the festival opens on 21 Aug 2026. |  | Medium | 1 |  |  | FR-LLMO-01; Delivery: Adobe US |  |  |  |  |  |
| 1302 | LLM Optimizer | Connect LLMO to AEMaaCS content so programme, trail, venue and festival details are optimised for AI-generated results. |  | Medium | 1 |  |  | FR-LLMO-02 |  |  |  |  |  |
| 1303 | LLM Optimizer | Use LLMO as an active optimisation layer complementing the GEO requirements. |  | Medium | 1 |  |  | FR-LLMO-03 |  |  |  |  |  |
| 1304 | LLM Optimizer | Align LLMO configuration with Heritage SG brand guidelines for on-brand, accurate AI representations. |  | Medium | 1 |  |  | FR-LLMO-04 |  |  |  |  |  |
| 1400 | Brand Concierge |  |  |  |  |  |  |  |  |  |  |  |  |
| 1401 | Brand Concierge | Configure Adobe Brand Concierge live on the SNF website by 31 Jul 2026, aligned with the media promotions milestone. |  | Medium | 1 |  |  | FR-BC-01; Delivery: Adobe US |  |  |  |  |  |
| 1402 | Brand Concierge | Ground Brand Concierge in AEMaaCS content including programmes, trails, venues, visiting info and FAQs. |  | Medium | 1 |  |  | FR-BC-02 |  |  |  |  |  |
| 1403 | Brand Concierge | Ensure Brand Concierge responses adhere to Heritage SG brand guidelines and tone, reviewed and approved pre-go-live. |  | Medium | 1 |  |  | FR-BC-03 |  |  |  |  |  |
| 1404 | Brand Concierge | Make Brand Concierge available to all visitors regardless of registration status. |  | Medium | 1 |  |  | FR-BC-04 |  |  |  |  |  |
| 1405 | Brand Concierge | Support Brand Concierge visitor intents including programme discovery, trail recommendations, venue info and general festival information. |  | Medium | 1 |  |  | FR-BC-05 |  |  |  |  |  |
| 1406 | Brand Concierge | Instrument Brand Concierge interactions via Adobe Analytics for engagement rates, query intents and escalation/failure rates. |  | Medium | 1 |  |  | FR-BC-06 |  |  |  |  |  |
| 1500 | Performance |  |  |  |  |  |  |  |  |  |  |  |  |
| 1501 | Performance | Conduct performance testing approximately 2 weeks prior to the website launch date. |  | Medium | 1 |  |  | NFR-PERF-01 |  |  |  |  |  |
| 1502 | Performance | Sustain peak festival traffic loads with specific load targets defined during solution design. |  | Medium | 1 |  |  | NFR-PERF-02; ~1,000,000 visitors, ~100,000 portal sessions |  |  |  |  |  |
| 1503 | Performance | Define and agree target page load times with Heritage SG during solution design. |  | Medium | 1 |  |  | NFR-PERF-03 |  |  |  |  |  |
| 1504 | Performance | Optimise mobile performance so Core Web Vitals (LCP, CLS, INP) meet Google's Good threshold using AEMaaCS EDS. |  | Medium | 1 |  |  | NFR-PERF-04 |  |  |  |  |  |
| 1600 | Security |  |  |  |  |  |  |  |  |  |  |  |  |
| 1601 | Security | Conduct penetration testing approximately 2 weeks prior to the website launch date in parallel with performance testing. |  | Medium | 1 |  |  | NFR-SEC-01 |  |  |  |  |  |
| 1602 | Security | Remediate all critical and high-severity vulnerabilities before go-live. |  | Medium | 1 |  |  | NFR-SEC-02 |  |  |  |  |  |
| 1603 | Security | Use email-only visitor authentication with no SMS of any kind. |  | Medium | 1 |  |  | NFR-SEC-03; SMS OTP requires gov.sg approved sender, out of scope |  |  |  |  |  |
| 1700 | Accessibility |  |  |  |  |  |  |  |  |  |  |  |  |
| 1701 | Accessibility | Conform the website to WCAG 2.1 Level AA. |  | Medium | 1 |  |  | NFR-ACC-01 |  |  |  |  |  |
| 1702 | Accessibility | Validate accessibility compliance as part of QA prior to launch. |  | Medium | 1 |  |  | NFR-ACC-02 |  |  |  |  |  |
| 1800 | PDPA & Privacy |  |  |  |  |  |  |  |  |  |  |  |  |
| 1801 | PDPA & Privacy | Comply with Singapore's PDPA and the Do Not Call (DNC) Registry Act for the website and all data collection. |  | Medium | 1 |  |  | NFR-PDPA-01 |  |  |  |  |  |
| 1802 | PDPA & Privacy | Process geolocation client-side only, passing a derived zone label to Adobe Target and never storing raw GPS server-side. |  | Medium | 1 |  |  | NFR-PDPA-02 |  |  |  |  |  |
| 1803 | PDPA & Privacy | Derive venue check-in data exclusively from QR scan events (installation ID), not GPS. |  | Medium | 1 |  |  | NFR-PDPA-03 |  |  |  |  |  |
| 1804 | PDPA & Privacy | Retain visitor personal data for a maximum of 36 months or until consent withdrawal, whichever is earlier. |  | Medium | 1 |  |  | NFR-PDPA-04 |  |  |  |  |  |
| 1805 | PDPA & Privacy | Provide self-service view, correction and erasure of personal data cascading to visit history and AEP event data. |  | Medium | 1 |  |  | NFR-PDPA-05 |  |  |  |  |  |
| 1806 | PDPA & Privacy | Derive the student cohort flag from geolocation cluster, visit timing and referral source without storing it as permanent PII, refreshed annually. |  | Medium | 1 |  |  | NFR-PDPA-06; studentCohortFlag |  |  |  |  |  |
| 1807 | PDPA & Privacy | Comply with PDPA obligations for Singapore Government websites, PDPC advisory guidelines and statutory board data policies, confirmed with NHB DPO pre-go-live. |  | Medium | 1 |  |  | NFR-PDPA-07 |  |  |  |  |  |
| 1808 | PDPA & Privacy | Implement a PDPA-compliant cookie consent mechanism categorising cookies as Strictly Necessary, Analytics & Performance, and Personalisation & Targeting. |  | Medium | 1 |  |  | NFR-PDPA-08 |  |  |  |  |  |
| 1809 | PDPA & Privacy | Display a cookie consent banner on first visit and suppress non-essential cookies until explicit consent, with no pre-ticked acceptance. |  | Medium | 1 |  |  | NFR-PDPA-09 |  |  |  |  |  |
| 1810 | PDPA & Privacy | Provide an accessible cookie settings control to manage preferences at any time, with withdrawal effective immediately. |  | Medium | 1 |  |  | NFR-PDPA-10 |  |  |  |  |  |
| 1811 | PDPA & Privacy | Record cookie consent choices per visitor and respect them across sessions without relying on a non-essential cookie. |  | Medium | 1 |  |  | NFR-PDPA-11 |  |  |  |  |  |
| 1812 | PDPA & Privacy | Provide an accessible Cookie Policy page documenting all cookies, purpose, category and retention period. |  | Medium | 1 |  |  | NFR-PDPA-12 |  |  |  |  |  |
