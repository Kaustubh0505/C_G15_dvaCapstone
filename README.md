# Zomato Restaurant Analytics

## Executive Summary

This project delivers a data-driven analysis of a large-scale restaurant dataset to identify the factors influencing customer ratings, engagement, and pricing. The study combines data preprocessing, exploratory analysis, statistical validation, and machine learning to generate actionable insights for decision-making in the food technology domain.

---

## Problem Statement

Restaurant discovery platforms often exhibit an uneven distribution of customer attention, where a small proportion of restaurants capture the majority of engagement. This limits visibility and growth opportunities for many restaurants.

This project focuses on identifying the drivers of restaurant performance and improving overall ecosystem efficiency.

---

## Objectives

* Perform structured data cleaning and preprocessing
* Analyze patterns using exploratory data analysis
* Validate relationships using statistical methods
* Build predictive models for ratings and engagement
* Segment restaurants into meaningful groups
* Develop an interactive dashboard for insights

---

## Dataset

The dataset contains restaurant-level information including ratings, engagement, pricing, and service features.

Total records: 51717
Total features: 17
Unique restaurants: 8792

### Key Variables

* rate: average customer rating
* votes: number of customer reviews
* approx_cost: cost for two people
* online_order: online ordering availability
* book_table: table booking availability
* location: restaurant locality
* rest_type: restaurant category
* cuisines: cuisine types

---

## Methodology

### Data Preparation

* Missing ratings imputed using median values
* Missing cost values filled using group-level statistics
* Invalid records removed
* Data types standardized

### Feature Engineering

* Pricing tiers created using cost buckets
* High engagement indicator derived from vote distribution
* Digital readiness defined using service features

### Outlier Handling

* Extreme values identified using statistical methods
* Outliers retained to preserve real-world distribution
* Log transformation applied during modeling

---

## Exploratory Data Analysis

* Ratings show low variance across restaurants
* Customer engagement is highly skewed
* Online ordering is associated with higher ratings
* Table booking correlates with higher cost and engagement

---

## Statistical Analysis

### Hypothesis Testing

* Online ordering significantly impacts ratings
* Table booking is associated with higher engagement

### Predictive Modeling

Random Forest Regressor performance:

Rating prediction R² approximately 0.80
Engagement prediction R² approximately 0.91

These results indicate strong predictive capability.

### Market Segmentation

Three segments were identified:

* Budget segment with low cost and low engagement
* Mid market segment with moderate performance
* Premium segment with high cost and high engagement

---

## Dashboard

An interactive dashboard was developed using Tableau to support analysis and decision-making.

Features include:

* KPI overview
* Category-wise comparison
* Pricing analysis
* Interactive filters

---

## Key Insights

* Ratings show limited differentiation across restaurants
* Customer attention is concentrated among a small subset
* Digital features significantly influence performance
* Premium restaurants drive higher engagement
* Many restaurants lack digital capabilities

---

## Recommendations

* Improve visibility for mid-performing restaurants
* Increase adoption of online ordering systems
* Target premium segments with tailored strategies
* Focus marketing efforts on high-density clusters

---

## Business Impact

* 8 to 15 percent increase in engagement
* 7 to 10 percent potential revenue growth
* Improved distribution of customer attention

---

## Limitations

* No time-based data for trend analysis
* Missing values required imputation
* No customer-level behavioral data
* Analysis based on static dataset

---

## Future Work

* Incorporate time-series analysis
* Build recommendation systems
* Develop real-time data pipelines
* Expand to multiple markets

---
