# Payments-Accounting-Data-Analytics
Company: Booking Holdings India Private Limited,Payments Accounting Data Analytics Team ,To leverage data to solve business problems in the payments accounting domain.  To generate insights, perform root cause analysis, create reports, reconcile data, and support stakeholders. it’s insight generation + stakeholder consulting + big data analysis.

As a DATA ANALYST: who can own the analytics process with minimal supervision.
A problem solver who can turn business needs into data-driven solutions.
A person with hands-on technical skills (SQL, Python, ETL, Visualization).
A strong communicator who can influence stakeholders using data storytelling.


-Business Context
Domain: Payments & Accounting (work with transaction, reconciliation, and financial data).
Impact: Your insights will influence operational, tactical, and strategic decisions.
Team Type: Cross-functional, involving analytics + finance + business stakeholders.

-Key Responsibilities 
Independent Work:
Collect and prepare data.
Analyze data and generate insights.
Conduct root cause analysis autonomously.

Collaboration & Communication:
Communicate findings clearly to stakeholders.
Participate in team activities (standups, planning, retrospectives).
Network beyond immediate team scope.

Technical Responsibilities:
Work with big data platforms (Snowflake, AWS).
Maintain key reports, metrics, and workflows.
Perform data reconciliation and ensure data quality.

a realistic synthetic payments + reconciliation dataset and saved three CSVs 
 transactions.csv — 5,000 transaction rows, with fields for amounts, fees, tax, ledger values, reconciliation status, settlement dates, payment method, gateway, merchant, customer, processing times, etc.
 customers.csv — customer dimension (800 rows).
 merchants.csv — merchant dimension (60 rows).


data dictionary / key columns:-
Transaction_id — unique transaction identifier
Transaction_date, settlement_date, settlement_days — timestamps / lag
merchant_id, merchant_name, region, country, category — merchant dimensions
customer_id — customer dimension
amount, fee, tax, net_amount — financial fields
ledger_amount — accounting ledger value (may differ slightly from net_amount)
reconciliation_status — matched / unmatched (computed)
status — success / refunded / chargeback / failed
refund_amount, dispute_id — refund/chargeback info
payment_method, card_type, payment_gateway — payment rails data
processing_time_seconds, batch_id, invoice_id, product_id
created_at, updated_at

# Payments Accounting Data Analytics Dashboard

## Overview
This project provides a **comprehensive Payments Accounting Dashboard** built using **Power BI**,
designed to monitor transactions, revenue, chargebacks, and reconciliation health.

## Dataset
- **transactions.csv** – Payment transactions (5000 rows)
- **customers.csv** – Customer dimension (800 rows)
- **merchants.csv** – Merchant dimension (60 rows)

## Key Metrics
- **Total Amount**: ₹383,428
- **Net Revenue**: ₹352,787
- **Chargeback Rate**: 2%
- **Unmatched Transactions**: 179 (₹23,787 mismatch)

## Features
- **Interactive filters**: Date, Region, Payment Gateway, Payment Method
- **Reconciliation module**: Highlights unmatched transactions 
- **Chargeback hotspot analysis**
- **Top merchants & categories breakdown**

## Tools & Tech
- **Power BI**: DAX, Star Schema, Conditional Formatting
- **SQL**: Data extraction & preprocessing
- **Python**: Synthetic data generation
- **Airflow & dbt**: Optional ETL pipeline

## How to Use
1. Download the CSVs from `/data`.
2. Open `Payments_Accounting.pbix` in Power BI Desktop.
3. Connect to your database or refresh the sample data.
4. Explore dashboards: Executive Overview, Payment Health, Reconciliation.

## Insights
- Travel & Accommodation lead in payment volume.
- Chargebacks higher in France & Japan.
- Automated reconciliation potential: ₹23K flagged for review.

## Author
Lavanya – Data Analyst (Payments & Accounting Analytics)



Data Storytelling – Payments Accounting Dashboard
1. Objective
The analysis aims to:Monitor total payments volume, net revenue, chargeback rates, and reconciliation mismatches.

Provide actionable insights for payments accounting & finance teams.
Identify unmatched transactions, high-risk merchants, and optimize payment gateways.

2. Key Highlights (Executive Summary)
Total Amount Processed: ₹383,428
Net Revenue: ₹352,787
Chargeback Rate: 2% – within acceptable range but with country-level variance.
Unmatched Count: 179 transactions, total mismatch amount ~₹23,787.

3. Geographic Insights
Top Performing Countries (Net Revenue):
Canada: ₹61K
United States: ₹46K
Singapore: ₹33K
Chargeback Hotspots:
France (3.4%)
Japan (3.2%)
India (2.2%)

Action: Focus fraud prevention & dispute management in high chargeback regions.
4. Category & Loyalty Insights

Top Categories by Total Amount:
Travel: ₹108K
Accommodation: ₹106K
Retail: ₹83K
Top Loyalty Tiers:
Gold: ₹105K
Platinum: ₹98K

Action: High-spend loyalty tiers (Gold/Platinum) show strong engagement — consider exclusive payment offers.
5. Payment Gateway & Method Analysis
Payment Gateway Distribution: GatewayA (24K), GatewayB (23K), GatewayC (18K)
Payment Method: Cards dominate (100%) — UPI/wallet adoption is low (potential growth area).

Action: Optimize routing rules between GatewayA & GatewayB during peak months (June, August, September).
6. Reconciliation & Risk
Mismatch Amount: ₹23,787
Refund Amount: ₹1,228

Top unmatched merchants include Merchant_31, Merchant_44, Merchant_60.

Action: Investigate these merchants’ settlements and implement auto-reconciliation rules.
7. Recommendations
Automate reconciliation using thresholds (>₹0.50 mismatch flag).
Deploy chargeback alerts in France & Japan.
Introduce UPI & wallet promotions to diversify payment mix.
Refine loyalty tier campaigns for high-value segments.





Payments Accounting Data Analytics Dashboard
Power up your financial insights with a fully built and professionally designed Power BI dashboard—ideal for analysts, business users, and students eager to showcase their analytic capabilities.

 What's Inside
1. Modular Dashboard for Multifaceted Insights
Navigate through structured sections tailored to enterprise and accounting needs:
Executive Summary: Instant access to key metrics like total processed payments, net revenue, chargeback rate, and reconciliation mismatches.
Payments Health: Visualize trends and breakdowns across payment methods (cards, UPI, wallets) and gateways.
Reconciliation & Root-Cause: Drill into mismatches, dispute reasons, and flagged transactions—all with precision.

2. Interactive, Dynamic Filters
Tailor your analysis in real time:
Date Range Filtering: Day, month, quarter, year-to-date, custom periods.
Segment-Level Views: Filter by Region, Merchant, Payment Gateway, Status (e.g. Chargeback), Reconciliation Status.

3. Advanced Visual Storytelling
Experience responsive, user-driven visuals:
KPI Cards: Strategically placed for rapid executive insights.
Trend Lines & Combo Charts: Seamlessly analyze revenue, mismatches, and volume over time.
Heatmaps & Geomaps: Highlight regional chargeback risk and reconciliation hotspots.
Drillthrough Tables: Interactive unmatched transaction listings with conditional formatting (mismatch > ₹0.50 highlighted).

4. Workflow-Ready Navigation
Easily switch between pages: Overview → Payments Breakdown → Reconciliation Drilldown. Designed for fluid interaction and stakeholder demos.

5. Ready to Impress
Ideal for enhancing portfolios, team presentations, or academic showcases:
Clear, business-focused design
Story-driven layout, aligning visuals with financial risk & revenue themes
Export-ready visuals—perfect for stakeholder deliverables.
Perfect For...
Business Analysts & Finance Teams: Quickly uncover insights from reconciliation to net revenue.
Data Professionals: Showcase your mastery of DAX, Power BI modeling, and storytelling capabilities.
Students & Learners: A comprehensive, real-world project to sharpen your analytics skills end-to-end.
