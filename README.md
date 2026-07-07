# Competitor Language X-Ray

**Give Codex and Claude an ecommerce competitor research brain.**

> Drop in a Shopify store, DTC brand, Amazon product, product category, or buyer avatar and get a structured ecommerce x-ray: funnels, offers, pricing, bundles, subscriptions, PDP/CRO, Meta/TikTok ad angles, Shopify apps/themes, review wounds, buyer language, objections, proof gaps, and next tests.

Codex / generic skills:
```bash
git clone https://github.com/mrb0ats/competitor-language-x-ray ~/.codex/skills/competitor-language-x-ray
```

Claude Code / manual skills:
```bash
git clone https://github.com/mrb0ats/competitor-language-x-ray ~/.claude/skills/competitor-language-x-ray
```

Claude Desktop / claude.ai-style skill import: download `competitor-language-x-ray.skill` from the repo or latest release and import it into your Skills / Capabilities settings.

Zero config to start. The skill uses live sources during each run and asks the agent to cite evidence instead of relying on static claims. If a source, price, app, theme, or review pattern cannot be verified, the correct output is `not found` or `not verifiable`, not a guess.

## What's inside

- **Ecommerce competitor x-ray** - positioning, audience vs buyer, funnel, offer stack, price architecture, proof, paid-social maturity, PDP/CRO, bad-review edges, links, and threat ranking.
- **Buyer-language mining** - real buyer words from Reddit, forums, YouTube/TikTok comments, Amazon reviews, marketplace reviews, public communities, and competitor one-star reviews.
- **Shopify app/theme detection** - asks the agent to check visible app and theme signals with tools such as TrendTrack Shopify Apps Detector, Koala Shopify App Detector, and Koala Shopify Theme Detector.
- **Offer and angle synthesis** - turns desire + behavior + gap into angles, hook directions, proof needs, PDP tests, bundle tests, subscription tests, and landing-page tests.
- **Evidence discipline** - separates `CONFIRMED`, `REPORTED`, `INFERRED`, and `RAW VOICE` so strategy does not blur facts with guesses.

---

Most competitor research stops at "they run ads" or "their landing page looks good." That is not enough for ecommerce.

A useful x-ray should show how the store actually sells: what promise appears above the fold, what apps and theme signals are visible, how the offer raises AOV, what review wounds create objections, what buyers say before purchase, and what angle is worth testing next.

`competitor-language-x-ray` is built for that kind of work.

## What people use it for

**Reverse-engineer Shopify stores.** Compare visible apps, theme, PDP structure, bundles, subscriptions, review stack, cart/upsell flow, proof blocks, and paid-social angles.

**Find buyer language before writing ads.** Give it a category or avatar and ask for the phrases, fears, failed attempts, objections, and proof demands buyers repeat in the wild.

**Build angle maps.** Turn customer language into sub-avatar angles, hooks, native image/UGC concepts, PDP proof blocks, advertorial tests, and offer tests.

**Rank threats.** Score competitors by offer strength, funnel depth, proof strength, paid-social maturity, tech-stack maturity, momentum, customer-language fit, and vulnerability.

## How it works

1. **You provide a target.** A store URL, competitor list, Amazon listing, product category, or buyer avatar.
2. **The skill normalizes the request.** It decides whether the job is competitor research, buyer-language mining, offer/angle work, or a full market x-ray.
3. **The agent researches live sources.** Owned pages, PDPs, ad libraries, review surfaces, marketplaces, comments, public communities, Shopify app/theme detectors, and search surfaces.
4. **Findings are tagged by evidence strength.** Confirmed facts, third-party reports, reasoned inference, and raw buyer voice stay separate.
5. **The output becomes ecommerce action.** Hooks, angles, PDP sections, FAQ/objection blocks, proof needs, app/theme observations, bundle tests, and offer tests.

## Install

| Surface | Install |
|---|---|
| **Codex** | `git clone <repo-url> ~/.codex/skills/competitor-language-x-ray` |
| **Claude Code / manual** | `git clone <repo-url> ~/.claude/skills/competitor-language-x-ray` |
| **Claude Desktop / claude.ai-style import** | Download `competitor-language-x-ray.skill` and import it into Skills / Capabilities. |
| **Optional command** | Copy `commands/x-ray.md` into your command folder if your surface supports slash commands. |

### Codex

```bash
git clone <repo-url> ~/.codex/skills/competitor-language-x-ray
```

Then start a new Codex thread and ask:

```text
Use $competitor-language-x-ray to research these Shopify stores: brand1.com, brand2.com, brand3.com
```

### Claude Code / manual

```bash
git clone <repo-url> ~/.claude/skills/competitor-language-x-ray
```

Optional slash command:

```bash
cp ~/.claude/skills/competitor-language-x-ray/commands/x-ray.md ~/.claude/commands/x-ray.md
```

Then use:

```text
/x-ray brand1.com brand2.com "category: sleep supplements"
```

### Skill bundle

Use the packaged file when your AI surface supports `.skill` uploads:

```text
competitor-language-x-ray.skill
```

## Usage

```text
Use competitor-language-x-ray to research AG1, Beam, and MoonBrew. I want offers, funnel, pricing, bad reviews, PDP/CRO notes, and the customer language around people who cannot stay asleep.
```

```text
Research these Shopify stores: brand1.com, brand2.com, brand3.com. Compare their Meta ads, landing pages, PDPs, Shopify apps/themes, bundles, guarantees, subscriptions, review wounds, and biggest threat.
```

```text
My product category is dog water fountains for anxious pet owners. Find buyer language from Reddit, YouTube, TikTok, Amazon reviews, and competitor one-star reviews. Turn it into angles, hooks, proof needs, and offer tests.
```

```text
Use competitor-language-x-ray on this Amazon listing and its top alternatives. I want review wounds, proof gaps, buyer objections, and better offer ideas.
```

## Shopify apps and themes

For Shopify stores, the skill asks the agent to check visible app/theme signals with sources such as:

- TrendTrack Shopify Apps Detector - `https://www.trendtrack.io/tools/shopify-apps-detector`
- Koala Shopify App Detector - `https://koala-apps.io/tools/app-detector/`
- Koala Shopify Theme Detector - `https://koala-apps.io/tools/theme-detector/`

Detector results should be treated as `REPORTED` unless confirmed through visible storefront code or owned pages. Backend-only, private, heavily customized, or obfuscated apps may not be detectable. The skill should say that plainly instead of guessing.

## Output formats

Default output is a chat brief. For larger jobs, ask for:

- **Spreadsheet matrix** - best for 5+ competitors or large language banks.
- **Word doc** - best for a clean internal/client report.
- **Designed report** - best for shareable PDF/HTML-style intelligence assets.

## Limits

- **No private platform access.** The skill does not log into ad accounts, Shopify admins, private communities, or paid tools unless the user provides access inside the current environment.
- **Detector visibility is limited.** Shopify app/theme detectors cannot reliably see every backend, private, customized, or obfuscated integration.
- **Live source quality varies.** If reviews, comments, ads, or detector results are blocked or unavailable, the report should name the gap.
- **Not a measured index by default.** Threat rankings are strategic judgments unless the user asks for a transparent scoring table.

## Structure

```text
.
├── competitor-language-x-ray/        # skill folder for Codex and Claude-style skills
│   ├── SKILL.md                      # main skill contract
│   ├── agents/openai.yaml            # UI metadata
│   ├── references/                   # research and output guides
│   └── evals/evals.json              # example eval prompts
├── commands/x-ray.md                 # optional slash-command shortcut
├── competitor-language-x-ray.skill   # packaged skill bundle
├── INSTALL.md                        # detailed install notes
└── LICENSE
```

## Develop

After editing the skill folder, validate it:

```powershell
python "$env:USERPROFILE\.codex\skills\.system\skill-creator\scripts\quick_validate.py" ".\competitor-language-x-ray"
```

Rebuild the `.skill` bundle from the repo root:

```powershell
Compress-Archive -Path ".\competitor-language-x-ray" -DestinationPath ".\competitor-language-x-ray.zip" -Force
Copy-Item ".\competitor-language-x-ray.zip" ".\competitor-language-x-ray.skill" -Force
Remove-Item ".\competitor-language-x-ray.zip"
```

## Open source

MIT license. Created by **Mr. Boats**.

---

[LICENSE](LICENSE)
