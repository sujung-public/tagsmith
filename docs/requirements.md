# Singapore Night Festival 2026 — Requirements Document

**Document:** 01-requirements-v1.md
**Project:** Adobe × Heritage SG — Singapore Night Festival 2026
**Client:** National Heritage Board (NHB) / Heritage SG
**Author:** Enterprise Architecture
**Status:** Draft for Review
**Date:** 2026-06-10
**Version:** 1.0

---

## Table of Contents

1. [Overview](#1-overview)
2. [Project Context](#2-project-context)
3. [Stakeholders](#3-stakeholders)
4. [Objectives](#4-objectives)
5. [Key Performance Indicators](#5-key-performance-indicators)
6. [Scope](#6-scope)
7. [Functional Requirements](#7-functional-requirements)
8. [Non-Functional Requirements](#8-non-functional-requirements)
9. [Key Dates & Timeline](#9-key-dates--timeline)
10. [Delivery Team](#10-delivery-team)
11. [Open Items & Decisions](#11-open-items--decisions)
12. [References](#12-references)
13. [Changelog](#13-changelog)

---

## 1. Overview

This document defines the requirements for the Singapore Night Festival 2026 (SNF 2026) digital experience — a public-facing website delivering festival information, programme discovery, personalised visitor navigation, and in-venue engagement.

The project is an Adobe × Heritage SG collaboration, showcasing how Adobe's technology stack can deliver personalised, data-driven visitor experiences at scale. Accenture is the delivery partner responsible for the user experience design, MapBox license procurement, and MapBox style system. Adobe is responsible for the map implementation.

---

## 2. Project Context

### 2.1 Event Details

| Attribute | Detail |
|-----------|--------|
| Event | Singapore Night Festival 2026 (SNF 2026) |
| Organiser | Heritage SG, a division of the National Heritage Board (NHB) |
| Location | Bras Basah–Bugis (BBB) precinct, Singapore |
| Festival Dates | 21 August – 5 September 2026 (15 nights) |
| Expected Footfall | ~1,000,000 visitors over the festival window |
| Daily Average | ~66,000 visitors/night |

### 2.2 Visitor Profile

| Segment | Description |
|---------|-------------|
| Primary audience | Singapore locals |
| Repeat visitors | A significant and strategically important proportion, particularly university students from BBB precinct institutions (LASALLE, NAFA, SMU, SIM) who form an annual SNF attendance habit and continue attending post-graduation |
| Strategic value | The student and repeat visitor cohort represents NHB's highest long-term cultural engagement audience, becoming long-term NHB cultural participants after graduation |

### 2.3 Problem Statement

Visitor navigation has been a recurring challenge at previous SNF editions. Key pain points identified by Heritage SG stakeholders:

- Visitor unfamiliarity with the Bras Basah–Bugis precinct layout
- Poor wayfinding signage in nighttime conditions
- Difficulty using physical maps while moving through crowds
- Visitors frequently missing exhibits as a result

The digital solution is intended to directly address this navigation challenge while simultaneously enabling personalised discovery and engagement.

### 2.4 Adobe's Role

Adobe has been engaged by NHB / Heritage SG to showcase how Adobe tools can deliver personalised visitor experiences at the Night Festival. Adobe's primary objective is demonstrative — to illustrate the capabilities of Adobe's technology stack in a live, high-profile cultural event context. Adobe will work closely with Accenture, who will deliver the user experience and map components.

---

## 3. Stakeholders

| Stakeholder | Organisation | Role |
|-------------|--------------|------|
| Heritage SG / NHB | Client | Project owner; content authors; event organiser |
| Adobe | Technology Partner | Overall Adobe product ownership; showcase sponsor |
| Adobe Professional Services (Adobe ProServ) | Adobe Delivery | Implementation and customisation of AEMaaCS, AEP, RT-CDP, Adobe Target, and Adobe Analytics |
| Adobe Ultimate Success (Adobe US) | Adobe Delivery | Delivery of Adobe LLM Optimizer and Adobe Brand Concierge |
| Accenture | Delivery Partner | User experience design; MapBox license procurement; MapBox style system |

---

## 4. Objectives

### 4.1 Primary Objective
Drive increased visitor attendance at the Singapore Night Festival 2026.

### 4.2 Secondary Objective
Drive year-round traffic to NHB museums and galleries, converting SNF festival engagement into sustained long-term cultural participation.

### 4.3 Adobe Showcase Objective
Demonstrate how Adobe tools — AEMaaCS, AEP, RT-CDP, Adobe Target, and Adobe Analytics — can deliver a personalised, data-driven visitor experience in a live cultural event context.

### 4.4 Navigation Objective
Address the recurring visitor navigation pain point by providing digital wayfinding that works effectively in a nighttime, crowded-precinct environment, ensuring visitors can discover and reach festival installations with minimal friction.

---

## 5. Key Performance Indicators

> **Status:** Proposed — to be formally confirmed with Heritage SG / NHB. Specific measurable targets are to be aligned as a separate exercise following completion of this requirements document. See Open Item OD-01.

### 5.1 Primary KPI — Festival Attendance

| KPI | Measurement Method |
|-----|--------------------|
| Total festival footfall | NHB on-ground attendance data |
| Klook ticketing page click-throughs from the SNF website | Adobe Analytics |
| Unique website sessions during the festival window (21 Aug – 5 Sep) | Adobe Analytics |

### 5.2 Digital Engagement — Portal Adoption

| KPI | Measurement Method |
|-----|--------------------|
| Email registration rate — % of portal sessions that complete registration | Adobe Analytics + AEP |
| QR scan rate — % of registered users who scan ≥1 installation | AEP event data |
| Trail adoption rate — % of registered users who save or follow a trail | AEP event data |
| Trail completion rate — % of trail followers who complete all stops | AEP event data |
| Average installations visited per registered user | AEP event data |

### 5.3 Personalisation Effectiveness

| KPI | Measurement Method |
|-----|--------------------|
| Adobe Target activity CTR vs. control (personalised vs. default experience) | Adobe Target reporting |
| Bookmark rate — % of sessions with ≥1 bookmark | Adobe Analytics |
| Return visit rate — % of registered users who visit on 2+ festival nights | AEP profile data |

### 5.4 Navigation

| KPI | Measurement Method |
|-----|--------------------|
| Map page engagement rate — % of sessions that interact with the map | Adobe Analytics |
| Trail completion rate — proxy for successful navigation through the precinct | AEP event data |

### 5.5 Secondary KPI — Year-Round NHB Engagement

| KPI | Measurement Method |
|-----|--------------------|
| NHB museum/gallery page click-throughs from the SNF website | Adobe Analytics |
| Year-round opt-in rate — % of registered users with Tier 2 consent | AEP profile data |

---

## 6. Scope

### 6.1 In Scope

- Public-facing SNF 2026 website — desktop and mobile, English only
- Five website pages: Home, Programme Details, About, Visit, Map
- Content management via Adobe Experience Manager as a Cloud Service (AEMaaCS), delivered using Edge Delivery Services (EDS) for high performance and scalability
- One-time content migration from existing Heritage SG content (Adobe-assisted)
- Interactive precinct map implemented by Adobe using MapBox (MapBox license and style system delivered by Accenture)
- Privacy Policy page and Terms of Use page (mandatory for Singapore Government websites)
- Government disclaimer on all pages (clarification from Heritage SG)
- Visitor registration via OTP (mobile number; email as fallback)
- QR code check-in at festival installations
- Self-guided trail discovery, selection, and progress tracking
- Custom itinerary creation, sharing, and community adoption
- Eight selected personalisation use cases via Adobe Target (see Section 7.5)
- Visitor profile management via Adobe Experience Platform (AEP) and Real-Time CDP (RT-CDP)
- Adobe Analytics instrumentation across all pages and key interactions
- Adobe LLM Optimizer (LLMO) — AI search and generative engine content optimisation, live before festival opens
- Adobe Brand Concierge — AI-powered conversational assistant, live by 31 Jul 2026
- SEO with structured metadata and Schema.org markup for programme listings
- GEO (Generative Engine Optimisation) — visibility to agentic and AI-powered search traffic
- Social sharing meta tags (Open Graph and Twitter Card) for programmes and itineraries
- Performance testing and penetration testing prior to website launch
- PDPA-compliant three-tier consent model
- WCAG 2.1 Level AA accessibility compliance

### 6.2 Out of Scope

| Item | Notes |
|------|-------|
| Ticketing purchase and related flows | Handled entirely by Klook (third-party platform); the SNF website will link to Klook only |
| Adobe Journey Optimizer (AJO) | Not in scope; no email or messaging communication journeys will be delivered in this project |
| Post-festival email communication journeys | Dependent on AJO; excluded from this project scope |
| Multilingual support | English only; no additional languages |
| Native mobile application | Web experience only; no iOS or Android app |
| SMS (all channels) | No SMS of any kind — visitor registration is via email only; SMS OTP is excluded as sending requires a gov.sg approved sender, which is not in scope for this project |

---

## 7. Functional Requirements

### 7.1 Public Website Pages

The website shall comprise the following five pages, designed and delivered per the approved wireframes in `assets/pweb-wireframes/`:

| Page | Desktop | Mobile |
|------|---------|--------|
| Home Page | ✓ | ✓ |
| Programme Details | ✓ | ✓ |
| About | ✓ | ✓ |
| Visit | ✓ | ✓ |
| Map | ✓ | ✓ |
| Privacy Policy | ✓ | ✓ |
| Terms of Use | ✓ | ✓ |

**FR-PW-01:** All pages shall be responsive and designed with a mobile-first approach, given that the majority of festival traffic is expected from mobile devices. Desktop viewports shall also be fully supported, as per the approved wireframes.

**FR-PW-02:** The website shall include a clearly visible call-to-action directing visitors to the Klook ticketing platform. No ticketing functionality shall be built within the SNF website.

**FR-PW-03:** The website shall display festival programme and installation listings, including title, description, venue, dates, and times.

**FR-PW-04:** The website shall comply with Heritage SG brand guidelines as documented in `00_brand_guidelines_v1.md`.

**FR-PW-05:** The website shall include a Privacy Policy page documenting all personal data collected, the purpose of collection, retention periods, and visitor rights under PDPA. This page is distinct from the Cookie Policy (NFR-PDPA-12) and is mandatory for Singapore Government websites.

**FR-PW-06:** The website shall include a Terms of Use page setting out the conditions governing use of the SNF website. This is mandatory for Singapore Government-affiliated websites. Content for both the Privacy Policy and Terms of Use pages shall be provided and approved by NHB / Heritage SG.

**FR-PW-07:** A standard government disclaimer shall appear on all pages of the website, as required by Heritage SG. The exact disclaimer text shall be provided by NHB / Heritage SG.

### 7.2 User Registration & Consent

**FR-REG-01:** Visitors shall be able to register using an email address, verified via a one-time code or link sent to their email. Mobile number registration is not in scope; SMS OTP requires a gov.sg approved sender, which is outside the scope of this project.

**FR-REG-02:** The email registration flow shall be optimised for mobile, given the expected majority of mobile traffic during the festival.

**FR-REG-03:** Registration shall be optional. Unregistered visitors shall have full, unrestricted access to all website content. Registration unlocks personalisation features only and shall never be presented as a gate to content.

**FR-REG-04:** The following three-tier consent model shall be implemented at registration:

| Tier | Purpose | Required For |
|------|---------|--------------|
| Tier 0 — Functional | Email registration; visitor profile storage; in-app features (itinerary, QR scanning, trail progress) | All in-app personalisation use cases |
| Tier 1 — Festival Marketing | Consent for festival-period communications | Collected for future use; no communication journeys are in scope for this project |
| Tier 2 — Year-Round NHB | Consent for post-festival NHB museum/gallery communications | Collected for future use; no communication journeys are in scope for this project |

**FR-REG-05:** All consent checkboxes shall render unchecked by default. Positive user action is required for each consent tier. Tier 1 and Tier 2 shall be separate checkboxes with distinct, plain-language purpose statements. Tier 1 and Tier 2 consent shall not be bundled into a single checkbox.

**FR-REG-06:** Visitors shall be able to withdraw consent at any time via self-service profile settings. Withdrawal shall take effect immediately.

**FR-REG-07:** A consent log shall be maintained recording each consent grant and withdrawal, capturing: visitor ID, consent type (Tier 1 / Tier 2), action (grant / withdraw), timestamp, and hashed IP address. This log is required as audit evidence for PDPA compliance.

### 7.3 Navigation & Map

**FR-MAP-01:** The website shall include an interactive map of the Bras Basah–Bugis precinct, displaying all festival programme and installation locations.

**FR-MAP-02:** The map shall be implemented by Adobe using MapBox. Accenture is responsible for procuring the MapBox license and delivering the MapBox style system.

**FR-MAP-03:** When location permission is granted by the visitor, the map and programme listing shall support proximity-based sorting, ranking nearby installations by walking distance from the visitor's current location.

**FR-MAP-04:** Visitors who deny location permission shall see the default listing without any degradation of experience.

**FR-MAP-05 (Phase C):** The map shall display live crowd density indicators (🟢 Quiet / 🟡 Busy / 🔴 Packed) per venue, derived from Adobe Analytics real-time session data. Raw GPS coordinates shall not be stored server-side.

### 7.4 Programme Discovery, Trails & Itinerary

**FR-TRAIL-01:** The website shall present curated self-guided trails for visitor selection and navigation.

**FR-TRAIL-02:** Registered visitors shall be able to save and follow a trail. Trail progress shall be tracked via QR scan check-ins at each stop.

**FR-TRAIL-03:** Registered visitors shall be able to create custom itineraries by adding programmes and installations of their choice.

**FR-TRAIL-04:** The system shall detect conflicts and inefficiencies in custom itineraries (e.g., time overlaps, suboptimal walking routes, gaps) and surface inline optimisation suggestions. Suggestions shall be dismissible and non-blocking.

**FR-TRAIL-05:** Custom itineraries shall be shareable via native device share. No OAuth to any social platform is required.

**FR-TRAIL-06:** Shared itineraries shall be publicly viewable without authentication. Recipients shall be able to adopt an itinerary in one tap, which triggers a light registration prompt.

**FR-TRAIL-07:** Itineraries that achieve 10 or more unique adoptions within the festival window shall be surfaced as "Community Picks" on the Trails page, alongside the curated trails.

### 7.5 QR Scanning & Check-in

**FR-QR-01:** Each festival installation and programme shall have a unique QR code.

**FR-QR-02:** Scanning a QR code shall load the programme detail page, which shall include unlocked content visible only to visitors who have physically scanned in (e.g., artist notes, best viewing spot tips, performance countdowns).

**FR-QR-03:** The first QR scan by an unauthenticated visitor shall trigger a dismissible email registration prompt. Declining the prompt shall have no impact on the visitor's experience.

**FR-QR-04:** QR scan events shall be recorded against the registered visitor's profile as confirmed check-ins, capturing the installation ID and timestamp.

**FR-QR-05:** Unlocked content per installation shall be an optional field authored by Heritage SG in AEMaaCS. Installations without authored unlocked content shall not display an empty state to the visitor.

### 7.6 Personalisation

The following 8 use cases shall be implemented using Adobe Target, AEP, and RT-CDP. Full use case definitions are in `00_personalizations_v1.md`; the journey map is in `assets/snf-journey-personalization-map.html`.

| ID | Name | Journey Step | Phase | Auth Required |
|----|------|--------------|-------|---------------|
| A-01 | Temporal Programme Feed | Plan | 1 | No |
| Q-01 | Physical Attendance → Registration | Arrive | 1 | No |
| Q-02 | In-Venue Unlocked Content | Engage | 1 | No |
| K-01 | Bookmark-Based Personalised Feed | Plan → Arrive | 2 | Yes |
| K-04 | Social Amplification Loop | Advocate | 2 | Yes |
| K-06 | Post-Visit Re-engagement (Night 2+) | Finale → Plan | 2 | Yes |
| I-03 | Social Itinerary Sharing & Community Picks | Advocate | 2 | Yes |
| FR-P2-17 | Live Crowd Density Indicators | Engage | Phase C | No |

**FR-PERS-01 (A-01):** The programme listing and landing page shall auto-sort to surface programmes running on the current festival night. Urgency labels ("On now", "Ending in X hrs") shall appear for programmes nearing their close. After 9pm, a "Tonight's last chance" section shall surface programmes ending before 11pm.

**FR-PERS-02 (Q-01):** The first QR scan by an unauthenticated visitor shall trigger a dismissible email registration prompt. This is the highest-converting registration moment in the visitor journey.

**FR-PERS-03 (Q-02):** Each QR scan shall unlock installation-specific content not visible to non-attendees. Unlocked content is authored per installation in AEMaaCS and is optional.

**FR-PERS-04 (K-01):** Registered visitors with saved bookmarks shall see a "Your picks tonight" section above the general programme feed, populated with their bookmarks and up to 3 affinity-matched recommendations.

**FR-PERS-05 (K-04):** When a shared programme is subsequently viewed or bookmarked by another visitor in the same share loop, a "Trending with your circle" chip shall appear on the programme card for the original sharer. Cross-visitor PII linkage is not permitted; session hash clustering shall be used.

**FR-PERS-06 (K-06):** Registered visitors returning on a subsequent festival night with unvisited bookmarks or incomplete trail stops shall see a contextual banner ("You've got X unvisited stops from last night — they're on again tonight") linking directly to their remaining itinerary.

**FR-PERS-07 (I-03):** Visitors shall be able to share custom itineraries via native share. Shared itineraries shall be viewable without login and adoptable in one tap. Itineraries with ≥10 unique adoptions shall surface as Community Picks on the Trails page.

**FR-PERS-08 (FR-P2-17 — Phase C):** The map shall display live crowd density indicators per venue (🟢/🟡/🔴) derived from Adobe Analytics real-time session data. No raw GPS coordinates shall be stored server-side.

### 7.7 SEO, GEO & Social Sharing

**FR-SEO-01:** All public pages and programme/installation listings shall be indexable by search engines. A `sitemap.xml` and a `robots.txt` shall be implemented and kept current.

**FR-SEO-02:** Each page shall implement unique, descriptive `<title>` and `<meta description>` tags. Programme and installation detail pages shall derive these dynamically from AEMaaCS content.

**FR-SEO-03:** Programme and installation listings shall be marked up with Schema.org structured data (`Event`, `Place`, `ImageObject` as applicable) using JSON-LD, enabling rich results in search engines and improving discoverability for a high-profile cultural event.

**FR-GEO-01:** The website shall be structured to support visibility in AI-powered and agentic search traffic (Generative Engine Optimisation). This includes semantic HTML, descriptive headings, structured data markup (FR-SEO-03), and clear, machine-readable programme and event content to enable accurate extraction and representation by large language models and AI search engines (e.g., Google AI Overviews, ChatGPT, Perplexity). Adobe LLM Optimizer (Section 7.11) shall be the primary tool for managing and optimising this visibility.

**FR-GEO-02:** A `/llms.txt` file shall be implemented to communicate to AI crawlers and agents the site structure, key content locations, and permitted use of content for indexing and summarisation.

**FR-SOCIAL-01:** All programme detail pages and shareable itinerary pages shall implement Open Graph meta tags (`og:title`, `og:description`, `og:image`, `og:url`) to control how content renders when shared on social platforms.

**FR-SOCIAL-02:** All programme detail pages and shareable itinerary pages shall implement Twitter Card meta tags to ensure rich previews when shared on X (Twitter).

### 7.8 Content Management

**FR-CM-01:** All website content shall be managed via Adobe Experience Manager as a Cloud Service (AEMaaCS), delivered using Edge Delivery Services (EDS) to ensure high performance and scalability under peak festival traffic loads.

**FR-CM-02:** Heritage SG content authors shall be able to update and publish content independently, without requiring developer involvement. Rapid content publishing is a key requirement, particularly during the festival period.

**FR-CM-03:** Adobe shall deliver a one-time content migration from the existing Heritage SG content. The migration approach shall be designed to support bulk, high-speed migration to minimise time and manual effort.

**FR-CM-04:** The AEMaaCS content model for festival programmes and installations shall include:
- An optional `unlockedContent` field to support QR scan unlocked content (FR-QR-05)
- A `firstFestivalYear` field to support new vs. returning programme differentiation for repeat visitors

### 7.9 Analytics

**FR-AN-01:** Adobe Analytics shall be instrumented across all pages and key user interactions.

**FR-AN-02:** Analytics instrumentation shall capture all events required to measure the KPIs defined in Section 5.

**FR-AN-04:** Real-time Adobe Analytics session data shall be used to derive per-venue crowd density signals for the live crowd density indicators on the map (FR-PERS-08 / Phase C).

### 7.10 Reporting

**FR-RPT-01:** Adobe Analytics workspaces and dashboards shall be configured for Heritage SG stakeholders, covering at minimum: real-time visitor activity, programme and trail engagement, QR scan rates, registration funnel performance, and map interaction. Dashboard access shall be provisioned for the appropriate Heritage SG team members prior to go-live.

**FR-RPT-02:** A real-time operational dashboard shall be available to the Heritage SG operations team throughout the festival window (21 Aug – 5 Sep), providing visibility into active sessions, venue-level engagement, and registration activity during each festival night.

**FR-RPT-03:** Adobe Target activity reporting shall be configured to surface personalisation effectiveness metrics — including lift, confidence, and conversion rates — for each active use case, enabling iterative optimisation during the festival period.

**FR-RPT-04:** AEP profile and segment reporting shall provide Heritage SG with visibility into registered visitor counts, consent tier distribution, and key RT-CDP segment sizes (e.g., returning visitors, trail completers, year-round opt-ins) throughout and after the festival.

**FR-RPT-05:** Registration and consent funnel performance shall be reportable by registration trigger moment (e.g., QR scan, trail save, itinerary adoption), enabling Heritage SG to understand which prompts drive the highest registration conversion.

**FR-RPT-07:** A comprehensive post-festival analytics report shall be produced following the close of SNF 2026 (5 Sep 2026), covering performance against all KPIs defined in Section 5, personalisation use case outcomes, and secondary KPI metrics for year-round NHB engagement.

**FR-RPT-08:** Aggregated metrics and raw event data shall be exportable in standard formats (e.g., CSV, Excel) to support NHB's internal planning and reporting processes.

**FR-RPT-09:** All reporting dashboards and data exports shall comply with PDPA. Personally identifiable information shall not be exposed in aggregate reporting views unless access is restricted to authorised NHB personnel.

### 7.11 Adobe LLM Optimizer

Adobe LLM Optimizer (LLMO) ensures that SNF 2026 content is accurately and prominently represented when visitors discover the festival through AI-powered search engines and agentic interfaces. **Delivery: Adobe Ultimate Success (Adobe US).**

**FR-LLMO-01:** Adobe LLM Optimizer shall be configured and live on the SNF website before the festival opens on 21 Aug 2026.

**FR-LLMO-02:** LLMO shall be connected to SNF 2026 content managed in AEMaaCS, ensuring that programme listings, trail descriptions, venue information, and festival details are optimised for accurate representation in AI-generated search results and summaries.

**FR-LLMO-03:** LLMO shall complement the GEO requirements defined in FR-GEO-01 and FR-GEO-02, providing an active optimisation layer on top of the structural and markup-based foundations.

**FR-LLMO-04:** LLMO configuration shall be aligned with Heritage SG brand guidelines to ensure that AI-generated representations of SNF content are on-brand and accurate.

### 7.12 Adobe Brand Concierge

Adobe Brand Concierge provides visitors with an AI-powered conversational assistant embedded on the SNF website, enabling natural language discovery of festival programmes, trails, venues, and visitor information. **Delivery: Adobe Ultimate Success (Adobe US).**

**FR-BC-01:** Adobe Brand Concierge shall be configured and live on the SNF website by 31 Jul 2026, aligned with the media promotions and press conference milestone.

**FR-BC-02:** Brand Concierge shall be grounded in SNF 2026 content managed in AEMaaCS — including programme listings, trail information, venue details, visiting information, and festival FAQs — ensuring responses are accurate and current.

**FR-BC-03:** Brand Concierge responses shall adhere to Heritage SG brand guidelines and tone of voice. Response behaviour and guardrails shall be reviewed and approved by Heritage SG prior to go-live.

**FR-BC-04:** Brand Concierge shall be available to all visitors regardless of registration status, functioning as a discovery and wayfinding tool for both anonymous and known users.

**FR-BC-05:** Brand Concierge shall handle at minimum the following visitor intents: programme and installation discovery, trail recommendations, venue location and visiting hours, and general festival information. The specific scope of supported intents shall be confirmed with Heritage SG during configuration.

**FR-BC-06:** Brand Concierge interactions shall be instrumented via Adobe Analytics to capture engagement rates, common query intents, and escalation or failure rates, enabling ongoing optimisation.

---

## 8. Non-Functional Requirements

### 8.1 Performance & Scalability

**NFR-PERF-01:** Performance testing shall be conducted approximately 2 weeks prior to the website launch date (see Section 9).

**NFR-PERF-02:** The website shall sustain peak festival traffic loads. Specific load targets (concurrent sessions, response times, throughput) shall be defined during solution design, informed by the expected ~1,000,000 festival visitors and estimated ~100,000 portal sessions across the festival window.

**NFR-PERF-03:** Target page load times shall be defined and agreed with Heritage SG during solution design.

**NFR-PERF-04:** The website shall be optimised for mobile performance as the primary target device. Mobile Core Web Vitals (LCP, CLS, INP) shall meet Google's "Good" threshold. AEMaaCS Edge Delivery Services shall be leveraged to achieve this.

### 8.2 Security

**NFR-SEC-01:** Penetration testing shall be conducted approximately 2 weeks prior to the website launch date, to be coordinated in parallel with performance testing.

**NFR-SEC-02:** All critical and high-severity security vulnerabilities identified during penetration testing must be fully remediated before the website goes live.

**NFR-SEC-03:** Visitor authentication shall be via email only. No SMS of any kind shall be sent — visitor registration is email-based, as SMS OTP requires a gov.sg approved sender which is outside the scope of this project.

### 8.3 Accessibility

**NFR-ACC-01:** The website shall conform to WCAG 2.1 Level AA.

**NFR-ACC-02:** Accessibility compliance shall be validated as part of the QA process prior to launch.

### 8.4 Privacy & Data Compliance

**NFR-PDPA-01:** The website and all associated data collection shall comply with Singapore's Personal Data Protection Act (PDPA) and the Do Not Call (DNC) Registry Act.

**NFR-PDPA-02:** Raw GPS coordinates shall not be stored server-side. Geolocation shall be processed client-side only for proximity calculations, with only the derived zone label (e.g., zone identifier) passed to Adobe Target.

**NFR-PDPA-03:** Venue check-in data shall be derived exclusively from QR scan events (installation ID) and not from GPS data.

**NFR-PDPA-04:** Visitor personal data shall be retained for a maximum of 36 months, or until consent is withdrawn, whichever is earlier.

**NFR-PDPA-05:** Visitors shall have self-service access to view, correct, and request erasure of their personal data. Erasure shall cascade to visit history and all AEP event data.

**NFR-PDPA-06:** The student cohort inference signal (`studentCohortFlag`) shall be derived from a combination of geolocation cluster, visit timing, and referral source. It shall not be stored as a permanent PII attribute and shall be refreshed annually.

**NFR-PDPA-07:** As a digital service operated by NHB / Heritage SG, a Singapore government statutory board, the website shall comply with the PDPA requirements applicable to Singapore Government websites. This includes adherence to the Personal Data Protection Commission (PDPC) Advisory Guidelines, the Government's data protection and data governance policies, and any specific data handling obligations applicable to statutory boards under Singapore law. Specific compliance requirements shall be confirmed with NHB's Data Protection Officer (DPO) prior to go-live.

**NFR-PDPA-08:** The website shall implement a PDPA-compliant cookie consent mechanism. Cookies shall be categorised as follows:

| Category | Examples | Consent Required |
|----------|----------|-----------------|
| Strictly Necessary | Session management, OTP authentication | No |
| Analytics & Performance | Adobe Analytics | Yes |
| Personalisation & Targeting | Adobe Target | Yes |

**NFR-PDPA-09:** A cookie consent banner shall be displayed to all visitors on first visit. Non-essential cookies (analytics and targeting) shall not be set or fired until the visitor has explicitly consented. Pre-ticked acceptance is not permitted.

**NFR-PDPA-10:** Visitors shall be able to manage their cookie preferences at any time via an accessible cookie settings control on the website. Withdrawal of cookie consent shall take effect immediately and suppress all non-essential cookie activity for that visitor.

**NFR-PDPA-11:** Cookie consent choices shall be recorded per visitor and respected across sessions for the duration of the consent period. The consent record shall be stored in a manner that does not itself rely on a non-essential cookie.

**NFR-PDPA-12:** The website shall include an accessible Cookie Policy page documenting all cookies in use, their purpose, category, and retention period.

---

## 9. Key Dates & Timeline

| Date | Milestone |
|------|-----------|
| ~1 Jul 2026 | Performance and penetration testing begins (~2 weeks before public website launch) |
| **15 Jul 2026** | **Public website go-live — aligned with ticketing launch on Klook** |
| **31 Jul 2026** | **Adobe Brand Concierge go-live; media promotions and press conference** |
| 19 Aug 2026 | Media preview |
| **21 Aug 2026** | **Festival opens — full interactive experience and Adobe LLM Optimizer live** |
| **5 Sep 2026** | **Festival closes** |

> **Note:** The ~1 Jul testing start date is derived from the 15 Jul public website launch and the 2-week testing requirement. The exact testing start date shall be confirmed during project planning.

---

## 10. Delivery Team

### Adobe Professional Services (Adobe ProServ)
Responsible for implementation and customisation of AEMaaCS, AEP, RT-CDP, Adobe Target, and Adobe Analytics.

| Role | Responsibility |
|------|----------------|
| Project Manager | Project planning, scheduling, and delivery coordination; stakeholder communication; risk and issue management |
| Enterprise Architect | Overall architecture governance; solution design oversight |
| Technical Architect | Technical design; integration architecture; developer guidance |
| Front-end Developer | Website implementation; AEMaaCS component development |
| Back-end Developer | Services integration; AEP, RT-CDP, and Adobe Target implementation |
| QA | Testing strategy; functional, performance, accessibility, and security test coordination |

### Adobe Ultimate Success (Adobe US)
Responsible for delivery of Adobe LLM Optimizer and Adobe Brand Concierge.

| Role | Responsibility |
|------|----------------|
| Adobe US Team | Configuration, onboarding, and go-live of Adobe LLM Optimizer and Adobe Brand Concierge; coordination with Adobe ProServ for content and analytics integration |

---

## 11. Open Items & Decisions

| # | Item | Owner | Status |
|---|------|-------|--------|
| OD-01 | KPI targets — specific measurable targets to be confirmed with Heritage SG / NHB | Enterprise Architect / NHB | Open |
| OD-02 | Single website vs. separate public site and festival portal — preference is single website, pending solution design validation on seamlessness and technical feasibility | Technical Architect | Open |
| OD-03 | Peak load targets and page performance benchmarks — to be defined during solution design | Technical Architect | Open |
| OD-04 | Rapid content publishing SLA — specific time-to-publish target to be agreed with Heritage SG | Heritage SG | Open |
| OD-05 | Exact performance and penetration testing start date — to be confirmed during project planning | QA | Open |

---

## 12. References

| Document | Description |
|----------|-------------|
| `references/00_brand_guidelines_v1.md` | Heritage SG brand guidelines |
| `references/00_mapbox_implementation.md` | MapBox implementation reference |
| `references/00_personalizations_v1.md` | Full personalisation use case library (32 use cases) |
| `references/00_user_personas_v1.md` | Visitor personas |
| `assets/pweb-wireframes/` | Public website wireframes (desktop and mobile) |
| `assets/snf-journey-personalization-map.html` | Selected personalisation use cases (8) mapped to visitor journey |
| `assets/SNF2025 Content_for_Marketing_For Reference.xlsx` | Festival content and self-guided trail reference |

---

## 13. Changelog

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2026-06-10 | Enterprise Architecture | Initial draft |
| 1.0 | 2026-06-10 | Enterprise Architecture | Added NFR-PDPA-07: PDPA compliance for Singapore Government websites (statutory board obligations, PDPC guidelines, DPO confirmation required pre-go-live) |
| 1.0 | 2026-06-10 | Enterprise Architecture | Added NFR-PDPA-08 to NFR-PDPA-12: Cookie consent requirements covering cookie categories, consent banner, preference management, consent persistence, and Cookie Policy page |
| 1.0 | 2026-06-10 | Enterprise Architecture | Updated AEMaaCS delivery to use Edge Delivery Services (EDS); changed visitor registration to email-only (mobile/SMS OTP excluded — gov.sg approved sender required); updated map delivery to Adobe with Accenture scoped to MapBox license and style system; added mobile-first requirement (FR-PW-01, FR-REG-02, NFR-PERF-04); updated all OTP references to email |
| 1.0 | 2026-06-10 | Enterprise Architecture | Added Privacy Policy page (FR-PW-05), Terms of Use page (FR-PW-06), and Government disclaimer (FR-PW-07) as mandatory Singapore Government website requirements; added new Section 7.7 covering SEO (FR-SEO-01–03), GEO / agentic visibility (FR-GEO-01–02), and social sharing meta tags (FR-SOCIAL-01–02) |
| 1.0 | 2026-06-10 | Enterprise Architecture | Added new Section 7.10 Reporting covering stakeholder dashboards (FR-RPT-01), real-time festival operations dashboard (FR-RPT-02), Adobe Target personalisation reporting (FR-RPT-03), AEP segment reporting (FR-RPT-04), registration funnel reporting (FR-RPT-05), post-festival KPI report (FR-RPT-07), data export (FR-RPT-08), and PDPA-compliant reporting (FR-RPT-09) |
| 1.0 | 2026-06-23 | mathai | Removed WOGAA references confirmed not required by HSG (22 Jun 2026): removed FR-AN-03, FR-RPT-06, NFR-GOV-01, Section 8.5 Government Standards, and "WOGAA standards compliance" from Section 6.1 scope |
| 1.0 | 2026-06-10 | Enterprise Architecture | Added Adobe LLM Optimizer (Section 7.11, FR-LLMO-01–04, live before 22 Aug) and Adobe Brand Concierge (Section 7.12, FR-BC-01–06, live by 31 Jul) as additional Adobe products; updated Section 6.1, FR-GEO-01, and Key Dates accordingly |
| 1.0 | 2026-06-10 | Enterprise Architecture | Clarified delivery responsibilities: Adobe ProServ delivers AEMaaCS, AEP, RT-CDP, Adobe Target, and Adobe Analytics; Adobe Ultimate Success (Adobe US) delivers Adobe LLM Optimizer and Adobe Brand Concierge; updated Sections 3, 7.11, 7.12, and 10 accordingly |
| 1.0 | 2026-06-10 | Enterprise Architecture | Added Project Manager to Adobe ProServ delivery team (Section 10) |
| 1.0 | 2026-07-03 | mathai | Festival start date corrected from 22 Aug to 21 Aug 2026 (confirmed) across the document; end date (5 Sep) unchanged |
