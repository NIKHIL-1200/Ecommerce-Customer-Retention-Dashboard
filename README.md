# Ecommerce-Customer-Retention-Dashboard
An advanced Power BI dashboard analyzing customer cohorts, behavior funnels, and churn metrics using multi-category e-commerce web logs.


## Project Overview
An advanced, multi-page Power BI portfolio project focused on deep-dive behavioral analysis, conversion funnels, and customer retention mechanics. Utilizing an e-commerce web logs dataset containing millions of behavioral records, this dashboard models user paths from discovery to conversion while tracking weekly customer cohort survival rates.



## Dataset Source
Data sourced from the Kaggle dataset: [eCommerce behavior data from multi-category store](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store).

## Key Features & Insights
* **Interactive Data Model:** Engineered a custom, highly optimized Calendar dimension table to resolve high-volume datetime granular mismatches and implement clean relationships.
* **E-Commerce Conversion Funnel:** Visualizes the full customer lifecycle (`View` -> `Cart` -> `Purchase`) to pinpoint user drop-off intervals.
* **Advanced Cohort Matrix:** Uses memory-optimized DAX calculations to construct a dynamic user retention heatmap over rolling weekly horizons without resource performance degradation.

## Tech Stack & Skills
* **BI Tool:** Power BI Desktop
* **Data Transformation:** Power Query (ETL, schema optimization, custom column segmentation)
* **Modeling & Metrics:** DAX (Data Analysis Expressions) for time-intelligence, filtering override contexts, and unique customer clustering

## Dashboard Previews
### 1. Performance & Conversion Overview
![Overview Dashboard](./Screenshots/01_Overview_Dashboard.png)

### 2. Customer Cohort Retention Analysis
![Cohort Analysis Heatmap](./Screenshots/02_Cohort_Analysis_Dashboard.png)
