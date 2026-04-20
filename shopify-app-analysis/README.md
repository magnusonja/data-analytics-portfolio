# Shopify App Analysis (Power BI)

## Overview
This project analyzes the Shopify App Marketplace using public app, category, and review data. The goal is to understand what drives app success by evaluating engagement, ratings, developer responsiveness, and category distribution.

The analysis was built in Power BI with multiple dashboards designed to translate raw marketplace data into actionable business insights.

---

## Business Objective
Identify the key factors that influence Shopify app performance, including:
- App adoption and engagement trends
- Relationship between ratings and review volume
- Impact of developer responsiveness on user ratings
- Category-level performance differences

---

## Data Sources
The dataset consists of four related tables:

- **apps**: Core app metadata
- **apps_categories**: Mapping of apps to categories
- **categories**: Category definitions
- **reviews**: User reviews and developer responses

Relationships were built between:
- `apps.id → reviews.app_id`
- `apps.id → apps_categories.app_id`
- `categories.id → apps_categories.category_id`

---

## Key Analyses

### 1. App Landscape
- Total number of apps in the marketplace
- Review volume trends over time
- Relationship between review count and average rating

Insight:
Apps with higher review counts tend to show more stable rating distributions, indicating maturity and sustained usage.

---

### 2. Reviews Analysis
- Created weighted review metric:
  `helpful_reviews = rating * (1 + helpful_count)`
- Measured impact of developer responses on ratings
- Compared apps with and without developer engagement

Insight:
Developer engagement shows measurable correlation with improved review quality and perceived app value.

---

### 3. App Performance by Developer
- Aggregated rating performance by developer
- Adjusted for review volume bias
- Compared average rating vs weighted helpful reviews

Insight:
Raw rating totals are misleading without normalization for review volume and engagement.

---

## Tools Used
- Power BI
- DAX (calculated columns and measures)
- Data modeling (relationships across tables)
- Data visualization (bar charts, scatterplots, KPI cards, line charts)

---

## Key Takeaways
- Engagement metrics are more informative than raw ratings
- Developer responsiveness correlates with better perceived app quality
- Category distribution helps explain performance clustering in the marketplace
- Normalized metrics are critical for fair comparison across apps

---

## Portfolio Context
This project represents my applied Power BI work focused on:
- Data modeling
- Business KPI design
- Product analytics interpretation
- Visualization-driven insight generation
