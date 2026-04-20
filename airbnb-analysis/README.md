# Airbnb Market Analysis (New York City)

## Overview
This project analyzes Airbnb listings in New York City to identify which neighborhoods and property sizes generate the highest rental activity and revenue potential. The goal is to provide investment guidance for short-term rental decision-making based on demand signals in the market.

The analysis was conducted using Excel/Google Sheets with pivot tables and structured data cleaning.

---

## Business Objective
The objective of this analysis is to determine:
- Which neighborhoods show the highest rental demand
- Which property sizes (number of bedrooms) are most attractive to guests
- How revenue potential varies across listings
- How demand patterns differ across NYC neighborhoods

---

## Data Source
The dataset contains Airbnb listings for New York City, including:
- Neighborhood location data
- Property characteristics (bedrooms, listing type)
- Booking activity proxy via **number_of_reviews_ltm**
- Pricing and calendar-based revenue estimates

---

## Data Preparation
Key cleaning and transformation steps included:

- Standardizing neighborhood names (removed inconsistencies and whitespace)
- Creating `neighborhood_clean` field for analysis
- Cleaning bedroom data and replacing missing values with 0 (studio classification)
- Creating `bedrooms_clean` field for consistent grouping
- Building pivot tables to aggregate demand by neighborhood and property size
- Estimating revenue using calendar availability and adjusted price data

---

## Key Analyses

### 1. Neighborhood Demand Analysis
Demand was measured using **number_of_reviews_ltm** as a proxy for booking frequency.

Top performing neighborhoods included:
- Lower East Side
- Hell’s Kitchen
- Harlem

Insight:
Demand is heavily concentrated in a small subset of neighborhoods, indicating strong location-based clustering in short-term rental activity.

---

### 2. Property Size Demand
Analysis of bedroom distribution showed:

- Studios
- 1-bedroom units
- 2-bedroom units

Insight:
1-bedroom and studio units dominate demand across most high-performing neighborhoods, indicating strong preference for affordability and flexibility in NYC short-term rentals.

---

### 3. Neighborhood vs Property Size Preferences
Cross-analysis showed that different neighborhoods exhibit distinct property size preferences.

Insight:
Most high-demand neighborhoods converge on 1-bedroom listings as the optimal investment unit type.

---

### 4. Revenue Estimation
Revenue was estimated using calendar availability and adjusted pricing, then annualized.

Insight:
Top-performing listings generate disproportionately high revenue relative to the broader market, reinforcing the concentration of returns in specific properties and locations.

---

## Tools Used
- Excel / Google Sheets
- Pivot Tables
- Data Cleaning (text normalization, missing value handling)
- Basic revenue modeling
- Data aggregation and segmentation

---

## Key Takeaways
- NYC Airbnb demand is highly concentrated geographically
- 1-bedroom units are the most consistently optimal property size
- A small number of listings generate a disproportionate share of revenue
- Neighborhood selection is a stronger driver than property variation alone

---

## Portfolio Context
This project represents foundational analytical work focused on:
- Market segmentation
- Demand estimation using proxy metrics
- Revenue modeling
- Early-stage investment analysis using structured datasets
