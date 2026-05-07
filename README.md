# Angel Reese · 24 Stats for 24 Years

A birthday data story celebrating Angel Reese's 24th birthday on May 6, 2026. An interactive D3 ticker that walks through 24 verified career milestones, paired with a Flourish-ready CSV for a season-by-season rebounding chart.

**Live story:** https://theblacktechie.github.io/angel-reese-24/
**By:** [Kris E. Smith](https://twitter.com/theblacktechie) · @theblacktechie

---

## What's Inside

| File | Purpose |
|------|---------|
| `angel-reese-24-stats-ticker.html` | Single-file D3 interactive. 24 stat cards with auto-advance, prev/next/play-pause controls, keyboard navigation, and clickable progress dots. |
| `angel-reese-24-flourish-data.csv` | Six rows of season-by-season rebounding (RPG) data for Flourish. Includes era grouping and a hex color column for the pink gradient. |

---

## The 24 Stats

Narratively ordered across her career arc:

1. Origin (1-3): Birthday, height, jersey number
2. High School (4-7): Saint Frances Academy in Baltimore
3. Maryland (8-10): Foot fracture, sophomore breakout
4. LSU Arrival (11): May 6, 2022 commit on her 20th birthday
5. LSU Junior (12-15): Junior dominance and the 28-rebound game
6. Championship (16-17): 2023 National Championship and Final Four MOP
7. LSU Senior (18-19): Career college totals
8. WNBA Arrival (20): 2024 Draft pick
9. WNBA Dominance (21-23): 446 rebounds, 13.1 RPG, two All-Star selections
10. Atlanta Dream (24): April 6, 2026 trade

---

## Deploying to GitHub Pages

1. Create a new repo (or add to `theblacktechie.github.io`)
2. Drop both files into the repo root or a subfolder
3. Push to `main`
4. Enable GitHub Pages in repo Settings if not already on
5. Direct link to the HTML for sharing on Twitter, Bluesky, Threads

The HTML file is fully self-contained. No build step. D3 and Inter load from CDN.

---

## Flourish Setup

1. Log into Flourish (free plan works fine)
2. Create new visualization
3. Choose **Bar chart** template (not Bar chart race)
4. Click **Data** tab and upload `angel-reese-24-flourish-data.csv`
5. In settings:
   - Set bar color to use the `Color` column for the pink gradient
   - Sort by row order (already chronological)
   - Title: "Angel Reese, Career Rebounds Per Game"
   - Subtitle: "Maryland to LSU to the WNBA, season by season"

---

## Customization

**Colors** are in CSS variables at the top of the HTML:

```
--hot-pink:#FF1493     Primary accent
--bright-pink:#FF6BB5  Light accent
--pop-pink:#FF3D9A     Mid accent
--dream-red:#E03A3E    Atlanta Dream chapter card only
--pink-cream:#FFF8FB   Page background
--black:#1A0B14        Body text
```

**Auto-advance speed** is the `DURATION` constant in the script (default 5000ms).

**Cards** live in the `STATS` array. Edit `big`, `label`, `desc`, or `era` to swap content. Era classes (`era-origin`, `era-maryland`, etc.) control the pill color.

---

## Data Sources

All statistics verified against primary sources:

- **ESPN** Angel Reese records tracker
- **Sports-Reference** (college career line: 116 games, 18.6 PTS, 12.3 TRB)
- **Basketball-Reference** (WNBA totals)
- **Maryland Athletics** (freshman and sophomore season notes)
- **LSU Athletics** (junior and senior season records)
- **WNBA.com** (Sky franchise records, 2024 and 2025 totals)
- **CNN** and **Sports Illustrated** (April 6, 2026 trade announcement)

Statistics current through the 2025 WNBA season.

### Notes on Two Numbers

**446 rookie rebounds.** Reese set the WNBA single-season rebounding record on September 1, 2024, breaking Sylvia Fowles's previous mark of 404. She held it for 16 days before A'ja Wilson surpassed her at 451 while Reese was sidelined with a wrist injury. 446 remains the WNBA rookie single-season record.

**10.6 RPG sophomore at Maryland.** Maryland Athletics' bio page lists 9.1 RPG (likely conference-only), but the publicly cited and mathematically verified full-season figure is 10.6 RPG, which is what the ticker uses.

---

## Credit

Words, concept, design and code by **Kris E. Smith**
@theblacktechie · Atlanta, Georgia · May 6, 2026

Built for fans, for the culture, and for Bayou Barbie.
