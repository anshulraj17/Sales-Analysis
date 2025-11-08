#  Sales & Returns Analysis Dashboard

### Advanced Business Intelligence Solution for Sales & Return Optimization  

This project showcases a **comprehensive Power BI dashboard** designed for a global manufacturer of cycling products.  
The goal was to transform raw transactional data into meaningful insights on **sales trends**, **product profitability**, **returns**, and **customer behavior**, enabling management to make data-driven decisions.

This project was completed as part of the **Maven Analytics Power BI Desktop** course, deepening my expertise in **data modeling**, **DAX formulation**, and **business storytelling through visualization**.

---

##  Business Objectives

The dashboard answers critical business questions such as:

- What are the key **revenue, profit, and return-rate KPIs**?  
- How has **sales performance evolved over time**, and what **seasonal patterns** emerge?  
- Which **products and categories** contribute most to revenue and returns?  
- How do **sales and profitability vary by region**?  
- Who are our **top-performing customers**, and what are their demographic or income trends?  
- What insights can reduce **return rates** and improve **customer retention**?

---

##  Tools & Technologies

| Tool / Technology | Purpose |
|--------------------|----------|
| **Microsoft Power BI Desktop** | Data modeling, DAX calculations, and dashboard design |
| **Power Query (M Language)** | Data extraction, transformation, and cleansing |
| **DAX (Data Analysis Expressions)** | Creation of measures, KPIs, and time-intelligence functions |
| **Excel / CSV** | Source-data storage and structure |

---

## Project Phases & Key Learnings

### 1️⃣ Data Acquisition & Transformation
- **Process:** Connected multiple CSV files for sales, returns, customers, geography, and calendar data. Cleaned missing values, standardized types, and merged datasets in Power Query.  
- **Learning:** Strengthened ETL knowledge — ensuring clean, reliable data for downstream analysis.

---

### 2️⃣ Data Modeling
- **Process:** Built a **Star Schema** model linking fact tables (*Sales*, *Returns*) with dimension tables (*Product*, *Customer*, *Calendar*, *Region*).  
- **Learning:** Mastered relational-model design and optimized relationships for high-performance filtering.

---

### 3️⃣ DAX Calculations
- **Process:** Created calculated measures and KPIs for core metrics:

```DAX
Total Revenue = SUM(Sales[SalesAmount])
Total Profit = SUM(Sales[Profit])
Return Rate = DIVIDE(SUM(Returns[Quantity]), SUM(Sales[Quantity]))
Profit Margin = DIVIDE([Total Profit], [Total Revenue])
YOY Growth = [Current Year Sales] - [Previous Year Sales]




---

### 4️⃣ Dashboard Design & Visualization

#### 🏠 Executive Dashboard
- **Purpose:** Provides a top-level summary of business performance, combining revenue, profit, and order insights.  
- **KPIs:**  
  - **$24.9M Revenue**  
  - **$10.46M Profit**  
  - **25K Total Orders**  
  - **2.17% Return Rate**
- **Key Visuals & Insights:**
  - *Revenue Over Time* → Month-wise sales trend and revenue growth.
  - *Orders by Category* → Distribution of total orders across **Accessories**, **Bikes**, and **Clothing**.
  - *Product Performance Table* → Comparison of **Total Revenue**, **Orders**, and **Return Rate** by product.
  - *Dynamic Highlights:*
    - **Most Ordered Product:** *Tires and Tubes*
    - **Most Returned Product:** *Shorts*

---

#### 🌍 Regional Map Dashboard
- **Purpose:** Visualizes geographical performance and identifies high-revenue markets.  
- **Key Visuals & Insights:**
  - *Total Revenue by Region (Map Visualization)* → Interactive map depicting **North America**, **Europe**, and **Pacific** territories.  
  - **Observations:**
    - *United States* records the highest total sales.
    - *Australia* shows the highest average revenue per customer.
    - *Germany* and *United Kingdom* display consistent growth.

---

#### 📦 Product Details Dashboard
- **Purpose:** Focuses on product-level KPIs and performance against monthly targets.  
- **Key Metrics:**
  - **Monthly Orders vs Target Orders**
  - **Monthly Revenue vs Target Revenue**
  - **Return Rate Trend**
- **Key Visuals & Insights:**
  - *Metric Selector Panel* → Toggle between **Total Orders**, **Total Revenue**, **Total Returns**, and **Return Rate**.
  - *Profit Over Time* → Trend of actual vs adjusted profit.
  - *Return Rate Over Time* → Fluctuations in return percentage over months.
- **Insight:**  
  Helps identify underperforming or high-return products, aiding inventory and pricing optimization.

---

#### 👥 Customer Insights Dashboard
- **Purpose:** Examines customer segmentation, spending behavior, and income-based trends.  
- **KPIs:**
  - **17K Unique Customers**
  - **$1.43K Avg Revenue per Customer**
- **Key Visuals & Insights:**
  - *Top 10 Customers by Revenue* → Highlights highest revenue contributors.
  - *Orders by Income Level* → Customer distribution across **Professional**, **Skilled Manual**, **Clerical**, and **Management** groups.
  - *Customer Growth Over Time* → Rising trend in total customer base post-2021.
- **Filters & Interactivity:**
  - Region and Income Level filters for exploring specific customer segments.
- **Insights:**
  - *Professional (31%)* and *Skilled Manual (24%)* segments dominate order volume.
  - *Maurice Shan* recorded the highest total purchase value of **$12.4K**.

---



📊 Key Insights & Findings

📈 Revenue Trend: Consistent growth with seasonal peaks in Q4.

🏆 Product Performance: Bikes drive maximum revenue; Accessories contribute volume with lower margins.

🌍 Regional Trends: North America leads sales; Australia shows higher avg revenue per customer.

🔄 Return Analysis: Shorts and Helmets record ~3–3.5 % returns — potential quality issues.

👥 Customer Insights: Professional & Skilled Manual groups generate 55 %+ of revenue.

📉 Optimization Scope: Improving top returned products can reduce return rate by ≈ 0.8 %.

💡 Business Impact & Recommendations

Enforce quality checks for high-return categories (Shorts, Helmets).

Introduce loyalty offers to increase repeat purchases.

Focus marketing in high-performing regions (U.S., Germany, Australia).

Align pricing and inventory with seasonal demand peaks.



---

## 📊 Key Insights & Findings

- **📈 Revenue Trend:** Consistent growth observed throughout the timeline with clear seasonal peaks during Q4.  
- **🏆 Product Performance:** _Bikes_ generated the highest revenue, while _Accessories_ maintained high order volume but lower profit margins.  
- **🌍 Regional Trends:** _North America_ leads in overall sales, whereas _Australia_ shows higher average revenue per customer.  
- **🔄 Return Analysis:** _Shorts_ and _Helmets_ recorded ~3–3.5% return rates, indicating potential sizing or quality issues.  
- **👥 Customer Insights:** _Professional_ and _Skilled Manual_ income groups contribute over **55%** of total revenue.  
- **📉 Optimization Scope:** Improving top returned products could reduce overall return rates by approximately **0.8%**.  

---





---

## 📁 Repository Structure

| File / Folder | Description |
|----------------|-------------|
| `AdventureWorks.pbix` | Main Power BI dashboard file |
| `/data/` | Raw and processed datasets |
| `/snips/` | Dashboard screenshots and visual snippets |

---
