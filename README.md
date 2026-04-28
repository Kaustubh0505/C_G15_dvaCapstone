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
| Data Lead | _Name_ | `[link]` |
| Visualization Lead | _Name_ | `[link]` |
| Analysis Lead | _Name_ | `[link]` |
| ETL Lead | _Name_ | `[link]` |
| Strategy Lead | _Name_ | `[link]` |
| PPT and Quality Lead | _Name_ | `[link]` |

---

## Business Problem

On restaurant platforms like Zomato, only a few restaurants capture most of the customer attention, making it challenging for mid-level and new restaurants to grow and get noticed. This project analyzes a comprehensive dataset to understand the key drivers of customer ratings, engagement, and pricing. The insights aim to guide strategies for better visibility and optimize platform efficiency in the highly competitive food industry.

**Core Business Question**

> What are the primary factors that influence restaurant ratings and customer engagement on the Zomato platform?

**Decision Supported**

> Enable restaurants to decide on adopting digital features (like online ordering and table booking) and help platform managers develop strategies to redistribute visibility towards mid-market restaurants.

---

## Dataset

| Attribute | Details |
|---|---|
| **Source Name** | Zomato |
| **Direct Access Link** | (https://www.kaggle.com/datasets/rajeshrampure/zomato-dataset) |
| **Row Count** | 51,717 |
| **Column Count** | 17 |
| **Time Period Covered** | _To be filled by team_ |
| **Format** | CSV |

**Key Columns Used**

| Column Name | Description | Role in Analysis |
|---|---|---|
| `rate` | Average customer rating | Key KPI / Target Variable |
| `votes` | Number of customer reviews | Used for Engagement KPI |
| `approx_cost` | Cost for two people | Used for Pricing Segmentation |
| `online_order` | Whether online ordering is available | Used for Digital Readiness Analysis |
| `book_table` | Whether table booking is available | Used for Digital Readiness Analysis |
| `location` | Restaurant area | Used for Geographic Segmentation |
| `rest_type` | Type of restaurant | Used for Categorization |
| `cuisines` | Types of food offered | Used for Variety Analysis |

For full column definitions, see [`docs/data_dictionary.md`](docs/data_dictionary.md).

---

## KPI Framework

| KPI | Definition | Formula / Computation |
|---|---|---|
| Average Rating | The mean customer rating for a restaurant | Mean of `rate` column |
| Total Engagement | The level of customer interaction | Sum of `votes` |
| Average Cost for Two | Expected spend for two people | Mean of `approx_cost` |
| Digital Readiness | Availability of digital services | Presence of `online_order` and `book_table` |

Document KPI logic clearly in `notebooks/04_statistical_analysis.ipynb` and `notebooks/05_final_load_prep.ipynb`.

---

## Tableau Dashboard

| Item | Details |
|---|---|
| **Dashboard URL** | [Tableau Public Link](https://public.tableau.com/views/Book1_17772634695820/HOME?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) |
| **Executive View** | High-level summary of KPIs, overall ratings, and engagement distributions |
| **Operational View** | Detailed breakdown of restaurants by location, category comparisons, and pricing analysis |
| **Main Filters** | Interactive filters for location, cost, restaurant type, and digital features |

Store dashboard screenshots in [`tableau/screenshots/`](tableau/screenshots/) and document the public links in [`tableau/dashboard_links.md`](tableau/dashboard_links.md).

---

## Key Insights

1. **Rating Uniformity:** Ratings do not vary significantly across most restaurants.
2. **Skewed Engagement:** Customer engagement is highly uneven, with most attention going to a few top restaurants.
3. **Digital Edge:** Offering online ordering is strongly linked to higher ratings.
4. **Premium Features:** Table booking availability is associated with higher costs and greater engagement.
5. **Market Segments:** The market is divided into Budget (low cost/engagement), Mid-market (moderate performance), and Premium (high cost/engagement).
6. **Feature Underutilization:** Many restaurants are currently not utilizing digital features to their full potential.
7. **Premium Performance:** Premium segment restaurants generally receive disproportionately higher engagement.
8. **Cost vs Engagement:** Higher `approx_cost` often correlates with services like table booking, which in turn drive higher customer votes.

---

## Recommendations

| # | Insight | Recommendation | Expected Impact |
|---|---|---|---|
| 1 | Skewed Engagement | Implement platform strategies to help mid-level restaurants get more visibility | Better distribution of customer attention across the platform |
| 2 | Digital Edge | Actively encourage restaurants to adopt online ordering | 8 to 15 percent increase in customer engagement |
| 3 | Feature Underutilization & Premium Focus | Focus marketing and sales strategies on premium segments and high-demand areas | 7 to 10 percent possible revenue growth |

---

## Repository Structure

```text
C_G15_dvaCapstone/
|
|-- README.md
|
|-- data/
|   |-- raw/                         # Original dataset (never edited)
|   `-- processed/                   # Cleaned output from ETL pipeline
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
```

---


## Tech Stack

| Tool | Status | Purpose |
|---|---|---|
| Python + Jupyter Notebooks | Mandatory | ETL, cleaning, analysis, and KPI computation |
| Google Colab | Supported | Cloud notebook execution environment |
| Tableau Public | Mandatory | Dashboard design, publishing, and sharing |
| GitHub | Mandatory | Version control, collaboration, contribution audit |

---

**Presentation Deck**

- [ ] Final presentation exported as PDF into `reports/`
- [ ] Title slide through recommendations, impact, limitations, and next steps

**Individual Assets**

- [ ] DVA-oriented resume updated to include this capstone
- [ ] Portfolio link or project case study added

---