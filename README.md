# The-Pant-Project# The Pant Project Growth Report

An interactive brand growth report on [The Pant Project](https://pantproject.com/), written as an independent analysis by a brand manager. It is a single HTML page: no build step, no backend, no accounts.

**Analysis by:** Mishita Maggo
**Built from:** two research documents ("The Pant Project Overview" and "Executive Summary"), which draw on press coverage, pantproject.com and public forums.
**Date:** 14 October 2026
**Not affiliated with The Pant Project.** The author has not seen the company's internal data.

---

## What the report says

> Fit earned the trust. Speed earned the growth. Consistency decides FY27.

| Finding | Evidence |
|---|---|
| Growth came from a fix | Revenue went from ₹1.0 Cr (FY21) to ₹40.7 Cr (FY25). The pivot was from custom-only trousers (10–14 days) to ready-made sizes built from custom-order measurements (48-hour dispatch, under an hour on Blinkit). |
| The fit promise sits on the wrong product | The 93% first-time fit rate and two free alterations belong to custom orders. Ready-made gets size exchange only, and carries the volume. |
| Complaints point at stitching, not fabric | Public threads report seams and pocket stitching failing after 5 to 10 washes. Colour and shrinkage hold up. |
| The tag price has stopped meaning anything | Tags run ₹2,990–4,990, prices paid ₹1,690–2,590. At the midpoints that is about 46% off. |
| FY27 depends on stores | The company plans 120–150 stores. The research names 8 today. At one opening a month, 120 stores take over nine years. |

## What you can do on the page

| Section | Interaction |
|---|---|
| Growth | Type an FY26 revenue and move four sliders (growth, new stores, orders per day, order value) to see what reaching ₹160 Cr in FY27 takes. |
| Trust | Switch between Ready-made, Made-to-measure and Marketplace. Filter customer feedback (All, Holds, At risk) and tap an item to expand it. |
| Price | Slide a price against the tag range to see the discount. |
| Stores | Test one mature store's economics, redraw the rollout map, and check a new city against a go or no-go line. |
| Moves | Five moves, each with why, first step and a test. Arrow keys work. |
| Theme | A Light/Dark toggle sits in the top bar. |

## How the numbers are worked out

Every figure marked "my arithmetic" on the page is calculated from reported numbers. Nothing is estimated from outside the research.

| Figure | Calculation |
|---|---|
| **+98% a year** | √(160 ÷ 40.7) = 1.98, the yearly growth needed from FY25 to FY27 |
| **≈ ₹81 Cr FY26** | √(40.7 × 160) = 80.7, the midpoint on a steady path. FY26 actuals are not public. |
| **8.2 orders a day per store** | ₹1.8 Cr a year ÷ ₹6,000 per order ÷ 365 days. Both inputs come from the company's own store targets. |
| **46% under the tag** | 1 − (₹2,140 ÷ ₹3,990), the midpoints of the price-paid and tag ranges |
| **9+ years to 120 stores** | (120 − 8 stores) ÷ 1 opening a month ÷ 12 |
| **3–4 openings a month** | (120 − 8 stores) ÷ 36 months = 3.1 |
| **≈ 320 orders a day in FY25** | ₹40.7 Cr ÷ ₹3,500 average order ÷ 365. The ₹3,500 is the midpoint of the reported ₹3,000–4,000 online order. |
| **Monthly spend ceiling** | Monthly gross profit minus cost to open ÷ payback months. Store running costs are not public, so this shows a ceiling, not a payback. |

## Assumptions to know about

- **The FY26 starting figure is a placeholder** (₹80.7 Cr, the steady path). Replace it with the real number if you have it.
- **New stores in the what-if open evenly through FY27 and run at full pace from day one.** The calculator counts half a year of revenue per new store. This is generous.
- **"Open today" is 8**: 4 own stores (Bandra, Hyderabad, Bengaluru, Jaipur) and 4 shop-in-shops inside White Crow stores (Surat, Ahmedabad, Kochi, Indore). The real count may be higher.
- **Gross margin of 55–60%** is the company's target, not a reported result.
- **The go or no-go line (8 orders a day)** is derived from the company's own ₹1.8 Cr per mature store target. It is a rule of thumb, not a benchmark.

## Where the sources disagree

The two research documents conflict in places. The page's collapsed note shows what I used.

| Item | Source A | Source B | Used |
|---|---|---|---|
| Own-site reviews | 24,000+, 94% positive | 12,241, 81% positive | The newer one |
| Series A | $4.25M, June 2024 | 2023, also called "bootstrapped" | June 2024 |
| Customers measured | 500,000+ | 30,000+ by 2022 | Not used. FY25 revenue implies about 116,000 orders. |
| "40x growth" | Placed under FY27 | — | It fits FY21 to FY25. FY27 would be 160x. |

## Limits of this analysis

- Based on public information only. Each "number to watch" is a question, not a verdict.
- Nothing was checked against the live site.
- Missing data that would change the conclusions: FY26 revenue by channel, return rates by channel, repeat-buyer rate, cost to win a customer, store profit and loss, and marketplace share and margin.

## Files

```
pant-project-growth-report.html   The report (single file, HTML + CSS + JS)
README.md                         This file
```

## Running it

Open the HTML file in any modern browser. It needs an internet connection only to load two Google fonts (Archivo and Manrope). If they fail to load, it falls back to the system font and everything still works.

## Sharing it

1. **Published link:** use the Share menu on the published page and allow anyone with the link to view it. Test the link in a private window before posting.
2. **Your own hosting:** upload the single HTML file to any static host (Netlify, GitHub Pages, Vercel). No configuration is needed.
3. **LinkedIn:** the post text works best on its own, with the link in the first comment.

## Editing it

All content lives in one file.

| To change | Look for |
|---|---|
| Colours and fonts | The `:root` block at the top of `<style>`. Light and dark values are defined separately. |
| Revenue chart | The `bars` array in the script |
| What customers say | The `R` array |
| Channel details | The `CH` object |
| The five moves | The `M` array |
| Default slider values | The `value` attributes on each `<input>` |
| Byline | The `.by` line under the headline |

## Credits

Typefaces: Archivo and Manrope via Google Fonts. No libraries or frameworks.