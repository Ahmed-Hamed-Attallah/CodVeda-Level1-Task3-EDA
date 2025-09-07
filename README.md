# 🛒 Supermarket Sales Performance - Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-lightgrey)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📖 Project Overview

This project involves a comprehensive **Exploratory Data Analysis (EDA)** of a supermarket's historical sales transaction data. The goal is to uncover hidden patterns, identify key performance indicators, derive actionable insights, and provide data-driven recommendations to optimize business strategy, marketing efforts, and operational efficiency.

The dataset contains nearly 10,000 transactions recorded between 2015 and 2018, including details on orders, customers, products, and sales figures.

## 📊 Dataset

- **Source:** [Kaggle - Supermarket Dataset for Exploratory Data Analysis](https://www.kaggle.com/datasets/moro146/supermarket-eda)
- **File:** `supermarket.csv`
- **Original Size:** 9,800 rows × 18 columns
- **Cleaned Size:** 9,789 rows × 18 columns (after handling missing values)
- **Description:** The dataset contains transaction records with information on:
  - **Order Details:** Order ID, Date, Ship Date, Ship Mode.
  - **Customer Info:** Customer ID, Name, Segment, Geographic Location (Country, City, State, Postal Code, Region).
  - **Product Info:** Product ID, Category, Sub-Category, Product Name.
  - **Sales:** Sales amount per transaction.

## 🛠️ Tech Stack & Libraries

- **Programming Language:** Python 3
- **Data Manipulation:** `pandas`, `numpy`
- **Data Visualization:** `matplotlib`, `seaborn`, `plotly`
- **Outlier Detection:** `datasist`
- **Correlation Analysis:** `dython`
- **Environment:** Jupyter Notebook / Google Colab

## 🔍 EDA Workflow

The analysis was conducted in a structured, phased approach:

1.  **Data Understanding & Loading:** Initial inspection of the dataset structure, data types, and summary statistics.
2.  **Data Cleaning:**
    - Handled missing values in the `Postal Code` column.
    - Converted `Order Date` and `Ship Date` to proper datetime objects.
3.  **Feature Engineering:** Created new time-based features (`Order-year`, `Order-Month`, `Ship-Year`, `Ship-Month`) for trend analysis.
4.  **Univariate Analysis:** Analyzed the distribution of individual variables (both numerical and categorical).
    - Numerical: Sales distribution
    - Categorical: Ship Mode, Customer Segment, Geographic distribution, Product Categories.
5.  **Outlier Analysis:** Detected and investigated outliers in the `Sales` column. Concluded they were legitimate business transactions and decided to retain them.
6.  **Multivariate Analysis:** Explored relationships between variables.
    - Sales by Segment and Region.
    - Sales by Category and Ship Mode.
    - Correlation Heatmap for numerical features.
    - Time Series Analysis of monthly sales trends.
7.  **Insights & Recommendations:** Synthesized findings into actionable business strategies.

## 📈 Key Insights

1.  **Dominant Customer Segment:** The **Consumer** segment is the largest and most profitable, contributing the highest sales across all regions, especially in the **West** and **East**.
2.  **Top Product Category:** The **Technology** category generates the highest total revenue, despite **Office Supplies** having the highest order frequency.
3.  **Shipping Strategy:** **Same Day** shipping, though less common, is associated with high-value transactions, particularly in the Technology category.
4.  **Clear Seasonality:** Sales exhibit strong and predictable peaks during the **November-December** holiday season every year.
5.  **Regional Disparity:** The **South** and **Central** regions underperform compared to the West and East, indicating a significant growth opportunity.
6.  **Temporal Correlation:** Strong correlation between order and ship dates confirms the influence of time-based trends on sales.

## 💡 Business Recommendations

| Area | Recommendation |
| :--- | :--- |
| **Marketing** | Launch targeted campaigns and loyalty programs for the **Consumer segment** in the **West and East regions**. |
| **Inventory** | Prioritize stock and invest in marketing for the high-revenue **Technology** category. |
| **Logistics** | Promote and potentially subsidize **Same Day shipping** for high-value orders to boost sales. |
| **Regional Strategy** | Implement targeted promotions and improve supply chain efficiency in the underperforming **South** and **Central** regions. |
| **Planning** | Use seasonal trends to forecast demand; begin stockpiling and marketing for the **Q4 holiday season** early. |



