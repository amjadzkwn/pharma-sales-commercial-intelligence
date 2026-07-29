# 💊 Pharma Sales & Commercial Intelligence Hub

![Power BI](https://img.shields.io/badge/Power_BI-Business_Intelligence-F2C811?style=for-the-badge&logo=powerbi)
![SQL](https://img.shields.io/badge/SQL-Analytics-blue?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-ETL-yellow?style=for-the-badge&logo=python)
![Excel](https://img.shields.io/badge/Microsoft_Excel-Reporting-green?style=for-the-badge&logo=microsoft-excel)

An end-to-end **Sales & Commercial Intelligence** project built for a pharmaceutical company to demonstrate practical **Data Analyst**, **Sales Analyst**, and **Business Intelligence** skills using **Power BI, SQL, Excel, Python, Power Query, and DAX**.

The solution transforms raw sales data into actionable business insights by monitoring sales performance, campaign effectiveness, quotation and tender pipeline, customer behavior, territory performance, and data quality.

---

# 📌 Business Scenario

A pharmaceutical company sells products through hospitals, clinics, pharmacies, and distributors across multiple territories.

Management currently faces several challenges:

- Sales data is stored across multiple files and departments.
- Sales performance is difficult to monitor.
- Quotation and tender follow-ups are not centralized.
- Campaign effectiveness cannot be measured accurately.
- Management lacks real-time visibility into KPIs.
- Manual Excel reporting consumes significant time every month.
- Data quality issues affect reporting accuracy.

The company requires a centralized commercial intelligence solution that supports better decision-making through automated reporting and interactive dashboards.

---

# 🎯 Project Objectives

This project aims to:

- Monitor sales performance across representatives, products, customers, and territories.
- Compare actual sales against monthly targets.
- Analyze product demand and customer purchasing behavior.
- Evaluate promotional campaign effectiveness.
- Track quotation and tender conversion.
- Monitor overdue follow-up activities.
- Improve reporting accuracy through data validation.
- Build executive dashboards for management.
- Generate actionable business recommendations.

---

# 🛠 Technology Stack

| Category | Tools |
|----------|------|
| Business Intelligence | Power BI |
| Database | SQL |
| Data Cleaning | Python, Power Query |
| Spreadsheet Analysis | Microsoft Excel |
| ETL | Python |
| Data Visualization | Power BI |
| Dashboard Design | Power BI |
| Version Control | GitHub |

---

# 📊 Dataset Overview

The project uses **synthetic pharmaceutical sales data** created specifically for portfolio purposes.

**No real customer, patient, or confidential company information is included.**

Dataset includes approximately:

| Dataset | Records |
|----------|---------|
| Sales Transactions | 3,200 |
| Customers | 180 |
| Products | 18 |
| Sales Representatives | 12 |
| Campaigns | 12 |
| Quotations & Tenders | 320 |
| Sales Targets | 216 |
| Sales History | 18 Months |

---

# 📂 Project Structure

```text
pharma-sales-commercial-intelligence/

│
├── README.md
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── excel/
│   └── Pharma_Sales_Commercial_Intelligence.xlsx
│
├── sql/
│   ├── 01_create_schema.sql
│   ├── 02_analysis_queries.sql
│   └── 03_data_quality_checks.sql
│
├── python/
│   └── etl_pipeline.py
│
├── powerbi/
│   ├── Pharma_Sales_Dashboard.pbix
│   ├── measures.dax
│   └── PowerBI_Setup_Guide.md
│
├── dashboard/
│   ├── 01_Executive_Overview.png
│   ├── 02_Sales_Rep_Performance.png
│   ├── 03_Product_Customer_Territory.png
│   ├── 04_Campaign_Performance.png
│   ├── 05_Quotation_Tender.png
│   └── 06_Data_Quality.png
│
└── documentation/
    ├── business_requirements.md
    ├── data_dictionary.csv
    ├── data_model.png
    └── project_report.pdf
```

---

# 🗂 Data Model

The project follows a **Star Schema** for efficient reporting and analysis.

```text
                 dim_date
                     │
dim_customer ────────┐
                     │
dim_product ─────────┤
                     │
dim_sales_rep ───────┤
                     │
dim_territory ───────┤
                     │
               fact_sales
                     │
                     ├──────── fact_sales_target
                     │
                     ├──────── fact_campaign_performance
                     │
                     └──────── fact_quotation_tender
```

This model improves:

- Query performance
- DAX calculation efficiency
- Dashboard responsiveness
- Data consistency

---

# 🧹 Data Cleaning & Validation

The ETL pipeline performs the following validation steps:

- Remove duplicate invoices
- Standardize customer names
- Standardize territory names
- Validate product IDs
- Validate customer IDs
- Convert data types
- Remove invalid sales records
- Validate quotation dates
- Check missing values
- Check negative sales
- Validate quotation status
- Validate converted invoices

The cleaned datasets are exported into **Power BI-ready CSV files**.

---

# 💻 SQL Analytics

SQL is used to perform business analysis including:

- Sales by representative
- Sales by territory
- Product performance
- Customer contribution
- Monthly sales growth
- Campaign analysis
- Quotation pipeline
- Tender tracking
- Win rate analysis
- Data quality validation

SQL concepts demonstrated:

- INNER JOIN
- LEFT JOIN
- GROUP BY
- CASE WHEN
- Common Table Expressions (CTE)
- Window Functions
- LAG()
- RANK()
- NULLIF()
- Aggregate Functions

---

# 📈 Power BI Dashboard

The report contains **6 interactive dashboard pages**.

---

# 1️⃣ Executive Overview

Provides a high-level summary of business performance.

### KPIs

- Total Sales
- Gross Profit
- Gross Margin
- Sales Growth
- Active Customers
- Target Achievement
- Average Order Value

### Visuals

- Monthly Sales vs Target
- Sales by Territory
- Sales by Product Category
- Sales by Customer Type
- Top Products
- Top Sales Representatives
- Management Alerts

---

## Dashboard Preview

> Replace with screenshot after dashboard is completed.

```markdown
![Executive Overview](dashboard/01_Executive_Overview.png)
```

---

# 2️⃣ Sales Representative Performance

Evaluates sales representative productivity.

### KPIs

- Total Sales
- Target Achievement
- Active Customers
- Average Order Value
- Quotation Win Rate

### Visuals

- Sales Rep Ranking
- Actual vs Target
- Monthly Sales Trend
- Performance Quadrant
- Product Matrix
- Performance Table

---

```markdown
![Sales Rep Performance](dashboard/02_Sales_Rep_Performance.png)
```

---

# 3️⃣ Product, Customer & Territory Analysis

Analyzes sales performance across products and customers.

### KPIs

- Products Sold
- Active Customers
- Total Territories
- Sales per Customer

### Visuals

- Product Sales Trend
- Product Category Contribution
- Customer Segmentation
- Territory Map
- Top Customers
- Territory Performance
- Heatmap Matrix

---

```markdown
![Product Customer Territory](dashboard/03_Product_Customer_Territory.png)
```

---

# 4️⃣ Campaign Performance

Measures marketing effectiveness.

### KPIs

- Campaign Cost
- Attributed Sales
- Campaign ROI
- Conversion Rate
- Customers Converted
- Cost per Conversion

### Visuals

- ROI Ranking
- Campaign Funnel
- Spend vs Sales
- Campaign Trend
- Product Campaign Analysis
- Campaign Detail Table

---

```markdown
![Campaign Performance](dashboard/04_Campaign_Performance.png)
```

---

# 5️⃣ Quotation & Tender Pipeline

Monitors commercial opportunities.

### KPIs

- Open Pipeline
- Weighted Pipeline
- Win Rate
- Average Days to Close
- Lost Opportunity Value
- Overdue Follow-ups

### Visuals

- Pipeline Funnel
- Pipeline by Sales Representative
- Opportunity Trend
- Quotation vs Tender
- Aging Analysis
- Follow-up Table

---

```markdown
![Quotation Tender](dashboard/05_Quotation_Tender.png)
```

---

# 6️⃣ Data Quality Dashboard

Ensures reporting integrity.

### KPIs

- Data Quality Score
- Duplicate Records
- Missing Values
- Invalid Product IDs
- Negative Sales
- Last Refresh

### Visuals

- Quality Issues
- Data Source Summary
- Error Trend
- Validation Results
- Records Loaded

---

```markdown
![Data Quality](dashboard/06_Data_Quality.png)
```

---

# 📑 Excel Reporting

The project also includes an advanced Excel workbook featuring:

- Interactive Dashboard
- Sales Transactions
- Quotation Tracker
- Tender Tracker
- Follow-up Tracker
- Campaign Summary
- Customer Master
- Product Master
- Sales Representative Master
- Monthly Sales Target
- Data Quality Report

Excel skills demonstrated:

- Power Query
- XLOOKUP
- Pivot Tables
- Pivot Charts
- Conditional Formatting
- Data Validation
- Dynamic Dashboard

---

# 🐍 Python ETL Pipeline

Python automates the entire data preparation process.

Workflow:

```text
Raw CSV Files
      │
      ▼
Python ETL
      │
      ▼
Data Validation
      │
      ▼
Data Cleaning
      │
      ▼
Export Clean Dataset
      │
      ▼
Power BI Dashboard
```

Python libraries used:

- pandas
- numpy
- openpyxl

---

# 📈 Key Business Insights

Example insights generated from the dashboard:

### Insight 1

Central Territory generated the highest total sales, while Northern Territory recorded the fastest growth rate, indicating strong future expansion potential.

### Insight 2

Several sales representatives managed a large customer portfolio but remained below their monthly sales targets, suggesting opportunities to improve product mix and sales effectiveness.

### Insight 3

A significant proportion of open quotation value was concentrated among a small number of strategic customers, highlighting the importance of timely follow-up.

### Insight 4

Some promotional campaigns generated high sales but delivered relatively low ROI because of higher campaign costs.

### Insight 5

Overdue quotation follow-ups represented unrealized revenue opportunities that should be prioritized by the sales team.

---

# 💡 Business Recommendations

Based on the analysis:

- Prioritize overdue quotation follow-ups with the highest weighted pipeline value.
- Increase investment in high-growth territories.
- Coach underperforming sales representatives.
- Review campaign spending against conversion performance.
- Conduct weekly commercial pipeline review meetings.
- Monitor data quality before monthly reporting.

---

# 🚀 Skills Demonstrated

## Business Intelligence

- Executive Dashboard Design
- KPI Development
- Business Reporting
- Dashboard Storytelling

## Power BI

- Data Modeling
- DAX
- Drill-through
- Interactive Filters
- Bookmarks
- Conditional Formatting

## SQL

- Analytical Queries
- Window Functions
- Ranking
- Data Validation
- Aggregation

## Excel

- Power Query
- Pivot Tables
- XLOOKUP
- Dashboard Design
- Reporting Automation

## Python

- ETL
- Data Cleaning
- Validation
- Automation

---

# ▶️ How to Run the Project

## Power BI

1. Open `Pharma_Sales_Dashboard.pbix`
2. Update CSV source path if required.
3. Refresh the model.

## Excel

Open:

```text
excel/Pharma_Sales_Commercial_Intelligence.xlsx
```

## Python

```bash
pip install -r requirements.txt

python python/etl_pipeline.py
```

---

# 📌 Resume Project Description

**Pharma Sales & Commercial Intelligence Hub**

Developed an end-to-end pharmaceutical sales analytics solution using **Power BI, SQL, Excel, and Python**. Built interactive dashboards to monitor sales representatives, product performance, territory analysis, campaign ROI, quotation conversion, and commercial pipeline while implementing automated ETL processes and data quality validation to support management decision-making.

---

# 👨‍💻 Author

**Muhammad Amjad Zakwan**

Bachelor of Computer Science (Hons.) in Data Science  
Universiti Malaysia Sabah

**Available for full-time opportunities from September 2026**

LinkedIn: *(Add your LinkedIn URL)*

Portfolio: *(Add your Portfolio URL)*

GitHub: *(Add your GitHub URL)*

---

# 📄 License

This repository is intended for **educational and portfolio purposes only**.

All datasets are **synthetically generated** and do not represent any real company, customer, or patient information.
