# Hotel SEO Prioritization – Test Assignment
Demonstrates data analysis and formula logic for SEO prioritization of hotels.

## Overview
This project demonstrates my approach to prioritizing hotels for SEO optimization. The goal is to help SEO specialists focus on pages that will bring the highest impact in the shortest time.

## Data
- Original dataset provided in `Data` tab (kept intact)
- Analysis performed on copied `Analysis` tab

## Approach
1. **Data Cleaning & Highlighting**
   - Automatically highlighted empty `Review Count` cells (orange)
   - Highlighted invalid characters in `Primary Keyword` (red)

2. **Key Metrics**
   - Counted hotels with `Search Volume > 1000` and `Review Count > 100`
   - Found hotels with highest `Search Volume`, highest `Review Count`, and lowest `SERP Position`

3. **Prioritization Formula**
   - Priority calculated based on **Search Volume** and **SERP Position**
   - Zones:
     - **Top 1–10:** Retention, moderate priority
     - **Positions 11–100:** Efficiency, highest priority
     - **>100:** Long-term, low priority
   - Formulas that were used:
   - Priority = SearchVolume * SERP_weight
   - SERP_weight = IF(P <= 10, 0.5, IF(P <= 100, 1 + (100-P)/90, 0.1))
> **Note:** The prioritization formula was designed independently by me based on the provided business logic.

## Outcome
- Sorted hotels by `Priority` to identify those worth focusing on first
- Priority reflects both potential traffic (Search Volume) and current SERP position

## How to Use
- Open `Analysis` tab in Google Sheets
- Review calculated `Priority` column
- Use conditional formatting and metrics to guide SEO decisions

## Key Takeaways
- Demonstrates analytical thinking and Excel/Sheets skills
- Shows ability to translate business logic into actionable formulas
