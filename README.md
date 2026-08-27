# Supermarket Sales Analysis — Excel BI Solution

An end-to-end Business Intelligence solution built entirely in Excel — from raw transaction data to a fully modeled, interactive dashboard — using Power Query, Power Pivot, and DAX.

## Overview

This project turns 1,000+ raw supermarket transaction records into a reusable, interactive BI solution inside a single Excel workbook. Rather than relying on static formulas, the workbook is built around a proper ETL and data-modeling workflow: Power Query handles transformation and feature engineering, Power Pivot hosts a structured data model with DAX measures, and PivotTables/dashboards consume that model for reporting.

## Dataset

Transaction-level supermarket sales data (1,000 rows × 23 columns), including `Invoice ID`, `Branch`, `City`, `Customer type`, `Gender`, `Product line`, `Unit price`, `Quantity`, `Tax`, `Total`, `Date`, `Time`, `Payment` method, `COGS`, and `Gross Income`.

## Tools & Technologies

- **Power Query** — data transformation and feature engineering
- **Power Pivot / Data Model** — relational modeling and DAX measures
- **PivotTables & PivotCharts** — reporting layer
- **Excel Dashboards** — interactive, slicer-driven reporting

## Methodology

**1. Data Transformation (Power Query)**
Raw transaction data is cleaned and enriched with derived attributes:
- `Month Name`, `Day Name` (localized)
- `Is Weekend` flag
- `Week of Year`
- `Time of Day` bucket (Morning / Afternoon / Evening)
- `Profit Margin`

**2. Data Modeling (Power Pivot / DAX)**
The cleaned data feeds a Power Pivot data model with custom DAX measures, including:
- `Sum of Total` — total revenue
- `Average of Rating` — average customer satisfaction rating
- `Count of Invoice ID` — transaction volume
- `Sum of Quantity`, `Sum of Gross Income`

**3. Reporting Layer**
**22 PivotTables** are built on top of the data model, feeding **two interactive dashboards** with slicers covering:
- Sales by branch and city
- Product line performance
- Payment method breakdown
- Time-based trends (daily, weekly, time-of-day)

## Key Insights

- Sales performance varies meaningfully by branch/city and by time-of-day bucket, informing staffing and promotional timing.
- Certain product lines consistently outperform others in both revenue and gross income contribution.
- Payment method distribution and customer type (Member vs. Normal) show distinct purchasing patterns worth targeting separately.

## Dashboard 
<img width="1643" height="857" alt="home1" src="https://github.com/user-attachments/assets/b8c861fa-2323-4937-b91b-cef44e37a9f9" />

<img width="1893" height="920" alt="execel2" src="https://github.com/user-attachments/assets/ba462af1-6720-452d-86f6-e4e87c0fb543" />

## Repository Structure

```
Supermarket-Sales-Analysis/
├── Supermarket_Sales_Analysis.xlsx   # Data, Power Query, Power Pivot model, PivotTables, Dashboards
└── README.md
```

## How to Use

1. Download `Supermarket_Sales_Analysis.xlsx`.
2. Open in Excel (Power Query and Power Pivot require Excel 2016+ / Microsoft 365).
3. Explore the `Dashboard` and `Dashboard (2)` sheets, or inspect the `pivot tables` sheet and the underlying data model directly.

## Author

**Mohamed Wasef**
[LinkedIn](https://www.linkedin.com/in/mohamed-wasef-789743233/) · [GitHub](https://github.com/Mo7239)
