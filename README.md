# 🏠 Airbnb NYC Data Analytics Project

## 📌 Project Overview

An end-to-end **Data Analytics & Business Intelligence project** using **Power Query, DAX, and Power BI** to analyze Airbnb NYC booking and listing data.

The project covers data cleaning, SQL analysis, data modeling, KPI development, and interactive dashboard reporting to understand **revenue, occupancy, pricing, bookings, hosts, properties, and neighborhood performance**.

---

## 🗂️ Dataset Overview

| Item | Details |
|---|---|
| Booking Records | 100,000+ |
| Properties | 80 |
| Hosts | 50 |
| Neighborhoods | 20 NYC Neighborhoods |
| Period | Jan 2023 – Dec 2024 |
| Fact Table | `fact_bookings` |
| Dimension Tables | `dim_host`, `dim_property`, `dim_location`, `dim_date` |

### Source Tables

- `fact_bookings` – Booking, pricing, review, and availability data
- `dim_host` – Host information and Superhost status
- `dim_property` – Property and room-type details
- `dim_location` – NYC neighborhood information
- `dim_date` – Date and calendar attributes

---

## 🔄 Data Cleaning & Processing

The data was cleaned and prepared using **Power Query** before analysis.

Key transformations included:

- Handling missing host names and bedroom values
- Standardizing host response rates and month names
- Cleaning currency-formatted price values
- Removing invalid review scores
- Removing invalid minimum-night values
- Handling invalid availability values
- Removing duplicate booking IDs
- Correcting whitespace and data types
- Creating a dedicated Date Table
- Implementing a **Star Schema** in Power BI

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power Query** | Data cleaning and transformation |
| **Power BI** | Dashboard development and visualization |
| **DAX** | KPI and business calculations |
| **Star Schema** | Data modeling |

---

## 📊 Power BI Dashboard

The report contains **2 interactive pages** covering overall business performance and detailed property/host analysis.

### Key KPIs

| KPI | Current | Previous Year | Change |
|---|---:|---:|---:|
| **Total Revenue** | **$176.08M** | $119.48M | **+47.4%** |
| **Avg Nightly Rate** | **$235.56** | $236.20 | -0.3% |
| **Occupancy Rate** | **48.8%** | 48.9% | -0.1 pts |
| **Avg Review Score** | **3.92** | 3.92 | Stable |
| **Cancellation Rate** | **20.0%** | 19.8% | +0.2 pts |

---

## 🔎 Key Analysis & Findings

- **Revenue reached $176.08M**, showing a 47.4% increase versus the comparison period.
- Revenue growth occurred while **Average Nightly Rate remained almost flat**, indicating the need to examine booking volume, inventory, and property mix.
- **Occupancy remained stable at 48.8%**, with monthly occupancy ranging approximately from 47.6% to 49.4%.
- **Entire home/apt** generated the largest share of bookings at approximately **56.16%**.
- The **Bronx** recorded the highest displayed neighborhood booking volume at approximately **12.6K**.
- In the 2024 dashboard view, **Superhosts accounted for 74.12% of bookings and 72.42% of revenue**.
- Host performance varies when comparing **booking volume, revenue, review score, and revenue per booking**.
- RevPAR and Average Nightly Rate analysis helps evaluate the relationship between **pricing and property utilization**.

---

## 📈 Key DAX & Analytics Concepts

- `CALCULATE`
- `VAR`
- `DIVIDE`
- `DATEADD`
- `SAMEPERIODLASTYEAR`
- `DATESYTD`
- Month-over-Month (MoM) Analysis
- Year-over-Year (YoY) Analysis
- Previous Year Comparisons
- KPI Variance Analysis
- Conditional Formatting
- Time Intelligence

---

## 🧠 What I Learned

- Performing end-to-end data analysis using **Power BI**
- Cleaning real-world data-quality issues using **Power Query**
- Designing a scalable **Star Schema**
- Developing reusable **DAX measures**
- Building interactive KPI dashboards
- Performing time-based and segment-level analysis
- Translating analytical results into meaningful **business insights**

---

## 📁 Project Structure

```text
Airbnb-Data-Analytics/
│
├── Dataset/
│   ├── fact_bookings.csv
│   ├── dim_host.csv
│   ├── dim_property.csv
│   ├── dim_location.csv
│   └── dim_date.csv
│
├── SQL/
│   └── Airbnb_Analysis.sql
│
├── PowerBI/
│   └── Airbnb_NYC_Analytics.pbix
│
├── Documentation/
│   └── Airbnb_Data_Analytics_Report.pdf
│
└── README.md

---

## 🚀 Project Workflow

```text
Raw CSV Data
     ↓
PgSQL / PostgreSQL
     ↓
Data Exploration & SQL Analysis
     ↓
Power Query
     ↓
Data Cleaning & Transformation
     ↓
Star Schema Data Model
     ↓
DAX Measures
     ↓
Power BI Dashboard
     ↓
Business Insights

