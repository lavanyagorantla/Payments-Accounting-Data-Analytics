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
- **Reconciliation module**: Highlights unmatched transactions (`> ₹0.50 mismatch`)
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

