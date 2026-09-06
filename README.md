# 🛒 Olist E-Commerce Marketplace Analytics

An end-to-end **Data Analytics & Business Intelligence project** built using **Python, Pandas, Matplotlib, and Power BI** on the Olist Brazilian e-commerce marketplace dataset.

The project focuses on understanding **marketplace performance, sales trends, delivery efficiency, customer satisfaction, product categories, seller performance, and payment behavior** through data-driven analysis and an interactive Power BI dashboard.

---

## 📌 Project Overview

The objective of this project is to transform raw e-commerce data into meaningful business insights that can help understand:

- 📈 Sales and order trends over time
- 🚚 Delivery performance and delivery delays
- ⭐ Customer satisfaction and review patterns
- 🛍️ Product category performance
- 🏪 Seller performance across locations
- 💳 Payment methods and installment behavior
- 🔎 Factors associated with low customer ratings

The analysis was performed in **Python**, and the final insights were presented through a **3-page Power BI dashboard**.

---

## 🎯 Business Questions

This project addresses the following key questions:

1. How did marketplace orders and sales change over time?
2. How does delivery performance affect customer satisfaction?
3. Which product categories generate the highest sales?
4. Which categories have better or lower customer satisfaction?
5. Are certain sellers or seller locations associated with lower ratings?
6. How do payment types and installment plans relate to customer reviews?
7. What are the major factors associated with low review scores?
8. Where are the biggest opportunities for improving marketplace performance?

---

## 🧰 Technologies & Tools

| Tool | Purpose |
|---|---|
| 🐍 Python | Data cleaning, transformation and analysis |
| 🐼 Pandas | Data manipulation and aggregation |
| 📊 Matplotlib | Exploratory data visualization |
| 📊 Power BI | Interactive dashboard and business reporting |
| 📁 Excel / CSV | Dataset storage and prepared analytical data |
| 📓 Jupyter / Google Colab | Python analysis environment |

---

## 📂 Dataset

The project uses the **Olist Brazilian E-Commerce dataset**, containing information about:

- Orders
- Order items
- Payments
- Reviews
- Customers
- Products
- Sellers
- Geolocation
- Product category translation

The original dataset contains approximately **100K orders** and multiple related tables.

### Prepared Master Dataset

A final order-level analytical dataset was created by combining relevant information from the source tables.

**Final dataset:**
- Rows: **99,441**
- Columns: **29**
- Unique Orders: **99,441**
- Duplicate Orders: **0**

The master dataset includes information such as:

- Order details
- Customer location
- Review score
- Product category
- Item and freight value
- Payment information
- Delivery days
- Delivery delay
- Delivery status
- Low-review indicator

---

## 🔄 Data Analysis Workflow

```text
Raw Olist Dataset
       ↓
Data Loading
       ↓
Data Cleaning & Validation
       ↓
Date & Delivery Analysis
       ↓
Review & Customer Satisfaction Analysis
       ↓
Product & Category Analysis
       ↓
Payment Analysis
       ↓
Seller & Geographic Analysis
       ↓
Order-Level Master Dataset
       ↓
Power BI Dashboard
       ↓
Business Insights
```

---

# 📊 Key Performance Indicators

| KPI | Value |
|---|---:|
| Total Orders | **99,441** |
| Delivered Orders | **96,470** |
| Total Sales | **15.84M** |
| Average Review Score | **4.14 / 5** |
| Average Delivery Time | **12.09 days** |
| Late Delivery Rate | **6.77%** |
| Low Review Rate (1–2) | **13.12%** |
| Average Order Value | **159.33** |
| Total Items Sold | **113K** |

---

# 🔍 Key Insights

## 🚚 Delivery & Customer Satisfaction

One of the strongest findings is the relationship between delivery delays and customer satisfaction.

| Delivery Status | Avg. Review Score |
|---|---:|
| On Time / Early | **4.28** |
| Late | **2.26** |

As delivery delays increase, average review scores generally decline.

Examples:

- On Time / Early → **4.28**
- 1–3 days late → **3.28**
- 4–7 days late → **2.09**
- 8–14 days late → **1.67**
- 15+ days late → **1.72**

This indicates that **delivery performance is strongly associated with customer satisfaction**.

> **Main Insight:** Improving delivery reliability is one of the most important opportunities identified in this analysis.

---

## ⭐ Customer Reviews

The overall average review score is **4.14 / 5**.

Review distribution:

- ⭐ 1 → 11.86%
- ⭐ 2 → 3.24%
- ⭐ 3 → 8.29%
- ⭐ 4 → 19.20%
- ⭐ 5 → 57.42%

Although most customers gave positive ratings, low reviews are strongly associated with delayed deliveries.

---

## 🛍️ Product Category Performance

The highest-revenue categories include:

1. **Health & Beauty**
2. **Watches & Gifts**
3. **Bed & Bath Table**
4. **Sports & Leisure**
5. **Computers & Accessories**

The analysis also compares category revenue with customer satisfaction to identify categories that perform well commercially but may need improvement in customer experience.

---

## 💳 Payment Analysis

Payment methods analyzed include:

- Credit Card
- Boleto
- Voucher
- Debit Card

Customer satisfaction differences across payment types are relatively small compared with the much stronger relationship observed between delivery delays and reviews.

Installment analysis also shows only a modest change in average review scores as the number of installments increases.

**Conclusion:** Payment behavior appears to be a weaker driver of customer satisfaction than delivery performance in this dataset.

---

## 🏪 Seller & Geographic Analysis

Seller-level and seller-state analysis was performed to identify geographic patterns in:

- Average review score
- Low-review rate
- Delivery delay
- Freight value

Some low-rated sellers do not have unusually high delivery delays, suggesting that **not all customer dissatisfaction can be explained by delivery timing alone**.

This indicates the potential importance of other factors such as product experience, seller service, order handling, or category-specific issues.

---

# 📊 Power BI Dashboard

The final Power BI report contains **3 interactive pages**.

### 1️⃣ Executive Overview

Provides a high-level view of:

- Total Orders
- Total Revenue
- Average Review Score
- Late Delivery Rate
- Average Delivery Days
- Monthly Sales Trend
- Review Distribution
- Category Sales
- Category Satisfaction
- Low Review Rate by Delivery Status

### 2️⃣ Delivery & Customer Experience

Focuses on:

- Delivery delay groups
- Customer satisfaction vs delivery delay
- Review score distribution
- Delivery KPIs
- Low-review patterns

### 3️⃣ Product & Seller Performance

Includes:

- Top product categories by sales
- Category satisfaction
- Payment type vs customer satisfaction
- Installment group vs customer satisfaction
- Payment type distribution
- Product, payment and customer insights

---

# 📁 Project Structure

```text
Olist-E-Commerce-Marketplace-Analytics/
│
├── README.md
│
├── Olist_Analysis.ipynb
│
├── olist_powerbi_master.csv
│   └── Prepared order-level analytical dataset
│
├── Olist_Ecommerce_Marketplace_Analytics.pbix
│   └── Power BI dashboard
│
└── screenshots/
    └── Dashboard screenshots
```

If the dataset or Power BI file is too large for GitHub, the corresponding compressed file or external file link can be provided separately.

---

# 💡 Recommendations

Based on the analysis:

### 🚚 1. Improve Delivery Reliability
Focus on reducing late deliveries, especially orders with repeated or significant delays.

### 🏪 2. Investigate Underperforming Sellers
Identify sellers with consistently low ratings and investigate operational or service-related issues.

### 🛍️ 3. Monitor Category-Level Experience
High-revenue categories with relatively lower satisfaction should receive additional attention.

### 📦 4. Improve Logistics Monitoring
Use delivery-delay indicators to identify potentially dissatisfied customers and operational bottlenecks.

### ⭐ 5. Track Customer Experience
Review scores can be used alongside delivery metrics to monitor marketplace health.

---

# ⚠️ Important Analytical Note

The project identifies **associations and patterns**, not guaranteed causal relationships.

For example, delayed delivery is strongly associated with lower review scores, but this analysis alone does not prove that delivery delay is the only cause of a low review.

---

# 👨‍💻 Project Summary

This project demonstrates an end-to-end analytics workflow:

**Data → Cleaning → EDA → Feature Engineering → Business Analysis → Power BI Dashboard → Insights**

The final goal is to turn complex e-commerce data into **clear, actionable business insights** for improving sales performance, logistics, and customer experience.

---

## 🚀 Project Highlights

- ✅ 99K+ orders analyzed
- ✅ 29-column analytical master dataset
- ✅ Delivery delay analysis
- ✅ Customer satisfaction analysis
- ✅ Product category analysis
- ✅ Seller performance analysis
- ✅ Payment behavior analysis
- ✅ Geographic analysis
- ✅ Interactive 3-page Power BI dashboard
- ✅ Business recommendations

---

**Built with 🐍 Python + 📊 Power BI + ❤️ Data Analytics**
