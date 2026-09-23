# Adventure-Works-Report
This report is an interactive **Power BI business intelligence dashboard** built using the Adventure Works dataset to analyze **sales, profitability, customers, products, returns, and geographic performance**, helping stakeholders monitor KPIs, identify trends, compare targets, and uncover actionable insights.

[📊 View Dashboard](https://github.com/akankshapillaii/Adventure-Works-Report/blob/main/AdventureWorks%20Report.pbix)

## Executive Summary

The Adventure Works dashboard provides a consolidated view of $24.9M in revenue, $10.5M in profit, 25.2K orders, and a 2.17% return rate across 17.41K customers. Overall performance is positive, but the analysis highlights a few areas that deserve attention: monthly revenue increased to $1.83M (+3.31%), while orders slightly declined to 2,146 (-0.88%); high-volume products are not always the strongest revenue contributors; and some product variants have return rates above 3%.

The key business opportunity is therefore not simply to increase sales volume, but to protect profitable products, understand high-return items, improve under-target product performance, and convert customer and regional insights into targeted actions.

## Table of Contents
- [Executive Summary]()
- [Business Problem](https://github.com/akankshapillaii/Adventure-Works-Report/blob/main/README.md#business-problem)
- [Dashboard]()
- [Key Stakeholders](https://github.com/akankshapillaii/Adventure-Works-Report#key-stakeholders)
- [Project Workflow](https://github.com/akankshapillaii/Adventure-Works-Report#project-workflow)
- [Data Structure & Initial Checks](https://github.com/akankshapillaii/Adventure-Works-Report#data-structure--initial-checks)
- [Dashboard Pages](https://github.com/akankshapillaii/Adventure-Works-Report#dashboard-pages)
- [Key KPIs](https://github.com/akankshapillaii/Adventure-Works-Report#key-kpis)
- [Analytical Capabilities](https://github.com/akankshapillaii/Adventure-Works-Report#analytical-capabilities)
- [Deep Dive Analysis & Findings](https://github.com/akankshapillaii/Adventure-Works-Report#-deep-dive-analysis--findings)

## Business Problem
Adventure Works needs a clear way to understand:
- How revenue, profit, orders, and returns are performing?
- Whether recent growth is coming from higher order volume or higher value per order?
- Which product categories and products are driving demand?
- Which products require attention because of elevated returns or weaker performance?
- How customer and regional patterns can support better business decisions?

The objective of this analysis was to turn transactional data into a decision-ready business view, rather than simply presenting a collection of charts.

## Dashboard
Power BI Report: [📊 View Dashboard](https://github.com/akankshapillaii/Adventure-Works-Report/blob/main/AdventureWorks%20Report.pbix)

The report contains four main analytical views:
|                   Page                         |                   Business Question                   |
|------------------------------------------------|-------------------------------------------------------|
|              Executive Dashboard               |         How is the business performing overall?       |
|                      Map                       |              Where is demand coming from?             |
|                Product Detail                  |       Which products are driving sales and profit?    |
|               Customer Detail                  |       Who are the customers driving business value?   |

## Key Stakeholders
- **Business Management** — Monitor overall sales, profitability, targets, and business performance
- **Sales Teams** — Track revenue, orders, targets, and sales trends
- **Product Teams** — Analyze product performance, profitability, demand, and returns
- **Customer Teams** — Understand customer contribution, purchasing behavior, and revenue per customer
- **Operations Teams** — Monitor orders, returns, and regional performance
- **Data / BI Teams** — Maintain dashboards, KPIs, data models, and analytical reporting

## Project Workflow
Business Requirements → Data Preparation → Data Modeling → DAX Measures → Interactive Report Design → KPI & Trend Analysis → Business Insights

## Data Structure & Initial Checks
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
| KPI                       |                         Value |
|---|---|
| **Revenue**	| $24.9M |
| **Total Profit** |	$10.5M |
| **Total Orders** | 25.2K |
| **Return Rate**	| 2.17% |
| **Unique Customers** | 17.41K |
| **Revenue per Customer** | ~$1K |

## Key Findings
1. Revenue is growing without an increase in order volume
Revenue increased from $1.77M to $1.83M (+3.31%), while orders fell from 2,165 to 2,146 (-0.88%).
- Business implication:
The latest revenue improvement appears to be driven by the value or mix of purchases rather than simply acquiring more orders. This makes product mix and customer purchasing behavior important areas to monitor.

2. Accessories generate the highest order volume
Order volume by category shows:
|       Category      ||          Orders |
|-----|-----|
| Accessories |     17.0K  |
|   Bikes  |   13.9K  |
Clothing

7.0K

Business implication:
Accessories are the largest contributor to order volume and represent an important opportunity for cross-selling and repeat purchases.

3. High-volume does not always mean high-revenue

Water Bottle – 30 oz

3,963 orders

$39.8K revenue

1.95% return rate

This is one of the strongest products by volume, but its revenue contribution is comparatively modest.

Fender Set – Mountain

1,975 orders

$87.0K revenue

1.36% return rate

Despite having roughly half the orders of the Water Bottle, the Fender Set generated more than 2× its revenue.

Business implication:
Management should evaluate products using both volume and value, rather than relying on order count alone.

4. Some products have noticeably higher return rates

Sport-100 Helmet variants

Product

Orders

Revenue

Return Rate

Sport-100 Helmet – Red

2,099

$73.4K

3.33%

Sport-100 Helmet – Blue

1,995

$67.1K

3.31%

Both variants have return rates above 3.3%, compared with the overall dashboard return rate of 2.17%.

Business implication:
These products should be investigated for possible common drivers such as product expectations, fit, quality, description accuracy, or customer segment differences.

5. Product targets identify opportunities for improvement

The Road Tire Tube reached approximately 91–92% of its target, with 213 orders against a 234-order target.

Business implication:
Products below target should be monitored separately from products that are already performing strongly. This creates a more focused approach to improving product-level performance.
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
