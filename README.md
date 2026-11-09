# Hotel Booking Analytics Platform

## Project Overview
This project analyzes hotel booking data using Databricks and the Medallion Architecture. It transforms raw booking data into clean, business-ready data and presents insights through a Databricks AI/BI Dashboard.

## Tools & Technologies
- Databricks
- Lakeflow Spark Declarative Pipelines
- Apache Spark / PySpark
- SQL
- Unity Catalog
- Databricks AI/BI Dashboard

## Dataset
- File: `hotel_bookings_raw.csv`
- Original records: 1,316
- Columns: 20
- Data includes hotel bookings, dates, room rates, discounts, booking channels, and customer details.

## Medallion Architecture

### Bronze Layer
- Loaded the raw CSV dataset into Databricks.
- Stored 1,316 records in the Bronze table.

### Silver Layer
- Cleaned and transformed booking data.
- Removed duplicate records.
- Separated clean and rejected records.

Tables:
- `silver_bookings_clean` – 1,269 records
- `silver_bookings_rejected` – 21 records

Duplicate records removed: 26

### Gold Layer
Created business summary tables:
- `gold_monthly_bookings`
- `gold_hotel_summary`
- `gold_room_type_summary`
- `gold_channel_summary`
- `gold_data_quality`

## Data Reconciliation

Bronze Records = Clean Records + Rejected Records + Duplicate Records Removed

1,316 = 1,269 + 21 + 26

Reconciliation: Passed

## Dashboard
Created a Databricks AI/BI Dashboard with three pages:

1. Overview
2. Hotel, Room & Channel Analysis
3. Data Quality

The dashboard presents booking performance, revenue trends, hotel comparisons, room-type analysis, channel performance, and data quality metrics.

## Key Project Outcomes
- Implemented Bronze, Silver, and Gold layers.
- Separated clean and rejected booking records.
- Removed duplicate records.
- Created five Gold summary tables.
- Built a three-page analytics dashboard.

## Author
Bandi Pavani

Data Analytics Learner | Innomatics Research Labs