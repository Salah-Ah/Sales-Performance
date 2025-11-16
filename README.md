# Sales-Performance

## Background & Overview

This project analyzes a retail company’s sales, costs, and profit performance over multiple years. The goal is to:

* Understand sales trends, regional performance, and product performance

* Identify high- and low-performing products and categories

* Examine costs and profitability to guide actionable decisions

The project was built using Excel with interactive navigation buttons and includes KPIs, charts, and insights.


## Data Structure & Modeling
<img width="1445" height="795" alt="Model" src="https://github.com/user-attachments/assets/12e01543-d198-4f00-bc45-6388e77d2c5c" />

Key Modeling Challenges:

* Same customer from multiple regions: Normalized Customer and Region tables separately; duplicates counted distinctly using DISTINCT where needed.

* Product name duplication: Removed inconsistent IDs, created a new index, and merged with fact table.

* Postcode conflicts: Normalized location by combining first letters of state + last letters of city + postal code using Power Query M Code.



## Executive Summary

### Top Insights:

1. Sales & Profit Trends: Highest sales in Nov, highest profit in Dec; lowest sales & profit in Jan–Feb

2. Top & Bottom Products by GM%: Some products with high sales have negative gross margin → review pricing/discount strategy

3. Cost Performance: Chairs & Phones are highest-cost subcategories but still profitable; Envelopes & Fasteners have low cost but high GM% → opportunity to scale

4. Regional Performance: Some regions consistently outperform others; targeted interventions can improve low-performing areas

## Analysis Deep Dive
### Sales Performance

Charts / KPIs: Total Sales, Total Cost, Total Quantity, # Orders, Total Profit

**Observations:**

1. Sales & Profit over time show increasing trend toward end-of-year

2. Bottom 10 products by GM% losing money per unit sold

**Insights / Recommendations:**

Investigate reasons for increasing profit (more orders, higher quantity, better cost control)

Review pricing & discount strategies on bottom 10 products

### Cost Performance

Charts / KPIs: Sub-Category GM%, Segments by Cost, Regions → States by Cost, Avg Cost per Order, Cost Over Time

**Insights:**

Chairs & Phones: high cost but positive GM% → optimize costs further

Envelopes & Fasteners: low cost, high GM% → increase sales volume

**Recommendations:**

Reduce costs for Chairs & Phones

Increase marketing campaigns for Envelopes & Fasteners

### Profit Performance

Charts / KPIs: Top/Bottom Products by Profit, Time by Profit & Quantity, Region & Category by Profit

**Insights:**

Some high-sales categories contribute little to profit

Need to align sales strategy with high-GM categories

## Recommendations (Actionable)
Area	Action
Sales Growth	Investigate profit growth causes; optimize quantity & orders
Product Portfolio	Focus on high-margin products; adjust pricing for low-margin products
Cost Management	Reduce cost for high-spend subcategories (Chairs & Phones)
Low-volume, high-GM products	Scale campaigns for Envelopes & Fasteners
Regional Strategy	Target low-performing regions with focused interventions
