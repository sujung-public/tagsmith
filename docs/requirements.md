# Northwind Outfitters — Web Analytics Requirements

**Site:** www.northwind-outfitters.example (outdoor apparel & gear e-commerce)
**Markets:** US, UK, KR · **Platforms:** desktop web, mobile web
**Analytics:** Adobe Analytics via Adobe Experience Platform Tags (Web SDK)
**Owner:** Digital Marketing · **Version:** 1.0 (2026-11-02)

## 1. Business goals

1. Grow online revenue 15% YoY by improving product discovery and checkout conversion.
2. Understand which marketing channels and campaigns drive first purchases vs. repeat purchases.
3. Reduce checkout abandonment, especially on mobile.
4. Measure how content (buying guides, videos) influences purchases.

## 2. Key questions the data must answer

- Which pages, sections and site areas get the most traffic, per market and device?
- Which marketing channels / campaigns (incl. internal banners) lead to orders and revenue?
- How do visitors find products: navigation, internal search, recommendations or campaigns?
- Where do visitors drop off between product view → cart → checkout → order?
- Which products and categories are viewed, added to cart and purchased?
- Do logged-in members convert better than guests?

## 3. Requirements

### 3.1 Page & site context
- Track the page name, site section and page type (home, category, product, cart, checkout, content, account) on every page.
- Track the site market / language (e.g. `us-en`, `kr-ko`) and the device platform.
- Track error pages (404 / 500) with the requested URL.

### 3.2 Visitor & login
- Track login status (logged-in / guest) on every page and the hashed member ID when logged in.
- Track successful logins and new account registrations as events.
- Track the membership tier (Basic, Plus, Pro) for logged-in members.

### 3.3 Marketing & campaigns
- Capture the external campaign tracking code (`cid` query parameter) and attribute orders to it.
- Track internal banner / promotion impressions and clicks with the banner ID and placement.
- Track newsletter sign-ups (footer form and checkout opt-in) as an event with the form location.

### 3.4 Product discovery
- Product listing pages: track the category, applied filters and sort order.
- Product detail pages: track product views with SKU, product name, category and price.
- Track recommendation widget clicks ("You may also like") with the widget name and position.
- Internal search — see [Site search requirements](flows/search.html).

### 3.5 Cart & checkout
- Track add-to-cart and remove-from-cart with product SKU, quantity and price, and where the add happened (PDP, quick view, recommendation).
- Track cart views.
- Checkout funnel and orders — see [Checkout funnel requirements](flows/checkout.md).

### 3.6 Content engagement
- Track buying-guide article views with the article title and topic.
- Track product video plays, 50% milestones and completions with the video name.
- Track PDF size-chart downloads with the file name.

## 4. Reporting needs

- Weekly dashboard: visits, orders, revenue, conversion rate by market, device and marketing channel.
- Funnel report: product view → add to cart → checkout start → order, by device.
- Search report: top keywords, zero-result keywords, search-to-order conversion.
