# Zomato Restaurant Analytics

## Executive Summary

This project analyzes a large restaurant dataset to understand what affects customer ratings, engagement, and pricing. It uses data cleaning, analysis, statistics, and machine learning to generate useful insights for better decision-making in the food industry.

---

## Problem Statement

On restaurant platforms, only a few restaurants get most of the attention from customers. This makes it hard for many other restaurants to grow and be noticed.

This project aims to find the key factors that affect restaurant performance and improve overall platform efficiency.

---

## Objectives

- Clean and prepare the data properly  
- Study patterns using exploratory data analysis  
- Test relationships using statistical methods  
- Build models to predict ratings and engagement  
- Group restaurants into meaningful segments  
- Create an interactive dashboard for insights  

---

## Dataset

The dataset includes information about restaurants such as ratings, engagement, pricing, and services.

- **Total records:** 51717  
- **Total features:** 17  
- **Unique restaurants:** 8792  

### Key Variables

- **rate:** average customer rating  
- **votes:** number of reviews  
- **approx_cost:** cost for two people  
- **online_order:** whether online ordering is available  
- **book_table:** whether table booking is available  
- **location:** restaurant area  
- **rest_type:** type of restaurant  
- **cuisines:** types of food offered  

---

## Methodology

### Data Preparation

- Missing ratings filled using median values  
- Missing cost values filled using group averages  
- Incorrect records removed  
- Data formats standardized  

### Feature Engineering

- Created pricing groups based on cost  
- Defined high engagement using vote distribution  
- Defined digital readiness based on services  

### Outlier Handling

- Extreme values identified using statistical methods  
- Outliers kept to maintain real-world data  
- Log transformation used during modeling  

---

## Exploratory Data Analysis

- Ratings do not vary much across restaurants  
- Customer engagement is uneven (skewed)  
- Online ordering is linked to higher ratings  
- Table booking is linked to higher cost and engagement  

---

## Statistical Analysis

### Hypothesis Testing

- Online ordering has a significant effect on ratings  
- Table booking is linked to higher engagement  


---

## Market Segmentation

Three groups of restaurants were identified:

- **Budget:** low cost, low engagement  
- **Mid-market:** moderate performance  
- **Premium:** high cost, high engagement  

---

## Dashboard

An interactive dashboard was created using Tableau.

### Features

- Key performance indicators (KPIs)  
- Category comparisons  
- Pricing analysis  
- Interactive filters  

---

## Key Insights

- Ratings are very similar across most restaurants  
- Most customer attention goes to a few restaurants  
- Digital features improve performance  
- Premium restaurants get higher engagement  
- Many restaurants are not using digital features  

---

## Recommendations

- Help mid-level restaurants get more visibility  
- Encourage use of online ordering  
- Focus strategies on premium segments  
- Target marketing in high-demand areas  

---

## Business Impact

- 8 to 15 percent increase in engagement  
- 7 to 10 percent possible revenue growth  
- Better distribution of customer attention  

---

## Limitations

- No time-based data for trend analysis  
- Missing values were estimated  
- No customer-level behavior data  
- Based on static dataset only  

---

## Future Work

- Add time-based analysis  
- Build recommendation systems  
- Create real-time data pipelines  
- Expand analysis to more markets  
