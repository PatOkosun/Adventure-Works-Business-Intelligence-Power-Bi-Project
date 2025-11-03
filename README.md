# Adventure-Works-Business-Intelligence-Power-Bi-Project

## Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data cleaning and preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Key Insights](#key-insights)
- [Recommendations and Strategic Impact](#recommendations-and-strategic-impact)
- [References](#references)

- ### Project Overview

The AdventureWorks Power BI Report delivers interactive insights into sales, revenue, profit, and customer behavior across regions and products. It enables data-driven decisions through trend analysis, profitability tracking, and customer segmentation. Built with Power BI, DAX, and SQL, the report identifies high-performing products, monitors KPIs, and highlights areas for growth and optimization, helping business leaders improve strategy, efficiency, and profitability. 

This project combines data cleaning, analysis, and visualization to deliver an intuitive and interactive experience for stakeholders. As a data analyst, this project served as a hands-on opportunity to apply my skills and knowledge in a real-world setting.

---

### Analysis Dashboard
#### Executive Sales Summary Dashboard 

![dashboad](https://github.com/PatOkosun/Adventure-Works-Business-Intelligence-Power-Bi-Project/blob/main/Executive%20Sales%20Overview.png)

The Executive Dashboard delivers a strategic snapshot of AdventureWorks’ business performance, combining key financial, operational, and product insights to guide executive decision-making.

Performance Overview:
AdventureWorks achieved $24.9M in revenue, $10.5M in profit, and processed 25.2K orders, maintaining a 2.2% return rate—reflecting strong sales execution and operational efficiency.

Revenue & Growth Trends:
Revenue has shown a steady upward trajectory since 2020, supported by consistent demand recovery and product diversification. Recent months highlight continued growth momentum with a 3.31% month-over-month increase in revenue, indicating sustained customer engagement and market strength.

Category & Product Insights:
The Accessories category leads performance with 17K orders, followed by Bikes and Clothing, underscoring strong consumer interest in complementary products. Among top-performing items, the Water Bottle – 30 oz. and Sport-100 Helmet series demonstrate high-volume sales with balanced return rates—key indicators of customer satisfaction and pricing effectiveness.

Operational Efficiency:
Monthly KPIs suggest stable performance—orders show a minor 0.88% decrease, while return volumes remain controlled at a 1.78% variance, signaling effective inventory and quality management.

Executive Insight:
This dashboard enables leadership to monitor profitability, identify growth levers, and assess category performance at a glance. It supports data-driven strategic planning by aligning revenue trends, product demand, and customer behavior with organizational goals.

---
#### Product Performance Dashboard 
##### Description: Analyzes product-level sales, profit trends, and returns. Identifies top-performing items and evaluates pricing and profitability changes over time.
![dashboad](https://github.com/PatOkosun/Adventure-Works-Business-Intelligence-Power-Bi-Project/blob/main/Product%20Overview-1.png )


---
#### Customer Insights Dashboard
##### Description: Examines customer demographics, purchase behavior, and revenue contribution by income level and occupation to guide targeted marketing strategies
![dashboad](https://github.com/PatOkosun/Adventure-Works-Business-Intelligence-Power-Bi-Project/blob/main/Customer%20Overview-1.png)


---

#### Geographical Performance Dashboard
##### Description:  Visualizes revenue distribution across countries and continents, enabling geographic performance comparison and market opportunity identification.
![dashboad](https://github.com/PatOkosun/Adventure-Works-Business-Intelligence-Power-Bi-Project/blob/main/Map%20Overview-1.png)


---
### Data Sources
The analysis is powered by data housed within the “Raw Data” repository, which contains comprehensive datasets used by the AdventureWorks business to monitor and evaluate performance across multiple dimensions.

These datasets provide detailed information on sales, products, customers, territories, and returns, enabling a holistic view of organizational operations and performance trends. The primary files include:

AdventureWorks Calendar Lookup.csv – Provides time-based dimensions for trend and period analysis.

AdventureWorks Customer Lookup.csv – Contains customer demographics and segmentation details.

AdventureWorks Product Categories Lookup.csv – Defines high-level product groupings for category performance analysis.

AdventureWorks Product Subcategories Lookup.csv – Breaks down product categories into detailed subgroups.

AdventureWorks Product Lookup.csv – Provides SKU-level product details for revenue, profit, and return insights.

AdventureWorks Territory Lookup.csv – Maps sales data to geographic territories for regional performance evaluation.

AdventureWorks Return Data.csv – Captures product return transactions to assess return rates and quality trends.

AdventureWorks Sales Data 2020.csv, 2021.csv, 2022.csv – Contain historical sales transactions across three fiscal years, supporting longitudinal analysis.

Product Category Sales (Unpivot Demo).csv – Demonstrates unpivoted category-level sales for advanced data modeling and visualization.

Together, these datasets form the foundation of the AdventureWorks Power BI Report, enabling accurate trend analysis, profitability tracking, and customer insights across time, geography, and product lines.

---
### Tools
- Power Bi
  -  Data Cleaning
  -  Data Modelling 
  -  Power Query - ETL (Extraction, Transform and Load data).
  -  Dax (Data analytical Expressions).
  -  Business Metrics 
  -  Data Analysis.
  -  Data Visualization.
 
    ---
 
### Data cleaning and preparation 

1. In the initial phase of the project, extensive data cleaning and preparation were conducted to ensure data accuracy, consistency, and readiness for Power BI modeling. The following key steps were performed:

2. Data Import – Connected Power BI to multiple raw source files, including sales, product, customer, and store datasets.

3. Data Type Formatting – Defined appropriate data types (e.g., dates, currency, and text) to support accurate calculations and visuals.

4. Column Renaming – Standardized and renamed columns to maintain clarity and consistency across all tables.

5. Filtering and Validation – Removed blank records, duplicates, and irrelevant rows to maintain data integrity.

6. Merging & Relationships – Established relationships and merged tables (e.g., Sales ↔ Products ↔ Customers ↔ Stores) for seamless data integration.

7. Text and Category Cleaning – Trimmed spaces, corrected inconsistent casing, and standardized product and category names.

8. Calculated Columns & Measures – Created new fields such as Profit, Profit Margin, and Return Rate to enhance analytical depth.

9. Date Table Creation – Developed or linked a dedicated date table to support time intelligence functions and trend analysis.

10. Data Aggregation – Grouped and summarized transactional data to improve performance and simplify reporting at various granularity levels.

Through these processes, the dataset was transformed from raw, inconsistent files into a clean, structured, and analysis-ready data model, forming the foundation for the AdventureWorks Power BI Executive Dashboard.

---
### Data Modelling 
Following the data cleaning and preparation phase, the data modelling stage focused on establishing robust relationships and a scalable analytical structure to enable efficient data exploration within Power BI.

The objective of this stage was to design a semantic data model that integrates multiple datasets into a unified framework, supporting accurate calculations and intuitive reporting.  The following key activities were performed:

- Model Design – Implemented a star schema with a central Sales Fact Table linked to dimension tables (Products, Customers, Calendar, Territories, Returns).

- Relationships Setup – Defined one-to-many relationships using primary and foreign keys.

- Hierarchies – Created drill-down paths (e.g., Year → Quarter → Month and Category → Subcategory → Product).

- DAX Measures – Developed KPIs like Total Sales, Profit, Return Rate, Profit Margin, and Revenue Growth %.

- Normalization – Separated lookup data to reduce redundancy and improve efficiency.

- Validation – Tested relationships and data flow for consistency and accuracy.

- Optimization – Reduced columns, used numeric keys, and applied summarization for better performance.

- Documentation – Recorded table structures, logic, and measure definitions for future reference.

  This model ensures seamless data integration, reliable analysis, and interactive reporting across all key business dimensions.
---
### Exploratory Data Analysis
  
  #### Adventure Works Business Problem Statement
- Declining Monthly Revenue Trends — Identify when and why sales performance drops over time.

- Low Profit Margins — Detect underperforming products and regions reducing profitability.

- High Return Rates — Determine which product types or categories experience excessive returns.

- Product Demand Forecasting — Analyze order trends to optimize inventory and production planning.

- Uneven Regional Performance — Reveal which countries or continents drive or lag in revenue generation.

- Customer Retention Challenges — Understand customer purchase frequency and lifetime value.

- Unbalanced Product Portfolio — Discover whether certain categories dominate orders or profits disproportionately.

- Inefficient Pricing Strategies — Track the impact of price adjustments on revenue and profit trends.

- Top and Low-Performing Products — Pinpoint best-selling and least-profitable items for decision-making.

- Profit Volatility Across Periods — Evaluate how profit trends fluctuate across months or years.

- Customer Segmentation Gaps — Identify purchasing patterns based on income level and occupation.

- Underperforming Sales Regions — Highlight regions that fall below revenue or order targets.

- Unclear Product Return Causes — Analyze return data to improve quality control and customer satisfaction.

- Revenue Concentration Risk — Identify dependence on a few top customers or product lines.

- Ineffective Marketing Targeting — Use demographic insights to better align campaigns with high-value segments.


--- 
### Key Insights

The analysis results and findings from the AdventureWorks Power BI report are summarized as follows:

#### Strong Financial Performance:
Total revenue of $24.9M and profit of $10.5M indicate consistent business growth and efficient operations.

#### Category Performance:
Accessories drive the highest sales volume, while Bikes contribute the most to total revenue, creating a balanced product portfolio.

#### Top Products:
Water Bottle – 30 oz., Sport-100 Helmets, and Fender Set – Mountain lead in both sales and profitability, supported by low return rates.

#### Profitability Trends:
Revenue continues to rise (+3.31% MoM), with minor order fluctuations (−0.88%) and stable return rates (+1.78%), signaling healthy demand and product quality.

#### Geographic Insights:
The US (39%) and Australia (30%) are the strongest markets, with significant contributions also from Europe (31%) — reflecting global market reach.

#### Customer Insights:
AdventureWorks serves 17.4K customers, averaging $1.43K revenue per customer.
High-income customers yield higher profitability, while lower-income groups contribute to sustained volume.

#### Product Profitability Focus:
Products like Mountain Tire Tube show high profit growth but declining adjusted margins, suggesting a need for cost and pricing optimization.

 

#### Overall Performance:  Adventureworks maintains steady growth, strong customer diversity, and a global sales balance, Making it well-positioned for continued expansion and market leadership
---
### Recommendations and Strategic Impact

Based on the analysis of AdventureWorks’ sales, profitability, and customer trends, the following strategic recommendations are proposed to enhance performance and accelerate growth over the next fiscal year.

####  1. Optimize Pricing and Margin Management

#####  Action:
Review pricing structures for mid-margin products (e.g., Mountain Tire Tube, Bikes) and implement dynamic pricing models using sales elasticity and competitor benchmarks.
######  Expected Impact:

- Improve overall profit margin by 5–8%, translating to an estimated $0.5M–$0.8M increase in annual profit.

- Stabilize adjusted profit fluctuations by aligning prices with demand cycles.

###  2. Expand High-Performing Product Lines

####  Action:
Increase production and marketing investment for top-selling items such as Sport-100 Helmets and Water Bottle – 30 oz., while phasing out low-yield SKUs.
###### Expected Impact:

- Drive an additional 8–10% growth in total revenue, adding approximately $2.0M–$2.5M annually.

- Reduce product return rates by maintaining focus on proven, customer-approved items.

#### 3. Strengthen Customer Segmentation and Retention

##### Action:
Deploy personalized loyalty programs targeting high-income and professional customers while offering bundle discounts to low-income segments.
###### Expected Impact:

- Increase repeat purchase rates by 12–15%.

- Boost customer lifetime value (CLV) by 10%, equivalent to roughly $1.4M in incremental revenue from returning customers.

#### 4. Geographic Market Expansion

##### Action:
Leverage growth momentum in the Pacific region (currently 30% of global revenue) by expanding distribution and targeted campaigns in Australia and New Zealand.
######  Expected Impact:

- Achieve 6–8% overall revenue growth, adding approximately $1.8M–$2.0M in new market sales.

- Diversify regional risk by reducing overreliance on North America from 39% to about 35% of total revenue.

#### 5. Invest in Data-Driven Marketing and Analytics

##### Action:
Adopt predictive analytics in Power BI and CRM tools to forecast demand, optimize campaigns, and identify cross-sell opportunities.
###### Expected Impact:

- Improve marketing ROI by 20–25% through smarter audience targeting.

- Contribute an estimated $1.0M uplift in annual revenue via conversion improvements and reduced campaign waste.

#### 6. Supply Chain and Return Optimization

##### Action:
Refine inventory forecasting and strengthen supplier coordination to minimize product returns and stockouts.
###### Expected Impact:

- Reduce return rate from 2.2% to 1.5%, saving roughly $175K annually in lost sales and logistics costs.

- Enhance on-time delivery performance by 10%, improving customer satisfaction scores.

#### Overall Business Impact

Implementing these recommendations collectively could yield:

- 10–15% increase in total annual revenue (~$2.5M–$3.7M)

- 5–7% improvement in net profit margin (~$0.5M–$0.7M gain)

- Enhanced customer retention, market diversification, and operational efficiency

These initiatives position AdventureWorks for sustained growth, higher profitability, and stronger global competitiveness in the upcoming fiscal year.

### References 
- Microsoft Power BI Desktop for Business Intelligence

[Udemy](https://www.udemy.com/course/microsoft-power-bi-up-running-with-power-bi-desktop/learn)



---
©️`Project by PATRICK OKOSUN`| Data Analyst | Power Bi Developer |

| Excel | SQL | DAX | POWER BI | TABLUE |

😄


























  
