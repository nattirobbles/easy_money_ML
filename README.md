# 💳 Easy Money - Customer Analytics & Machine Learning
Customer analytics project using machine learning to predict customer behavior and segment users to support marketing decision-making.


## 📌 Project Overview

This project analyzes customer and transactional data from EasyMoney, a digital financial services platform, with the goal of improving marketing efficiency and increasing customer value through a **market penetration strategy**.

The analysis covers a 17-month period and focuses on understanding customer behavior, product adoption, and business performance over time. Key aspects include the evolution of net margin, customer engagement, and the differences between new and existing customers.

Particular attention is given to identifying opportunities to increase product penetration among existing customers, as well as detecting imbalances between high-volume and high-margin products and retention issues in specific categories such as investment products.

Building on these insights, a machine learning approach was applied, including a **propensity model** to predict customer purchases and a **clustering model** to segment users based on financial behavior and product usage.

Finally, the results were translated into business impact through a campaign simulation, estimating ROI and enabling more efficient, targeted marketing strategies.

---

## 🧠 Business Problem

**Who should be contacted next month to maximize product conversions without wasting marketing budget on low-probability customers?**

---

## 🎯 Objectives

* Predict customer propensity to purchase financial products
* Segment customers based on behavior and product usage
* Optimize marketing campaigns through data-driven targeting

---

## 📊 Exploratory Analysis

Power BI dashboards were developed to analyze customer behavior and business performance over time.

### Analysis included:

* Evolution of net margin and product adoption
* Active vs inactive customers (app usage)
* New vs existing customers
* Product distribution and profitability

### Key insights:

* Sales growth peaked during the second half of 2018, with net margin peaks in February and July
* While early growth was driven by new customers, **existing customers became the main revenue drivers over time**
* Customer engagement increases with tenure and product adoption
* App-active users show higher product penetration
* Sales volume is highly concentrated in account-type products
* **High-margin products (e.g. investment/pension-related) generate most of the profitability (~79%) despite lower volume**
* A churn issue was detected in investment products, indicating low retention after acquisition

---

## 🧪 Solution

### 🔹 Propensity Model

A classification model was built to predict the probability of a customer purchasing a financial product in the next month.

To simplify the problem, the 15 products were grouped into:

* Savings
* Financing
* Investment
* Daily banking

**Results:**

* Top 10% of customers capture ~70% of buyers
* **Lift: ~7x vs mass campaigns**

---

### 🔹 Customer Segmentation

Customers were segmented into **7 clusters using K-Means** based on financial profile and product usage.

**Data preparation:**

* Salary outliers were treated using **winsorization (1st–99th percentiles)**
* This prevented artificial clusters driven by extreme values

---

## 💰 Business Impact

A campaign simulation was developed to estimate the financial impact of targeted marketing:

* **ROI: 2,769%**
* **Estimated profit: €4.4M**
* Significant improvement vs mass campaigns

---

## 📊 Visualizations

Dashboards built in Power BI to communicate insights:

* Customer segmentation
* Product performance
* Propensity distribution
* Campaign impact

![Dashboard](dashboards/top_decile_profile.png)

---

## 🚀 Key Recommendations

* Prioritize cross-selling over customer acquisition
* Focus on high-margin products (e.g. pension plans)
* Use propensity scoring for targeted campaigns
* Improve retention in investment products
* Leverage the app as the main engagement channel

---

## 🛠️ Tools & Technologies

* Python (Pandas, NumPy, Scikit-learn)
* Jupyter Notebooks
* Power BI

---

## 📝 Notes

All notebooks and analysis are written in Spanish, as this project was developed during the second part of a Master’s program.

The README is provided in English for broader accessibility.

