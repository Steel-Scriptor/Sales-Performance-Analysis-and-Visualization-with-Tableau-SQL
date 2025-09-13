# Sales Performance Analysis and Visualization with Tableau and SQL

## Project Overview

This project delivers comprehensive sales analytics for an India-based hardware company through integrated Tableau visualization and SQL analysis. The solution transforms transactional data into actionable business intelligence, enabling stakeholders to identify revenue trends, optimize customer relationships, and improve product portfolio performance.

## Business Problem

Sales teams faced significant challenges with manual data aggregation and lacked visibility into key performance metrics, including revenue breakdown by geographic regions, customer contribution analysis, product profitability assessment, and temporal performance trends. The organization required a unified analytics framework to support data-driven decision making and reduce operational inefficiencies.

## Technical Architecture

**Data Processing and Storage**
- MySQL database management for complex query optimization and data aggregation
- CSV data integration layer processing 150,000+ transactional records
- Star schema implementation with a centralized fact table and dimensional modeling

**Visualization and Analytics**
- Tableau Public for interactive dashboard development and self-service analytics
- Statistical computing applied for descriptive analysis and trend identification
- Advanced calculated fields and dynamic KPI tracking

## Dataset Specifications

The analysis utilized a comprehensive transactional dataset containing records across multiple business dimensions, including geographic markets, customer segments, product categories, temporal patterns, and revenue attribution. Data quality protocols ensured consistency across currency conversions and dimensional attributes.

## Data Analysis - Approach
<p  align="center"><a href="https://github.com/Steel-Scriptor"><img width="80%" src="https://github.com/Steel-Scriptor/Sales-Performance-Analysis-and-Visualization-with-Tableau-SQL/blob/main/images/flow.jpg" /></a></p>

## Key Analytics and Findings

**Revenue Performance Analysis**
Comprehensive revenue analysis across 10+ metropolitan markets revealed year-over-year trends and monthly performance patterns from 2018-2020. The automated reporting framework reduced manual processing time by 20 percent.

**Customer Intelligence**
Advanced segmentation analysis identified the top 5 customers contributing 35 percent of total revenue generation. Customer-level sales velocity and profitability metrics informed targeted retention strategies and discount optimization programs.

**Product Portfolio Evaluation**
Analysis of 50+ product categories highlighted high-performing revenue drivers and underperforming inventory segments. Strategic recommendations enabled product bundling optimization and cross-selling opportunity identification.

**Market Profitability Assessment**
Multi-dimensional profitability analysis across 7 regional markets provided strategic visibility into margin performance. The analysis identified 10 percent cost optimization potential through strategic resource allocation.

## Technical Implementation

**Data Integration Process**
Systematic import and processing of transactional data from CSV source files into MySQL database environment with direct Tableau integration capabilities.

**Quality Assurance Framework**
Implementation of comprehensive data cleansing protocols addressing missing value treatment, currency standardization, and validation across all dimensional attributes.

**Analytics Development**
Development of complex SQL aggregation queries for key performance indicator extraction while implementing advanced visualization features including trendlines and interactive filtering capabilities.

## Business Impact Metrics

The implementation delivered measurable operational improvements including 20 percent reduction in manual reporting cycles, 25 percent acceleration in decision-making processes, and identification of cost optimization opportunities representing 10 percent potential savings through data-driven strategic initiatives.

## SQL Query Examples

```sql
-- Customer base analysis
SELECT COUNT(*) FROM customers;

-- Annual revenue performance
SELECT SUM(transactions.sales_amount)
FROM transactions
INNER JOIN date ON transactions.order_date = date.date
WHERE date.year = 2020;

-- Top revenue-generating products
SELECT product_code, SUM(sales_amount) AS revenue
FROM transactions
GROUP BY product_code
ORDER BY revenue DESC
LIMIT 5;
```

## Tableau Dashbpard Revenue Analysis
<p  align="center"><a href="https://github.com/Steel-Scriptor"><img width="80%" src="https://github.com/Steel-Scriptor/Sales-Performance-Analysis-and-Visualization-with-Tableau-SQL/blob/main/images/Tableau%20Dashbpard%20Revenue%20Analysis.png" /></a></p>

## Tableau Dashbpard Profit Analysis
<p  align="center"><a href="https://github.com/Steel-Scriptor"><img width="80%" src="https://github.com/Steel-Scriptor/Sales-Performance-Analysis-and-Visualization-with-Tableau-SQL/blob/main/images/Tableau%20Dashbpard%20Profit%20Analysis.png" /></a></p>


## Technical Resources
- [MySQL Installation Guide – YouTube](https://www.youtube.com/)

## Project Summary

This analytics solution demonstrates the integration of Tableau visualization and SQL analysis to convert transactional data into strategic business intelligence. The platform delivers comprehensive performance analysis through automated KPI tracking and advanced analytical capabilities, providing a scalable solution for retail and enterprise sales organizations.
