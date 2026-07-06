# E-Commerce Customer Retention & Cohort Analysis Dashboard

## 📊 Project Overview
An advanced, multi-page Power BI portfolio project focused on deep-dive behavioral analysis, conversion funnels, and customer retention mechanics. Utilizing a high-volume e-commerce web logs dataset containing millions of raw behavioral records, this dashboard models user paths from initial item discovery to checkout while tracking weekly customer cohort survival rates.

Rather than basic historical reporting, this project addresses complex data orchestration challenges—such as handling mismatched datetime grains, optimizing heavy data models locally, and writing memory-efficient DAX formulas to prevent resource limits.

---

## 🛠️ Tech Stack & Technical Skills

| Phase | Tools Used | Key Concepts Applied |
| :--- | :--- | :--- |
| **ETL & Data Prep** | Power Query | Schema optimization, column parsing, data type casting, string manipulation |
| **Data Modeling** | Power BI Engine | Custom Star Schema design, dimension table building, 1-to-Many ($1 \rightarrow *$) relationships |
| **Analytical Calculations** | Advanced DAX | Iteration overrides, filter context filtering (`REMOVEFILTERS`), dynamic ratio calculations |
| **UI/UX Design** | Power BI Canvas | Widescreen 16:9 canvas scaling, conditional formatting heatmaps, structured KPI banners |

---

## 💡 Key Features & Architectural Insights
* **Interactive Star Schema Data Model:** Engineered a custom, highly optimized Calendar dimension table to resolve high-volume datetime granular mismatches, establishing clean links to raw transactional event logs.
* **E-Commerce Conversion Funnel:** Visualizes the full customer conversion lifecycle (`View` $\rightarrow$ `Cart` $\rightarrow$ `Purchase`) to isolate precise customer drop-off intervals across millions of interactions.
* **Memory-Optimized Cohort Matrix:** Implemented a streamlined DAX logic system utilizing context overrides to construct a dynamic user retention heatmap over rolling weekly horizons, entirely bypassing standard hardware local RAM bottlenecks.

---

## 🖼️ Dashboard Previews

### 1. Performance & Conversion Overview
![Overview Dashboard](./Screenshots/01_Overview_Dashboard.png)

### 2. Customer Cohort Retention Analysis
![Cohort Analysis Heatmap](./Screenshots/02_Cohort_Analysis_Dashboard.png)

---

## ⚙️ How to Replicate & Open This Project
Due to GitHub's standard 100 MB file limit per asset, the raw data rows have been stripped from the repository file structure to keep the codebase lightweight. 

To open and interact with the full model on your local computer:
1. Download the tiny **`Ecommerce_Customer_Retention_Dashboard.pbit`** template file from this repository.
2. Download the original source `2019-Nov.csv` dataset directly from [Kaggle: eCommerce behavior data from multi-category store](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store).
3. Open the downloaded `.pbit` file in Power BI Desktop.
4. When prompted by Power BI, change the data source pathway folder pointer to match the directory of your locally saved Kaggle CSV file. Click **Refresh** to automatically process the data and re-populate the visual components.
