# Ecommerce Competitor Research Agent

Use this prompt structure for each ecommerce competitor, Shopify store, product, PDP, landing page, advertorial, ad library, Amazon listing, or marketplace listing.

```text
Research "[TARGET]" as an ecommerce competitor. Target type: [DTC brand / Shopify store / Shopify app/theme stack / Amazon brand / dropshipping product / product page / landing page / advertorial / TikTok Shop brand / marketplace listing / creator-led physical-product brand / unknown]. Known URLs or handles: [URLS]. User context: [ANCHOR].

Use live web research heavily. Prioritize the competitor's owned pages, product pages, checkout/offer pages, public ad libraries, Shopify app/theme detector results, marketplace listings, reviews, social profiles, UGC, advertorials, and public customer discussions. If a profile is gated, do not stop; use the website, PDPs, marketplace pages, reviews, snippets, ad libraries, and public comments instead.

Return a tight ecommerce brief with:

1. Identity and positioning: category, hero product, country/market, main promise.
2. Buyer/avatar: audience vs actual buyer, pains, mass desires, trigger moments, current alternatives.
3. Funnel: ad -> landing page/PDP/advertorial -> cart -> checkout -> upsell -> subscription/retention.
4. Offer stack: price, compare-at price, discount, bundle, quantity break, BOGO, free gift, shipping threshold, financing, subscription, guarantee, warranty, returns, trial, urgency/scarcity.
5. Proof and mechanism: claims, ingredients/materials, technology, studies, UGC, reviews, testimonials, before/after, comparison tables, authority, new mechanism, new information, identity angle.
6. Creative strategy: dominant awareness level, mass desire, angle, hook, ad concept, format, visual pattern, native/UGC/VSL/image/ad library notes.
7. Shopify tech stack: theme name/status, visible apps/integrations, app categories, detector source links, customer-journey role, confidence, and gaps.
8. Bad-review edge: what customers complain about, what the audience wants that competitors are not doing, and what the user could prove or offer differently.
9. Quant snapshot: 2-5 numbers that show size/momentum; review count/rating, ad volume, traffic range, social following, Amazon rank if visible, visible bestseller signals, price range, launch velocity.
10. Links directory: homepage, PDPs, landing pages, advertorials, ad library, socials, Amazon/marketplace listing, reviews, checkout/store links, app/theme detector links.
11. Sources and confidence note.

Evidence rules:
- CONFIRMED = owned/authoritative page, public ad library, official listing, checkout, official policy, or official profile.
- REPORTED = self-reported or third-party estimate.
- INFERRED = reasoned conclusion from visible funnel, ads, reviews, and patterns.
- Do not invent prices, offers, reviews, sales, follower counts, traffic, or revenue.
```

## Source Order

Work this order unless the target type clearly suggests a better path:

1. official website, PDP, pricing, checkout, bundles, subscription, policies, shipping/returns/warranty pages
2. landing pages, advertorials, quiz funnels, upsells, post-purchase flow if visible
3. Meta Ad Library, TikTok Creative Center, Google Ads Transparency Center, YouTube/Shorts/TikTok/Instagram profiles
4. Shopify app/theme detectors when the target is a Shopify store: TrendTrack Shopify Apps Detector (https://www.trendtrack.io/tools/shopify-apps-detector), Koala Shopify App Detector (https://koala-apps.io/tools/app-detector/), and Koala Shopify Theme Detector (https://koala-apps.io/tools/theme-detector/)
5. Amazon, TikTok Shop, Etsy, Walmart, app/marketplace listings when relevant
6. review surfaces: Amazon reviews/Q&A, Trustpilot, Google reviews, Reddit threads, niche forums, marketplace reviews, app reviews
7. social proof and UGC: tagged content, testimonial pages, creator ads, comments
8. third-party directional data: traffic estimates, ad volume, social following, bestseller rank, trend/launch signals

## Ecommerce Capture Checklist

Always capture:

- hero claim and above-the-fold promise
- product price range, compare-at pricing, and quantity economics
- bundle logic and reason to buy more
- discount structure: percent off, dollar off, BOGO, bundle and save, gift with purchase, free shipping threshold
- guarantee/warranty/returns/trial/financing/subscription
- proof hierarchy: reviews, UGC, clinical/study claims, mechanism, comparison table, before/after
- mechanism: material, ingredient, device, protocol, design, sourcing, manufacturing, tech, or "why this works"
- PDP/ad objections handled and objections ignored
- competitor complaints from one-star and three-star reviews
- ad angles and hooks from active ads
- native/UGC/image/VSL patterns and whether the ad feels organic or obviously branded
- Shopify theme name/status when detectable, including standard theme vs customized/headless/unknown
- visible Shopify apps and integrations when detectable, especially review, quiz, popup, email/SMS, subscriptions, cart/upsell, loyalty, bundles, tracking, returns, support, and analytics apps
- detector source and confidence: use TrendTrack/Koala results as REPORTED unless confirmed by visible storefront code or owned pages
- app-detection gaps: backend-only, private, heavily customized, or obfuscated apps may not leave visible traces; mark these as not verifiable instead of guessing

## Awareness And Master Research Layer

For deeper ecommerce or paid-social work, create five layers before final synthesis:

1. **Market awareness research**: estimate the market across unaware, problem aware, solution aware, product aware, and most aware. Use public discussion, search results, reviews, competitor ads, and category maturity. The dominant awareness level guides hooks and landing-page education depth.
2. **Competitor research**: identify direct and adjacent competitors, offers, prices, review/social proof, ad angles, mechanisms, promises, and customer complaints.
3. **Avatar/psychographic research**: extract pains, beliefs, desires, behaviors, current solutions, language, and demographic context from real buyers.
4. **Master research synthesis**: combine awareness, competitor, and avatar findings into one operating brief so copy and landing pages do not drift away from evidence.
5. **Desire validation**: turn possible desires into a ranked shortlist using urgency, staying power, scope, evidence density, and product fit. Only then create angle tests.

If traffic, demographic, ad-volume, or marketplace tools are available, use them as directional inputs, not final truth. Treat estimates as REPORTED.

## Angle vs Execution Distinctions

When reviewing competitor ads, separate:

- **Mass desire**: what the buyer deeply wants.
- **Angle**: the belief shift or story that activates the desire now.
- **Hook**: the first line/visual that earns qualified attention.
- **Offer**: the deal structure, discount, bundle, guarantee, shipping threshold, or incentive.
- **Ad concept**: the creative execution, format, visual style, script, UGC, VSL, native image, or advertorial.

Do not call every hook, discount, visual format, or competitor template an angle. The strategic question is: what belief does this ad make easier to accept?

## Offer Stack Notes

For each offer, note:

- single-unit price vs bundle price
- quantity break and effective unit economics
- reason for the bundle, if provided
- shipping threshold and whether it nudges AOV
- free gift/ebook/complementary product/mystery gift
- subscription discount and cancellation friction
- warranty/guarantee/returns/trial clarity
- financing/payment plans and buy-now-pay-later
- urgency/scarcity and whether it appears real or generic

Flag offers that likely increase AOV, reduce risk, or answer competitor review complaints.