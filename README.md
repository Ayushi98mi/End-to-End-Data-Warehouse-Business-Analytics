# End-to-End-Data-Warehouse-Business-Analytics
This project demonstrates a comprehensive data warehousing and analytics solution, from building a data warehouse to generating actionable insights. Designed as a portfolio project, it highlights industry best practices in data engineering and analytics.

## Data Architecture
The data architecture for this project follows Medallion Architecture Bronze, Silver, and Gold layers:

<img width="854" height="639" alt="DATA_ARCHITECTURE drawio" src="https://github.com/user-attachments/assets/b2d4eb39-e245-4eb5-bd8d-41319b9b68a7" />


- **Bronze Layer:** Stores raw data as-is from the source systems. Data is ingested from CSV files into SQL Server Database.

- **Silver Layer:** This layer includes data cleansing, standardization  processes to prepare data for analysis.

- **Gold Layer:** Houses business-ready data modeled into a star schema required for reporting and analytics.

---
## 📖 Project Overview

This project involves:

1. **Data Architecture**: Designing a Modern Data Warehouse Using Medallion Architecture **Bronze**, **Silver**, and **Gold** layers.
2. **ETL Pipelines**: Extracting, transforming, and loading data from source systems into the warehouse.
3. **Data Modeling**: Developing fact and dimension tables optimized for analytical queries.
4. **Analytics & Reporting**: Creating SQL-based reports for actionable insights.

---

## 🚀 Project Requirements

### Building the Data Warehouse (Data Engineering)

#### Objective
Develop a modern data warehouse using SQL Server to consolidate sales data, enabling analytical reporting and informed decision-making.

#### Specifications
- **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
- **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
- **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
- **Scope**: Focus on the latest dataset only; historization of data is not required.
- **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics teams.

---
## 🛠️ Tools & Technologies
- **Database:** SQL Server, SSMS
- **Data Visualization:** Draw.io (Data Architecture Diagram)
- **Version Control:** GitHub
- **Data Format:** CSV Files

- ## Key Insights & Business Recommendations

### 1. Bikes Category Dominates Revenue
Bikes generate **96.46% of total revenue** ($28.3M out of $29.4M total sales), 
while Accessories and Clothing contribute only 2.39% and 1.16% respectively.
**Recommendation:** While Bikes is clearly the core revenue driver, this 
extreme concentration (96%+) represents a risk. Consider whether Accessories 
and Clothing are under-promoted (e.g., not bundled with bike purchases), or 
whether this simply reflects a specialty bike business model.

### 2. Mountain-200 Series Drives Top-End Revenue
All 5 top-revenue products are variants of the **Mountain-200** bike 
(different colors and sizes), each generating $1.29M–$1.37M individually. 
This single product line alone accounts for a substantial share of total 
Bikes revenue.
**Recommendation:** Given how concentrated revenue is in one product line, 
ensure supply chain and inventory planning prioritize Mountain-200 
availability, and evaluate whether its design/pricing strategy could be 
extended to other underperforming lines.

### 3. Customer Base is Overwhelmingly New, Not Retained
Of 18,484 total customers, **79% (14,631) fall into the "New" segment** 
(less than 12 months of purchase history), while only 9% (1,655) are VIP 
and 12% (2,198) are Regular customers.
**Recommendation:** This signals a potential retention problem — strong at 
acquiring new customers but weak at converting them into repeat buyers. 
A loyalty program or targeted re-engagement campaign for first-time buyers 
could meaningfully grow the VIP/Regular segments over time.

### 4. Top Customers Show Balanced, Non-Concentrated Spending
The top 10 customers by revenue each contribute between $12,914–$13,294 — 
a narrow range with no single customer dominating. This is a healthy sign: 
revenue isn't overly dependent on a handful of big spenders.

### 5. Low-Performing Products Are Small Accessories
The lowest-revenue products (e.g., Racing Socks variants at $2,430–$2,682, 
Patch Kits, Bike Wash) are all low-cost accessory items — consistent with 
the broader finding that Accessories/Clothing underperform Bikes 
significantly. There's a stark contrast: top products earn 500x+ more 
revenue than the bottom products.
**Recommendation:** Evaluate whether these low-revenue SKUs justify their 
inventory/shelf space, or whether they serve a strategic cross-sell 
purpose (e.g., paired with bike purchases) despite low standalone revenue.

### 6. Data Spans Over 3 Years, Enabling Reliable Trend Analysis
With order data ranging from Dec 2010 to Jan 2014 (37 months), the dataset 
is large enough to support meaningful year-over-year and seasonal analysis, 
not just a single snapshot.

### Suggested Next Steps
- Investigate why 79% of customers remain "New" — analyze whether there's 
  a specific drop-off point after the first purchase.
- Run a bundle/cross-sell analysis: do customers who buy Mountain-200 bikes 
  also buy Accessories, or are these largely separate purchase behaviors?
- Compare average order value between New, Regular, and VIP segments to 
  quantify the revenue upside of converting more customers to Regular/VIP.
- Assess whether low-revenue accessory SKUs (e.g., Racing Socks) should be 
  discontinued or repositioned as cross-sell add-ons.

## 👩‍💻 About
Built as part of my self-learning journey in Data Analytics 
while pursuing Chemical Engineering at IIT Jammu.
Implemented each component independently following 
industry best practices.
