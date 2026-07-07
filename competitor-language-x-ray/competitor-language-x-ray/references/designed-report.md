# Designed Ecommerce Report Reference

Use this only when the user asks for a polished PDF, deck-like report, client-ready brief, or shareable intelligence asset.

## Render Approach

Create a self-contained HTML report with embedded CSS and render it to PDF with WeasyPrint when available. If WeasyPrint is unavailable, use a simpler HTML/PDF or Word document fallback and state the limitation.

Always visually inspect rendered pages before delivery when browser/PDF rendering tools are available.

## Visual Structure

1. **Cover**
   - Report title
   - ecommerce market/category
   - targets researched
   - run date
   - evidence legend: CONFIRMED, REPORTED, INFERRED, RAW VOICE

2. **Executive Scoreboard**
   - threat ranking bars
   - biggest buyer desire
   - strongest offer gap
   - strongest customer-language pattern
   - biggest proof/PDP gap
   - biggest evidence gap

3. **Competitor Cards**
   - position and one-line read
   - hero product/category
   - audience vs buyer
   - funnel path
   - offer stack and price architecture
   - proof/mechanism
   - PDP/CRO notes
   - creative/ad notes
   - quant callouts
   - bad-review edge
   - links

4. **Offer Stack Comparison**
   - price and compare-at price
   - bundles and quantity breaks
   - subscription incentive
   - free gift/BOGO
   - shipping threshold
   - guarantee/warranty/returns
   - urgency/scarcity
   - upsell/retention signals
   - visible weakness/opportunity

5. **Customer-Language Heatmap**
   - desire clusters
   - pain clusters
   - failed attempts
   - objections
   - proof demands
   - review wounds
   - tone markers
   - language to avoid

6. **Avatar And Angle Map**
   - core buyer avatar
   - sub-avatar cards
   - desire + behavior + gap
   - belief shift / angle
   - hook direction
   - proof needed
   - PDP/ad/offer implication

7. **Opportunity Summary**
   - what to borrow carefully
   - what to avoid
   - where to differentiate
   - offer tests
   - PDP/CRO tests
   - creative tests
   - research gaps

8. **Sources And Gaps**

## Design Tokens

Use a restrained intelligence-report style:

- ink: `#14233A`
- accent: `#E8743B`
- green evidence: `#1F8A57`
- amber evidence: `#C0791F`
- gray evidence: `#6B7280`
- blue link/accent: `#2A6FDB`
- background: `#F6F8FB`
- cards: white with 1px `#E4E9F0`, 8px radius

Avoid decorative clutter. The report should feel like strategy, not a landing page.

## Page Rules

- Keep text scannable.
- Do not put huge raw-comment lists in the designed report.
- Use tables for comparison, cards for competitors, and callouts for key buyer language.
- Make source links visible in the appendix.
- Keep exact customer quotes short.
- Keep ecommerce numbers clearly labeled as confirmed, reported, or inferred.

## HTML Skeleton

```html
<main>
  <section class="cover">...</section>
  <section class="scoreboard">...</section>
  <section class="competitors">...</section>
  <section class="offers">...</section>
  <section class="language">...</section>
  <section class="angles">...</section>
  <section class="sources">...</section>
</main>
```

Use CSS page breaks before major sections and avoid breaking competitor cards across pages.