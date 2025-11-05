# 🛍️ Digikala Data Analysis (Sales, Discounts & Category Insights)

This project focuses on **analyzing product and sales data from Digikala**, one of the largest e-commerce platforms in Iran.
The analysis explores how **discounts, product categories, user ratings, and sales** relate to each other across different months and years.

---

## 📊 Project Overview

The dataset was sourced from a Kaggle Digikala dataset.
After cleaning and preprocessing, I focused on several key features, including:

* **Product categories**
* **Number of items sold**
* **User ratings**
* **Applied discounts**
* **Monthly sales comparisons** between **1402** and **1403 (2023–2024)**

---

## 🧹 Data Cleaning & Preprocessing

* Removed missing and inconsistent records
* Selected relevant columns for analysis
* Extracted and converted **dates** to **Jalali (Persian) calendar** using the `jalali` library
* Standardized numeric fields (e.g., discounts, prices, ratings)
* Created grouped summaries by **category** and **month**

---

## 🔬 Exploratory Analysis

The following relationships were analyzed:

* Sales counts by **product categories and brands**
* Relationship between **discount percentage** and **user ratings**
* Comparison of total sales between **this year and last year**
* Statistical significance of price differences between categories using **ANOVA**

### 🔹 ANOVA Results

| Metric               | Result                                                                                                                      |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **Valid Categories** | ['ابزار آلات و تجهیزات', 'خانه و آشپزخانه', 'خودرو و موتورسیکلت', 'مد و پوشاک', 'کالای دیجیتال', 'کتاب، لوازم تحریر و هنر'] |
| **F-stat**           | 19.5437                                                                                                                     |
| **p-value**          | 1.81e-19                                                                                                                    |

✅ **Interpretation:** The p-value (< 0.05) indicates that the differences in average prices between product categories are **statistically significant**.

---

## 📈 Correlation Analysis

The correlation coefficient between **discount percentage** and **user rating** was:

> **r = 0.107**

This suggests a **weak positive relationship** — meaning higher discounts are *slightly* associated with higher user ratings, possibly due to increased customer satisfaction during promotions.

---

## 🖼️ Visualizations

### 🟢 Sales Comparison: 1402 vs 1403

**(Insert your first chart here)**

![Sales Comparison](images/sales_comparison_1402_1403.png)

---

### 🟣 Discount vs. Sales Count

**(Insert your second chart here)**

This visualization shows that **most user ratings cluster within the 70–80% discount range**, indicating customers respond strongly to major discounts.

![Discount vs Sales](images/discount_vs_sales.png)

---

## 🧠 Libraries Used

* **pandas**, **numpy** → data cleaning & manipulation
* **matplotlib**, **seaborn** → visualization
* **scipy.stats**, **statsmodels** → statistical analysis (ANOVA, correlation)
* **scikit-learn** → scaling & preprocessing
* **persiantools**, **bidi**, **arabic_reshaper** → Persian text handling and date formatting

---

## 📚 Key Takeaways

* There are **significant price differences** across product categories.
* Sales performance and discount levels show **seasonal and annual variation**.
* Discounts of **70–80%** receive the **highest engagement and user ratings**.
* The market displays distinct “luxury” vs. “mid-range” category patterns.

---

## 🚀 Future Work

* Predictive modeling for **sales forecasting**
* Deeper time series analysis for **monthly trends**
* Brand-level comparison and rating distribution studies
* Interactive dashboard for visual exploration

---

**Author:** Sarina Aghamohammad Kashi
**Dataset:** [Kaggle - Digikala Dataset](https://www.kaggle.com)
**Language:** Python
**Year:** 1404 / 2025
