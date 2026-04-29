# Pally — concept homepage for Cyngn DriveMod Tugger

A reimagined homepage for [Cyngn Inc.](https://www.cyngn.com) (NASDAQ: CYN), built as a portfolio asset for the Head of Revenue Operations role.

**Live demo:** _(add Vercel URL after deploy)_

---

## What this is

Cyngn currently positions itself as a broad industrial autonomy platform — multiple product lines, multiple use cases, AMR-vs-AGV explainers in the hero. That positioning is correct for a $200M ARR company. Cyngn is at $4M ARR.

This concept tests a different bet: **collapse the surface area, name the lead product, and let a configurator do the qualifying work the sales team is doing today**.

The headline product — the DriveMod-enabled Motrec MT-160 tow tractor — gets a name (**Pally**) and a personality. The homepage stops being a platform overview and starts being a hiring decision: *"Pally is the headcount you couldn't fill."*

This is the framing the labor market is asking for, and it isn't on the current site.

---

## Strategic thesis

| Move | Rationale |
|---|---|
| **Single-product hero** | $4M ARR companies break through with focus, not breadth. Tugger is the highest-volume deployment, has the cleanest ROI math, and concentrates Cyngn's reference customers (G&J Pepsi, Coats, Vann Family Orchards, U.S. Continental). |
| **Named character (Pally)** | Naming compresses Cyngn → DriveMod → Tugger → SKU into a single mental model. iRobot did it with Roomba. Boston Dynamics did it with Spot. Naming is the cheapest moat available. |
| **"Hire Pally" framing** | The buyer's two anxieties are *will this work* and *am I firing my people*. The math section answers the first. Pally's voice ("I'm not replacing your team — I'm the hire you couldn't make") answers the second. The current site doesn't address question two at all. |
| **Configurator-as-interview** | Inverts the buyer power dynamic. Most B2B configurators feel like *the prospect getting qualified*. Pally's interview frames it as *the prospect doing the qualifying*. Tiny psychological shift; meaningfully lower form-completion friction. |
| **Light industrial palette** | The buyer's reference set is Toyota Material Handling, Crown, Raymond, Caterpillar — not Tesla and Linear. Light cream + safety orange reads as "real equipment from a real company," not "Silicon Valley experiment." |
| **Math section in dark** | Financial reckoning sections benefit from visual gravity. The single inversion in an otherwise light page makes the comparison feel weightier. |
| **References as outcomes** | Each customer card leads with a number (4× efficiency, 4 Pallys deployed, #1 Pepsi bottler), not a logo. Outcomes self-qualify the buyer's vertical. |

---

## What's intentionally not in this build

These are decisions, not omissions:

- **DriveMod Forklift** — listed as "select customers only" on the current Cyngn site, which signals pre-product. Putting it on the homepage dilutes the tugger story and signals scope creep. Add when forklift hits 10 commercial deployments; until then, focus is the only competitive advantage available.
- **AMR-vs-AGV explainer** — eats valuable real estate educating buyers who already know what they're looking for. A buyer Googling "autonomous tugger" doesn't need the category defined; they need to convert.
- **"Trusted by" logo wall** — replaced with named outcomes. Logos are decoration; outcomes are arguments.
- **Generic "Get Demo" CTA** — replaced with a configurator that captures sizing context before sales gets the lead. The handoff is closing-stage, not discovery-stage.

---

## Design decisions

**Typography**
- **Fraunces** (variable serif) — Pally's voice. Used for his greeting, section titles, customer quotes, and the closing CTA. Storytelling moments only.
- **Archivo** (industrial sans) — operational copy. Configurator questions, product specs, structural headers. Anything the buyer reads and clicks.
- **Manrope** — body text.
- **JetBrains Mono** — numerical specs and stats.

The principle: **personality belongs around the conversion mechanism, not inside it.** Pally narrates around the configurator. The configurator itself is ruthlessly clear.

**Color**
- Cream background (`#F5F1E8`) — warm industrial, references Caterpillar / Deere brochures
- Near-black ink (`#1B1B1F`) — text and primary CTAs
- High-vis safety orange (`#FF5F1F`) — accent. Same orange as warehouse floor markings and tugger LED indicators. Industrial buyers recognize it on sight.

**Custom Pally avatar**
Built as inline SVG. Geometric tugger silhouette — orange body, dark cab, LiDAR sensor with the orange ring on top, subtle yellow LED strip that reads as a face without being cartoonish. Scales from 132px (hero) to 48px (configurator) to 80px (closing CTA). Same character across every appearance.

---

## Tech notes

- **Single static HTML file.** No build step. No framework. ~2,000 lines, ~65KB, ~75KB transferred including Google Fonts.
- **Vanilla JS configurator.** Five-step flow with progress indicator, real-time ROI estimation based on inputs, contact form, results page. No external dependencies.
- **Fully responsive.** Desktop-optimized but works at tablet and mobile widths.
- **Accessible defaults.** Semantic HTML, sufficient contrast, keyboard-navigable.

---

## Deploy to Vercel

This is a static site — Vercel auto-detects and deploys without configuration.

### Option 1: GitHub → Vercel (recommended)

```bash
# 1. Push this directory to GitHub
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/pally-concept.git
git push -u origin main

# 2. Go to vercel.com/new
# 3. Import the repo
# 4. Vercel auto-detects: Framework = Other, no build command
# 5. Click Deploy
```

Auto-deploys on every push to `main`.

### Option 2: Vercel CLI

```bash
npm i -g vercel
cd pally-concept
vercel
```

Follow the prompts. First deploy creates a preview URL; running `vercel --prod` promotes to production.

---

## Local preview

No build step required. Just open `index.html` in a browser, or run a simple static server:

```bash
# Python 3
python3 -m http.server 8000

# Or Node
npx serve .

# Then visit http://localhost:8000
```

---

## Disclaimer

This site is a portfolio mockup built by Nizam Ali as part of the interview process for the Head of Revenue Operations role at Cyngn Inc. (NASDAQ: CYN).

It is **not affiliated with, endorsed by, or sponsored by Cyngn Inc.** All Cyngn brand references, customer names (G&J Pepsi, Coats, Vann Family Orchards, U.S. Continental, Arauco, DHL), and product details are drawn from publicly available sources (cyngn.com, SEC filings, press releases) and used illustratively to demonstrate strategic and design thinking.

ROI numbers shown in the math section are illustrative inputs intended to demonstrate a customer-facing comparison framework, not Cyngn's published unit economics. Cyngn's published metrics (33% productivity boost, 64% labor cost reduction, 18-month payback) are credited to Cyngn customer ROI analyses.

The "Pally" name and character were created by Nizam Ali for this exercise and are not Cyngn's actual product brand.

---

## Author

Built by [Nizam Ali](https://www.linkedin.com/in/nizamtali) — senior GTM and Revenue Operations professional.

License: [MIT](./LICENSE)
