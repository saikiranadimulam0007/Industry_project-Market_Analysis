📊 Market Data Analytics – Price Challenge Reporting
📌 Project Overview

The Market Data Analytics Price Challenge Reporting project focuses on designing and implementing a scalable analytics solution to compare and evaluate pricing data from multiple market data vendors.
Financial auditors depend on vendor market feeds that often differ due to proprietary pricing algorithms. This project helps identify deviations, outliers, and vendor reliability through statistical analysis and interactive dashboards.

🎯 Objectives

Process pricing data from multiple market data vendors

Clean, standardize, and transform heterogeneous financial datasets

Compute key statistical KPIs such as:

Median Price

Price Variation (%)

Standard Deviation

Identify pricing outliers and categorize deviations

Visualize insights using interactive Power BI dashboards

Generate a Price Challenge Report to support audit decisions

🏦 Business Problem

Market data vendors often provide inconsistent prices for the same security due to different valuation models.
Auditors need a standardized system to:

Compare vendor prices

Detect anomalies

Rank vendors based on data reliability

Enable corrective action and vendor feedback

🗂 Dataset Description

The dataset simulates real-world market pricing data with the following attributes:

Security ID (e.g., ISIN)

Vendor ID & Vendor Code

Source Feed ID

Price Type (Open, Close, Bid, Ask, Mid)

Exchange Code

Price Date

Currency Code

Security Price

Currency Conversion Rate (to USD)

The data covers multiple vendors, exchanges, feeds, and price types to replicate real auditing scenarios.

🛠 Tools & Technologies

Python: Pandas, NumPy (data cleaning & transformation)

SQL: Data aggregation and KPI computation

Power BI: Dashboard creation and visualization

Excel: Initial data collection and validation

Power BI Service: Cloud deployment and sharing

🔄 Methodology
Phase 1: Data Collection & Preprocessing

Collected pricing data from 5 vendors

Handled missing values and derived missing attributes

Removed duplicate records

Standardized data formats

Converted all prices to USD using currency conversion rates

Phase 2: KPI Calculation & Aggregation

Grouped data by:

Security ID

Vendor

Feed

Price Type

Exchange

Calculated:

Median Price

Price Variation (%)

Standard Deviation

Categorized deviations into outlier buckets:

0–3%

3–5%

>5%

Phase 3: Dashboard Development

Built interactive Power BI dashboards featuring:

Vendor performance comparison

Price deviation trends

Drill-through analysis (Date → Vendor → Security)

Dynamic filters for exchange, price type, date range

Used DAX measures for real-time analytics

Phase 4: Deployment

Published dashboards to Power BI Service

Enabled scheduled refresh

Shared secure access with stakeholders

Documented usage instructions

📈 Results & Insights

Identified vendors with high deviations (e.g., Vendor D with ~5.2% variation)

Bid/Ask prices showed higher volatility than Closing prices

Month-end refreshed data had lower deviations (<2%)

Certain exchanges (e.g., NYSE) showed higher pricing consistency

Outlier buckets simplified manual audit review

✅ Conclusion

This project successfully demonstrates:

Multi-vendor market data processing

Statistical KPI analysis

Business intelligence reporting

Real-world financial audit use case

The solution enables auditors to evaluate vendor accuracy, detect anomalies, and take corrective action, showcasing strong data engineering and analytics skills.

🚀 Future Enhancements

Real-time market data integration

Machine learning models for deviation prediction

Support for additional asset classes (bonds, derivatives, commodities)

Automated alerting for extreme price deviations

Reusable framework for other financial institutions

📚 References

TCS iON Industry Project Kit – Market Data Analytics Price Challenge Reporting

Microsoft Power BI Documentation

Python Statistical Libraries Documentation

Financial Data Auditing Standards

GeeksforGeeks – Data Warehousing & ETL Concepts

👤 Author

Adimulam Sai Kiran
TCS Industry Project (2024–2025)
