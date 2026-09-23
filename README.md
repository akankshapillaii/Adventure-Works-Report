# Adventure-Works-Report
This report is an interactive **Power BI business intelligence dashboard** built using the Adventure Works dataset to analyze **sales, profitability, customers, products, returns, and geographic performance**, helping stakeholders monitor KPIs, identify trends, compare targets, and uncover actionable insights.

[📊 View Dashboard](https://github.com/akankshapillaii/Adventure-Works-Report/blob/main/AdventureWorks%20Report.pbix)

## Business Problem
A large transactional dataset can contain valuable information about business performance, but extracting meaningful insights from raw records can be difficult.

Business stakeholders need to quickly understand:
- How much revenue is being generated?
- Is profitability keeping pace with revenue?
- Which products generate the most orders and revenue?
- Which products have higher return rates?
- How large and valuable is the customer base?
- Which markets contribute most to performance?
- Are individual products meeting their targets?
- How is performance changing month over month?
This project addresses these questions through a centralized, interactive Power BI reporting environment.

## Business Objectives
The dashboard was designed to help stakeholders:
- Monitor **sales, revenue, profit, orders, and customer KPIs**
- Compare **actual performance against targets**
- Identify **product and customer performance trends**
- Analyze **returns and their impact on sales**
- Explore performance across **time, territories, and countries**
- Drill down into **product and customer-level insights**
- Support **data-driven business decision-making**

## Key Stakeholders
- **Business Management** — Monitor overall sales, profitability, targets, and business performance
- **Sales Teams** — Track revenue, orders, targets, and sales trends
- **Product Teams** — Analyze product performance, profitability, demand, and returns
- **Customer Teams** — Understand customer contribution, purchasing behavior, and revenue per customer
- **Operations Teams** — Monitor orders, returns, and regional performance
- **Data / BI Teams** — Maintain dashboards, KPIs, data models, and analytical reporting

## Project Workflow
Business Requirements → Data Preparation → Data Modeling → DAX Measures → Interactive Report Design → KPI & Trend Analysis → Business Insights

# 🧩 Data Structure & Initial Checks
The Adventure Works data structure as seen below is connecting **sales transactions with product, customer, territory, returns, and calendar information** to support multi-dimensional analysis.

<p align="center">
  <img src="Dashboard Preview/Data Model.png" width="100%">
</p>

### Initial Data Checks
- Reviewed the available tables and fields.
- Checked data types and column consistency.
- Identified key fields required for table relationships.
- Validated relationships between transactional and lookup tables.
- Reviewed the data model to ensure it supported the required KPIs and analysis.

## Dashboard Pages
### 1. Executive Dashboard
Provides a high-level view of **Adventure Works' overall business performance**, covering revenue, profit, orders, return rate, revenue trends, category performance, and monthly KPIs. It also highlights top-performing products and key product trends to support quick executive-level decision-making.

<p align="center">
<img src="Dashboard Preview/Exec Dashboard.png" width="65%">
</p>

### 2. Regional Analysis
Visualizes **sales and customer distribution across global markets** using an interactive map. Users can filter regions such as Europe, North America, and Pacific to compare geographic performance and identify markets with stronger customer activity.

<p align="center">
<img src="Dashboard Preview/Map.png" width="65%">
</p>

### 3. Customer Details
Focuses on **customer performance and purchasing behavior**, with metrics for total customers, revenue per customer, orders by income level and occupation, and top customers by revenue. The page also enables users to explore customer trends and identify high-value customer segments.

<p align="center">
<img src="Dashboard Preview/Customer Details.png" width="65%">
</p>

### 4. Product Details
Provides a detailed view of **individual product performance against targets**, including orders, revenue, and profit. Interactive metric selection and parameter controls allow users to analyze product trends, compare actual performance with targets, and evaluate adjusted profit over time.

<p align="center">
<img src="Dashboard Preview/Product Details.png" width="65%">
</p>

## Key KPIs
The executive dashboard provides a high-level snapshot of the business:
| KPI | Value |
|---|---|
| **Revenue**	| $24.9M |
| **Total Profit** |	$10.5M |
| **Total Orders** | 25.2K |
| **Return Rate**	| 2.17% |
| **Unique Customers** | 17.41K |
| **Revenue per Customer** | ~$1K |

## Analytical Capabilities
The dashboard was designed around several important analytical questions.

### Trend Analysis
How are revenue, profit, and orders changing over time?
The calendar model supports analysis across:
- Year
- Quarter
- Month
This makes it possible to identify changes in business performance and investigate periods of growth or decline.

### Target Analysis
Performance is not evaluated solely through absolute numbers.
The report incorporates:
- Actual Performance
- Target
- Target Gap
This allows stakeholders to understand whether performance is aligned with expectations.

### Product Performance
Product-level analysis helps identify:
- High-revenue products
- High-profit products
- Product categories driving performance
- Subcategory contribution
- Products requiring further investigation

### Customer Performance
Customer analysis focuses on:
- Customer contribution
- Revenue per customer
- Customer-level performance
- Demographic characteristics
This provides a stronger understanding of who contributes to revenue, rather than looking only at overall sales.

### Geographic Analysis
Territory and country-level fields allow sales performance to be explored geographically.
This can help identify:
- Strong-performing markets
- Geographic concentration
- Regional performance differences
- Markets requiring deeper investigation

### Returns Analysis
Returns are incorporated into the dashboard to provide additional context around sales performance.
Instead of evaluating sales in isolation, stakeholders can investigate whether strong sales are accompanied by higher return activity.

## 🔍 Deep Dive Analysis & Findings
### Understanding Sales Performance Through Data
The dashboard provides an overview of **$24.9M in revenue, $10.5M in profit, and 25.2K orders**, allowing overall business performance to be evaluated alongside product, customer, return, and geographic metrics.

### Revenue Increased Despite Lower Order Volume
The latest monthly comparison shows revenue increasing from **$1.77M to $1.83M**, a **3.31% increase**, while orders decreased from **2,165 to 2,146**, a **0.88% decline**.

> **Finding:** Revenue growth alongside lower order volume creates an opportunity to investigate changes in average order value, product mix, or higher-value product contribution.

### Accessories Drive the Highest Order Volume
**Accessories recorded 17.0K orders**, followed by **Bikes with 13.9K** and **Clothing with 7.0K**.

> **Finding:** Accessories represent the highest order-volume category and provide an opportunity to further investigate their revenue contribution, product mix, and return behavior.

### Order Volume Does Not Always Translate Into Higher Revenue
**Water Bottle - 30 oz** recorded **3,963 orders and $39.8K revenue**, while **Fender Set - Mountain** recorded **1,975 orders and $87.0K revenue**.

> **Finding:** Product performance should be evaluated using multiple KPIs rather than order volume alone.

### High-Revenue Products Can Have Higher Return Rates
The **Sport-100 Helmet - Red** generated **$73.4K revenue** with a **3.33% return rate**, while the **Sport-100 Helmet - Blue** generated **$67.1K revenue** with a **3.31% return rate**.

Both are above the overall **2.17% return rate**.

> **Finding:** High-performing products with elevated return rates may require further investigation across product, customer, and geographic dimensions.

### Product Performance Against Targets
For the selected **Road Tire Tube**:
| Metric | Actual | Target |
|---|---:|---:|
| Orders | **213** | 234 |
| Revenue | **$1,668** | $1,804 |
| Profit | **$1,044** | $1,129 |

All three metrics achieved approximately **91–92% of their respective targets**.

> **Finding:** The consistent target gap across orders, revenue, and profit provides an opportunity to investigate the factors affecting product performance.

### Customer Value Adds Another Perspective
The dashboard includes **17.41K unique customers** with approximately **$1K revenue per customer**.
The selected top customer generated **$12.408K revenue from 6 orders**.

> **Finding:** Customer-level analysis provides additional insight into revenue concentration and helps identify high-value customers beyond overall customer counts.

### Overall Finding
The analysis moves beyond **"How much did the business sell?"** to understand **what is driving performance, which products contribute most, how customers contribute to revenue, where returns are concentrated, and how performance compares with targets**.

By bringing these dimensions together, the dashboard provides a data-driven view of business performance and highlights areas where **product, customer, operational, and geographic analysis can be explored further**.
