# Zomato Restaurant Analysis (Revenue & Performance Drivers)

## Business Problem
Zomato operates in a highly competitive restaurant marketplace where performance varies significantly across vendors. The goal of this analysis is to identify the key factors driving restaurant success and revenue concentration, and to determine whether specific characteristics (pricing, ratings, cuisine, or location) meaningfully influence performance outcomes.

---

## Objective
To analyze restaurant-level data and answer:

- Which restaurants generate the most revenue?
- What differentiates high-performing restaurants from lower-performing ones?
- Do pricing structures influence order volume and revenue?
- How do cuisine types impact performance?
- Does location play a measurable role in success?

---

## Data & Methodology

### Data Sources
- `restaurant` table
- `orders` table  
- Joined on: `restaurant.id = orders.r_id`

### Data Preparation
- Aggregated order-level data to calculate:
  - Total Revenue (`sales_amount`)
  - Total Orders (`sales_qty`)
- Standardized categorical fields (cuisine, city)
- Grouped low-frequency categories into “Other” for clarity
- Addressed inconsistencies in categorical data (notably cuisine labeling)

### Tools Used
- Tableau (data visualization & dashboarding)

---

## Analysis & Key Findings

### 1. Revenue Concentration
A small subset of restaurants generates a disproportionately large share of total revenue.

- Domino’s Pizza emerged as a major outlier, producing more than double the revenue of the next highest performer.
- Even within top performers, revenue distribution is highly uneven.

**Insight:**  
The market is not evenly competitive — it is dominated by a small number of high-performing entities.

---

### 2. Ratings vs Revenue
The relationship between ratings and revenue is inconsistent.

- High-performing restaurants often have strong ratings
- However, many lower-performing restaurants also maintain similar rating levels

**Insight:**  
Ratings alone are not a reliable predictor of financial success.

---

### 3. Pricing Structure & Market Behavior
Contrary to expectations, mid-range pricing does not dominate.

- The data reveals a strong pattern of **low-cost, high-volume transactions**
- Revenue is largely driven by frequent, lower-value orders

**Insight:**  
The market is structured around microtransactions, not premium pricing tiers.

---

### 4. Cuisine Performance
Certain cuisines contribute disproportionately to total revenue.

- Indian cuisine categories collectively dominate overall performance
- Unexpectedly, global chains such as Domino’s and Pizza Hut rank among top performers

**Insight:**  
While local cuisine drives aggregate demand, standardized global offerings maintain strong competitive positioning.

---

### 5. Location Impact
Location analysis was limited due to dataset granularity.

- Data was structured at a district level rather than clearly defined cities

**Insight:**  
Location impact remains inconclusive within this dataset and would require more granular geographic data for validation.

---

## Business Implications

- Market success is driven by **volume efficiency**, not premium pricing
- A small number of dominant players capture a large share of revenue
- Cuisine strategy and accessibility matter more than ratings alone
- Expansion strategies should prioritize scalable, high-frequency order models

---

## Limitations

- Lack of data on promotions, seasonality, and competitive landscape
- Inconsistent categorical labeling (especially cuisine)
- Limited geographic granularity (district vs city-level insights)

---

## Conclusion

The Zomato marketplace is defined by a high-volume, low-cost transaction model with strong revenue concentration among top performers. While customer ratings and engagement contribute to success, they are secondary to pricing accessibility and demand-driven consumption patterns.

This analysis highlights the importance of operational scalability and market positioning over traditional quality indicators in determining restaurant performance.

---

## Portfolio Context
This project represents my most advanced analytical work to date, combining data preparation, exploratory analysis, and business insight generation to evaluate real-world marketplace dynamics.
