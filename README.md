# NST DVA Capstone 2 - Zomato Restaurant Analytics

## Project Overview

| Field | Details |
|---|---|
| **Project Title** | Zomato Restaurant Analytics |
| **Sector** | Food & Beverage / Restaurant Industry |
| **Team ID** | C_G15 |
| **Section** | C |
| **Faculty Mentor** | Satyaki Sir |
| **Institute** | Newton School of Technology |
| **Submission Date** | 28-04-2026 |

--- 

### Team Members

| Role | Name | GitHub |
|---|---|---|
| Project Lead | Kaustubh Hiwanj | [GitHub](https://github.com/kaustubh0505) |
| Data Lead | Nistha Gupta | [GitHub](https://github.com/nishtha-09-gupta) |
| Visualization Lead | Adil Mirza | [GitHub](https://github.com/adilmirza975) |
| Analysis Lead | Krishiv Gupta | [GitHub](https://github.com/krishiv274) |
| ETL Lead | Kaustubh Hiwanj | [GitHub](https://github.com/kaustubh0505) |
| Strategy Lead | Nishta Gupta | [GitHub](https://github.com/nishtha-09-gupta) |
| PPT | Tejas Tyagi | [GitHub](https://github.com/Tejas10108) |
| Project Report | Tanish Yadav | [GitHub](https://github.com/tanishrao13) |

---

## Business Problem

On restaurant platforms like Zomato, only a few restaurants capture most of the customer attention, making it challenging for mid-level and new restaurants to grow and get noticed. This project analyzes a comprehensive dataset to understand the key drivers of customer ratings, engagement, and pricing. The insights aim to guide strategies for better visibility and optimize platform efficiency in the highly competitive food industry.

**Core Business Question**

> Which types of restaurants (based on location, cuisine, and cost) achieve higher ratings and customer engagement (votes), and how does this vary across locations?

**Decision Supported**

> Help restaurant owners optimize pricing, adopt digital features (online ordering & table booking), and enable platforms to improve visibility distribution across restaurant segments.

---

## Dataset

| Attribute | Details |
|---|---|
| **Source Name** | Zomato Bangalore Restaurants Dataset |
| **Direct Access Link** | [Data Link](https://www.kaggle.com/datasets/rajeshrampure/zomato-dataset) |
| **Row Count** | 51,717 |
| **Column Count** | 17 (including engineered features) |
| **Time Period Covered** | Not explicitly available (cross-sectional dataset) |
| **Format** | CSV |

---

## KPI Framework

| KPI | Definition | Formula / Computation |
|---|---|---|
| Average Rating | Overall customer satisfaction level | Mean of `rate` |
| Total Engagement | Customer interaction and popularity | Sum of `votes` |
| Average Cost for Two | Pricing level indicator | Mean of `approx_cost` |
| Digital Readiness | Adoption of platform features | `online_order` + `book_table` |

**Actual KPI Values:**

- Average Rating: **3.70**
- Total Votes: **14.67M**
- Average Cost for Two: **₹554.4**
- Total Restaurants: **8,792**

---

## Tableau Dashboard

| Item | Details |
|---|---|
| **Dashboard URL** | [Tableau Public Link](https://public.tableau.com/views/Book1_17772634695820/HOME?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) |
| **Executive View** | Displays KPIs like average rating, total votes, cost distribution, and top restaurant locations |
| **Operational View** | Includes cuisine-level analysis, pricing vs ratings scatter plot, and location-based heatmaps |
| **Main Filters** | Location, cuisine, restaurant type, pricing, online ordering, table booking |

### Dashboard Highlights

- **Top Locations:** Whitefield, BTM, Electronic City, HSR, Marathahalli  
- **Top Restaurant Types:** Microbreweries, Fine Dining, Pubs  
- **Online Ordering:** ~59% restaurants offer it  
- **Pricing vs Ratings:** No strong linear relationship observed  
- **Cuisine Trends:** Ratings mostly fall between 3.6–4.1 across locations  

---

## Key Insights

1. **Rating Uniformity:** Ratings are tightly clustered around ~3.7 across most restaurants.  
2. **Skewed Engagement:** A small number of restaurants capture a large share of total votes.  
3. **Premium Pricing ≠ Better Ratings:** Higher cost does not guarantee higher ratings.  
4. **Digital Impact:** Online ordering influences both engagement and pricing patterns.  
5. **Location Concentration:** Areas like Whitefield and BTM dominate restaurant density.  
6. **Moderate Correlations:**  
   - Rating vs Votes ≈ 0.43  
   - Table Booking vs Cost ≈ 0.62  
7. **Market Segmentation:** Restaurants fall into Budget, Mid-market, and Premium segments.  

---

## Recommendations

| # | Insight | Recommendation | Expected Impact |
|---|---|---|---|
| 1 | Skewed Engagement | Promote mid-tier restaurants using recommendation systems and visibility boosts | Better distribution of customer traffic |
| 2 | Digital Edge | Encourage adoption of online ordering for underperforming restaurants | ~10% increase in engagement and orders |
| 3 | Premium Segments | Target premium restaurants with loyalty programs and curated experiences | Higher revenue per customer |

---

## Impact

- **8–15% increase in engagement**
- **7–10% potential revenue growth**
- Improved platform efficiency and restaurant visibility balance  


---


## Repository Structure

```text
C_G15_dvaCapstone/
|
|-- README.md
|
|-- data/
|   |-- raw/
|   `-- processed/
|
|-- notebooks/
|   |-- 01_extraction.ipynb
|   |-- 02_cleaning.ipynb
|   |-- 03_eda.ipynb
|   |-- 04_statistical_analysis.ipynb
|   `-- 05_final_load_prep.ipynb
|
|-- scripts/
|   `-- etl_pipeline.py
|
|-- tableau/
|   |-- screenshots/
|   `-- dashboard_links.md
|
|-- reports/
|   |-- project_report_template.md
|   `-- presentation_outline.md
|
|-- docs/
|   `-- data_dictionary.md
|
|-- DVA-oriented-Resume/
`-- DVA-focused-Portfolio/