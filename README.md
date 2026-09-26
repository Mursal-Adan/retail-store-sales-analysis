# Retail Store Sales Analysis

## Business Problem
A retail store wants to understand sales performance across product categories, payment methods, and locations, and assess the effect of discounts on revenue — using Excel for cleaning and analysis, and Tableau for visualization.

## Dataset
**Retail Store Sales: Dirty for Data Cleaning** — 12,575 transactions, 8 product categories (25 items each), Jan 2022 – Jan 2025.
Source: [Kaggle](https://www.kaggle.com/datasets/ahmedmohamed2003/retail-store-sales-dirty-for-data-cleaning)

## Tools
Excel (cleaning, analysis) · Tableau (visualization)

## Dashboard
🔗 [View live dashboard on Tableau Public](https://public.tableau.com/shared/JKG6DD9BQ?:display_count=n&:origin=viz_share_link)

## Process
1. **Investigation** — checked row counts, blanks, duplicates, and value consistency across all columns.
2. **Cleaning** — recovered 609 missing prices (Total Spent ÷ Quantity), recovered 1,213 missing items (Category + Price lookup, 100% match rate), flagged 604 unrecoverable rows (missing both Quantity and Total Spent), labeled 4,199 missing discount values "Unknown" instead of assuming false.
3. **Analysis** — answered 4 business questions using pivot tables: revenue by category, discount effect on spend, payment method/location preference, and revenue trend over time.
4. **Visualization** — built a 5-chart Tableau dashboard.

## Key Findings & Recommendations

**1. Revenue by Category**
All 8 categories generate similar revenue (180K–208K, ~13% spread) — no single category dominates.
→ Spread inventory investment proportionally across categories rather than concentrating on a "top performer."

**2. Discount Effect**
Average transaction value is nearly identical whether discounted (130.49), not discounted (129.95), or unknown (128.51).
→ Discounts show no measurable lift in transaction size — investigate whether current discounting is targeted and cost-effective.

**3. Payment Method & Location**
No preference exists — all payment methods and locations are within 2-4% of each other.
→ No urgent gap to fix; resources are better focused elsewhere.

**4. Revenue Over Time (2022-2024)**
Revenue is flat across all 3 full years (~510K-525K/year), no growth, decline, or clear seasonality.
→ Growth likely requires a new lever (marketing, new products, expanded reach) rather than expecting organic increase.

## Files
- `retail_store_sales.xlsx` — raw and cleaned data (separate sheets)
- Tableau dashboard: see link above

## Limitations
- 604 rows (4.8%) have unrecoverable missing Quantity/Total Spent — excluded from revenue-specific totals, retained for category/payment/location analysis
- 33% of Discount Applied values were missing and labeled "Unknown" rather than assumed — avoiding fabricated conclusions
