# Triage Map — All 34 Posts (from summary feed, 2026-09-12)

Legend: 🔴 = critical (inline CSS / broken rendering), 🟠 = structural/SEO issue, ✅ = OK

| idx | Slug (short) | Title | Opening state | Issues |
|-----|--------------|-------|---------------|--------|
| 1 | circadian-rhythm | Circadian Rhythm Reset | image→p→TOC→takeaways | ✅ Clean (gold standard) |
| 2 | berberine | Berberine for Weight Loss | `<style>` CSS first | 🔴 CSS block at top, no image-first |
| 3 | healthy-plate | Healthy Plate for Blood Sugar | `<style>` CSS first | 🔴 CSS block at top |
| 4 | natural-glp-1 | Natural GLP-1 Foods | TOC first | 🔴 No featured image/intro before TOC |
| 5 | cortisol-belly | Cortisol Belly 7-Day Plan | comment+TOC | 🟠 No intro paragraph before TOC |
| 6 | alcohol-cancer | Alcohol Cancer Deaths | image→Key Takeaways | 🟠 No TOC, leftover `[38][50]` citation markers |
| 7 | creatine-women | Creatine for Women | image→Key Takeaways | 🟠 No intro para, no TOC |
| 8 | lower-cortisol | Lower Cortisol Naturally | image→Key Takeaways | 🟠 same |
| 9 | magnesium-rich | Magnesium Foods Recovery | image→Key Takeaways | 🟠 same |
| 10 | mobility-hips | Mobility for Stiff Hips | image→Key Takeaways | 🟠 same |
| 11 | protein-moment | Why Protein Is Having a Moment | image→Key Takeaways | 🟠 same |
| 12 | grip-strength | Grip Strength Longevity | image→Key Takeaways | 🟠 same |
| 13 | anti-inflammatory | Anti-Inflammatory Joint Foods | image→Key Takeaways | 🟠 same |
| 14 | evening-routine | Evening Routine for Sleep | image→Key Takeaways | 🟠 same |
| 15 | gut-health-best | Best Foods for Gut Health | SEO-brief comment first | 🟠 brief comment; check image/TOC |
| 16 | high-fiber-and-gut | High Fiber Foods (and gut) | SEO-brief comment first | 🟠 brief comment |
| 17 | high-fiber-that | High Fiber Foods (that work) | SEO-brief comment first | 🔴 DUPLICATE keyword of #16 |
| 18 | lose-weight-fast | Lose Weight Fast Naturally | SEO-brief comment first | 🟠 slug collision `_0802718094` |
| 19 | 9-foods-bp | 9 Foods High Blood Pressure | SEO-brief comment first | 🟠 brief comment |
| 20 | fibermaxxing | Fibermaxxing Explained | paragraph first | 🟠 image not first, no TOC? |
| 21 | sleep-hygiene | Sleep Hygiene Tips | paragraph first | 🟠 image not first |
| 22 | fix-sleep-schedule | Fix Your Sleep Schedule | paragraph first | 🟠 image not first |
| 23 | heart-healthy-eating | Heart-Healthy Eating Plan | paragraph→TOC | 🟠 image not first |
| 24 | japanese-walking | Japanese Walking 30-min | CSS+banner comment | 🔴 CSS at top |
| 25 | morning-routine | Morning Routine Energy | CSS+banner comment | 🔴 CSS at top |
| 26 | one-weekly-walk | One Weekly Walk Belly Fat | CSS+banner comment | 🔴 CSS at top |
| 27 | 7-day-meal-plan | 7-Day Balanced Meal Plan | paragraph→TOC | 🟠 image not first |
| 28 | 10-evidence-tips | 10 Health Tips Women | `body{}` CSS | 🔴 worst — page-wide CSS |
| 29 | walking-after-meals | Post-Meal Walking Glucose | `body{}` CSS | 🔴 worst |
| 30 | strength-training | Strength Training Beginners | `body{}` CSS | 🔴 worst |
| 31 | mental-health | Mental Health Wellness Tips | scoped CSS | 🔴 CSS + bad slug |
| 32 | retatrutide | Lilly Retatrutide Lawsuits | scoped CSS | 🔴 CSS + bad slug |
| 33 | fitness-trackers | Fitness Tracker Benefits | scoped CSS | 🔴 CSS at top |
| 34 | candida-auris | Candida auris Prevention | `html,body{}` CSS | 🔴 page-wide CSS + !important |

## Systematic problems
1. 13 posts start with `<style>` blocks (2 with global `body/html` selectors — break page layout).
2. ~9 posts have SEO-brief `<!-- Primary Keyword... -->` comments at top (leak editorial process).
3. ~14 posts miss required order: featured image → intro paragraph → TOC.
4. Duplicate: #16 vs #17 (same primary keyword "high fiber foods for digestion").
5. Slug problems: #18 suffix `_0802718094`; #31/#32 slugs are image descriptions.
6. #6 has leftover bracketed citation markers `[38][50]` with no link targets.
7. Internal-link + source-link coverage must be verified post by post.

## Gold-standard template (from post #1 circadian, theme v19 classes)
- `<img alt="..." decoding="async" loading="lazy" src="..." style="border-radius:12px;display:block;height:auto;margin:0 0 20px;max-width:100%;width:100%" width="640" height="430"/>`
- intro `<p>` with 1–2 internal links
- `<details class="toc toc-slim"><summary><span>Table of Contents</span></summary><div><ul><li><a href="#id">N. Heading</a></li></ul></div></details>`
- `<div class="key-takeaways"><strong>✨ Key Takeaways at a Glance</strong><ul>…</ul></div>`
- `<h2 id="anchor">` sections, tables in `<div class="vtd-table-wrap">`, `<div class="warning-box">`, FAQ `<details class="faq-item">`
- `<div class="source-box" id="references">` with DOI/NIH/CDC links (`rel="nofollow noopener" target="_blank"`)
- `<div class="medical-disclaimer"><div class="news-box-title">⚠️ Medical Disclaimer</div><p>…</p></div>`
