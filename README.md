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

## Dashboard Pages
### 1. Executive Dashboard
Provides a high-level view of **Adventure Works' overall business performance**, covering revenue, profit, orders, return rate, revenue trends, category performance, and monthly KPIs. It also highlights top-performing products and key product trends to support quick executive-level decision-making.
<img src="images/executive-dashboard.png" width="100%">

### 2. Customer Details

Focuses on **customer performance and purchasing behavior**, with metrics for total customers, revenue per customer, orders by income level and occupation, and top customers by revenue. The page also enables users to explore customer trends and identify high-value customer segments.

### 3. Regional Analysis

Visualizes **sales and customer distribution across global markets** using an interactive map. Users can filter regions such as Europe, North America, and Pacific to compare geographic performance and identify markets with stronger customer activity.

### 4. Product Details

Provides a detailed view of **individual product performance against targets**, including orders, revenue, and profit. Interactive metric selection and parameter controls allow users to analyze product trends, compare actual performance with targets, and evaluate adjusted profit over time.


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

### 💡 Key Analytical Takeaways
**5. Where is performance strongest geographically?**
Territory and country analysis can reveal differences in market contribution and highlight areas for further investigation.

**6. Is the business meeting its targets?**
Actual-vs-target measures help stakeholders distinguish between absolute performance and performance relative to expectations.
