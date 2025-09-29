# Capstone Project – AWS SaaS Sales Analysis

**Course:** Purwadhika Data Science (Online) – Module 2

---

## 📌 Project Overview

In today’s competitive SaaS landscape, **profitable growth matters more than revenue growth alone**.
This project analyzes the **AWS SaaS Sales dataset** at the order level to uncover **where the business is winning profitably, where it is losing money, and which levers (discounts, regions, segments) most impact results**.

The work is part of a capstone project for the Purwadhika Data Science program and is delivered in three formats:

1. **Jupyter Notebook** – documented code, analysis, and statistical validation.
2. **Tableau Dashboard** – interactive visualizations for stakeholders.
3. **Presentation Deck** – concise executive summary with insights and recommendations.

---

## 🎯 Business Questions

1. **Performance over time** – Are Sales and Profit moving together, or are we growing revenue at the expense of margin?
2. **Where to focus** – Which regions, industries, products, and customers drive profit (or destroy value)?
3. **Discount effectiveness** – Are discounts healthy volume drivers, or do they systematically erode margins?
4. **Customer & segment strategy** – How do SMB, Enterprise, and Strategic segments differ in profitability?

---

## 🛠️ Project Workflow

### 1. Data Preparation

* Inspected data shape, types, and anomalies (missing values, duplicates).
* Cleaned data: standardized formats, parsed dates, ensured numeric consistency.
* Flagged anomalies (negative profits, out-of-range discounts) without dropping signals.

### 2. Feature Engineering

* Created **Margin** (Profit/Sales), **Price per Unit**, and time fields (Year, Quarter, Month).
* Added discount flags and bands (0%, 0–20%, 20–50%, 50–100%).

### 3. Descriptive Analytics

* Explored sales/profit distributions by Region, Segment, and Product.
* Highlighted concentration: a few products/customers drive most profit, while some create losses.

### 4. Visualization (Python + Tableau)

* **Trends:** Sales vs. Profit over time → margin compression in certain quarters.
* **Regional:** EMEA/AMER profitable; APJ drags (notably Japan & ANZ).
* **Segment:** Enterprise customers show higher margins than SMB.
* **Discount impact:** Scatter & box plots confirm margin erosion with higher discounts.

### 5. Inferential Statistics

* **Welch’s t-test:** discounted vs non-discounted orders → margins significantly lower with discounts.
* **ANOVA:** margin differences across regions are statistically significant.

### 6. Deliverables

* Exported **cleaned dataset** to CSV and Excel for Tableau dashboarding.
* Developed executive-ready visualizations in Tableau.

---

## 💡 Key Insights

* **Discounts materially erode margins** (statistically significant).
* **Regional performance diverges:** AMER & EMEA profitable; APJ weak.
* **Enterprise > Strategic > SMB** in margin contribution.
* A small subset of products/customers drives most profit; several systematically destroy value.

---

## 📊 Recommendations

1. **Tighten discount policy** – cap discounts, enforce approval workflows, and review exceptions monthly.
2. **Double down on profitable regions** – scale resources in AMER/EMEA; reassess APJ go-to-market strategy.
3. **Prioritize Enterprise customers** – align campaigns and sales coverage to higher-margin accounts.
4. **Act on loss-making products/customers** – renegotiate contracts or discontinue offerings.
5. **Operational monitoring** – implement Tableau alerts for negative-margin orders; track quarterly margin KPIs.

---

## 📌 Next Steps

* Extend analysis with **predictive modeling** (e.g., regression on margin vs discount/segment).
* Automate Tableau dashboard refreshes.
* Integrate into a lightweight **Streamlit app** for demo.

---

✨ *This project bridges technical analysis with business decision-making, turning raw SaaS transaction data into actionable insights for growth and profitability.*
