# Ecommerce Customer-Language Mining

Use this when the user gives an ecommerce ICP, buyer avatar, product category, niche, competitor customer base, or asks for "customer language", "voice of customer", reviews, Reddit research, TikTok/YouTube comments, objections, pains, tone, hooks, angles, or offer ideas.

The goal is not generic market research. The goal is to find the exact language buyers use before, during, and after buying physical products, then turn that language into ad, PDP, offer, and funnel decisions.

## Source Priority

Start with sources where ecommerce buyers naturally complain, compare, ask, and justify purchases:

1. Amazon reviews and Q&A, especially one-star, three-star, and "most helpful" reviews.
2. Competitor PDP reviews, Trustpilot, Google reviews, Etsy, Walmart, TikTok Shop, Meta shop, App Store only when the product has an app component.
3. Reddit threads and comments, niche forums, public communities, Facebook group posts if public, Discord/Slack only if user-provided.
4. YouTube comments under product reviews, routines, transformations, comparisons, and "best X" videos.
5. TikTok comments under competitor ads, UGC, product demos, routines, and creator reviews when accessible.
6. Search autocomplete, People Also Ask, query modifiers, and public Q&A surfaces.
7. Public podcasts, interviews, testimonials, call transcripts, or survey data supplied by the user.

Use software/app review sites only when the ecommerce product is actually an app-enabled product. Otherwise stay on ecommerce buyer, marketplace, review, and community sources.

## Search Seeds

Turn the product/category/problem into many query families:

- "[product/category] reddit"
- "[product/category] forum"
- "[product/category] reviews"
- "[product/category] Amazon reviews"
- "[product/category] Q&A"
- "[competitor/product] reviews"
- "[competitor/product] complaints"
- "[competitor/product] does it work"
- "[competitor/product] worth it"
- "[competitor/product] dupe"
- "[competitor/product] alternative"
- "[competitor/product] side effects"
- "[competitor/product] broke"
- "[competitor/product] returned"
- "[competitor/product] shipping"
- "[competitor/product] subscription"
- "[problem] does anyone else"
- "[problem] I hate"
- "[problem] I wish"
- "[problem] tried everything"
- "[product/category] not working"
- "[desired outcome] without [hated tradeoff]"
- "[symptom/trigger moment] what do I do"
- "best [product/category] for [specific use case]"
- "[product/category] before after"
- "[product/category] routine"
- "[product/category] TikTok made me buy it"

For products with health, beauty, wellness, supplements, pets, babies, finance, safety, or regulated claims, also search skepticism and risk language:

- "[product/category] safe"
- "[product/category] scam"
- "[product/category] side effects"
- "[product/category] allergic"
- "[ingredient/material] concern"
- "[claim] evidence"
- "[claim] before after real"

## Collection Target

Adjust by depth:

- quick scan: 10-20 raw snippets from 3+ source types
- standard brief: 30-60 raw snippets from 5+ source types
- deep report: 80+ snippets, separated by segment, source type, and purchase stage

If available sources are thin, say so and explain where evidence was scarce.

## What To Extract

For each useful snippet, capture:

- source URL and source type
- date if visible
- product/competitor/category context
- purchase stage: pre-purchase, comparison, first use, repeat use, return/cancel, post-purchase review
- short exact phrase (RAW VOICE) or paraphrase
- tag: desire, pain, trigger, failed attempt, objection, proof demand, current workaround, competitor complaint, identity, anti-language, offer reaction, shipping/service wound, product-defect wound
- emotion: anger, shame, fear, hope, skepticism, pride, overwhelm, impatience, status, relief, confusion, embarrassment, disappointment
- awareness: unaware, problem aware, solution aware, product aware, most aware, or heavily skeptical
- commercial implication: ad hook, PDP proof, offer test, guarantee, FAQ, bundle, upsell, retention, creative concept, product improvement

## Pattern Categories

Cluster raw language into:

1. **Desires**: what they want, including surface outcomes and deeper emotional outcomes.
2. **Pains**: what hurts now, especially repeated trigger moments and social moments.
3. **Failed attempts**: products, routines, hacks, advice, competitors, or home remedies they tried.
4. **Objections**: what they doubt before buying.
5. **Proof demands**: what would make them believe, such as before/after, ingredient proof, durability tests, expert proof, review count, comparison demos, or third-party validation.
6. **Identity language**: how they describe themselves and who they do not want to be.
7. **Competitor wounds**: what alternatives failed to deliver.
8. **Product wounds**: defects, fit issues, taste/smell/texture, sizing, materials, packaging, setup, usability, side effects, durability, subscription/cancel friction, shipping, returns, customer support.
9. **Outcome language**: how they describe success in their own words.
10. **Offer reactions**: how buyers respond to price, bundle, subscription, free gift, discount, guarantee, shipping threshold, trial, warranty, or financing.
11. **Anti-language**: phrases that feel overused, fake, too clinical, too aggressive, too salesy, or misaligned.

## Avatar Model

Build avatars from buying likelihood, not generic demographics.

Prefer these building blocks:

- desire: what they want
- experience: what happened to them
- behavior: what they currently do or have already bought/tried
- emotion: how it makes them feel
- buying context: urgency, occasion, routine, household, life stage, pet/child/body/home context, budget, channel preference
- demographic/context: age, gender, location, income, only when useful for targeting or product fit

Create:

- **Core buyer avatar**: one main buying group, ideally desire-, experience-, or behavior-led.
- **Sub-avatars**: narrower combinations that create more relatable angles.
- **Beliefs**: derive from desire + experience + emotion + behavior; do not use belief as the only avatar definition.

Belief unpacking prompt:

```text
They believe: [belief].
What happened that made them believe this?
How does that belief make them feel?
What do they do or avoid because of this belief?
What desire is still alive underneath it?
What proof would break or soften the belief?
What product, offer, or page element would answer it?
```

## Language Bank Format

Use a table or bullets:

| Cluster | Customer words | Meaning | Source pattern | Ecommerce use |
|---|---|---|---|---|
| Desire | "feel normal again" | Wants control and relief | repeated in comments/reviews | angle: regain control without feeling deprived |
| Objection | "I don't want another subscription trap" | Fear of cancellation friction | repeated in one-star reviews | PDP/checkout: plain-language cancel policy |

Keep exact quotes short. For longer customer comments, summarize and preserve only the most useful phrase.

## Desire Validation

Before turning language into angles, score each major desire:

- **Urgency**: how badly and how soon do they want this solved?
- **Staying power**: is this desire persistent, recurring, or only a short-lived curiosity?
- **Scope**: how many people in the reachable market share it?
- **Evidence density**: how often does it appear across sources?
- **Commercial fit**: can the user's product or offer credibly satisfy it?
- **Purchasing friction**: what price, proof, trust, shipping, routine, or risk issues might stop them?

Prefer the desires that score high across urgency, staying power, scope, evidence density, and commercial fit. Keep lower-scoring desires as secondary angles or future tests.

## Angle Extraction

Use this route:

1. Product/offer benefit
2. Why the buyer wants that benefit
3. Desire behind it
4. Current behavior, product, routine, or failed attempt
5. Gap in that behavior or product
6. Belief shift / angle
7. Hook direction
8. Proof needed
9. Awareness level
10. Offer/PDP implication
11. Angle priority

Formula:

```text
Desire + current behavior + gap = angle.
Angle + proof + tone = hook direction.
Hook direction + offer/PDP implication = test plan.
```

Example structure:

```text
Sub-avatar: people who want restorative sleep and already avoid screens at night.
Behavior: no screens one hour before bed.
Gap: light still enters the room for eight hours.
Angle: your discipline is being wasted by the room environment.
Hook direction: "No screens for 1 hour. No light for 8."
Proof needed: blackout test, light explanation, before/after sleep data.
Ecommerce implication: PDP above-the-fold demo, native image ad, bundle with sleep mask, FAQ on fit/comfort.
```

## Angle Priority Filters

After generating possible angles, narrow to the 3-5 strongest. Score each angle by:

- **Avatar language fit**: does it sound like the buyer conversation, not marketer language?
- **Emotional voltage**: would the buyer feel seen, exposed, relieved, or understood?
- **Problem-solution clarity**: is the bridge from pain/desire to product obvious enough?
- **Mechanism alignment**: does the product have a credible reason it can solve the problem differently or better?
- **Whitespace/freshness**: are competitors already hammering this exact frame, or is there an opening?
- **Awareness fit**: does the angle match how educated or skeptical the market already is?
- **Offer fit**: can the angle be supported by a credible bundle, guarantee, comparison, trial, or PDP proof block?

Do not launch 20 weak angles because the research produced 20 insights. Pick a small number of high-probability angles, then create multiple ad concepts or hooks around each.

## Hook Quality Rules

A hook should qualify the right person, not only stop anyone. Check:

- Does it speak to the exact buyer segment?
- Does it match their current emotional state?
- Does it imply the angle without needing too much cognitive work?
- Is it specific enough to avoid generic clickbait?
- Does it fit the awareness level?
- Can the product page, offer, or proof actually pay off the promise?

## Validation Rules

- Do not let AI invent customer language.
- Do not turn isolated comments into universal truths.
- Prefer repeated phrases, repeated emotional patterns, or repeated situations.
- Include dissent and skepticism if it appears.
- Cite source URLs for each cluster or representative snippet.
- Separate product complaints from fulfillment/service complaints.
- Treat regulatory, medical, and safety claims conservatively.
- If comments are inaccessible due to login walls, use public alternatives and name the gap.