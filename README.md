# Sales Data Cleaning & Transformation — Power Query (Power BI)

## Overview
End-to-end data cleaning and transformation of a raw sales dataset using
Power Query in Power BI. The goal was to take a messy, real-world-style
dataset and prepare it for analysis by fixing missing values, inconsistent
formats, and data quality errors.

## Dataset
`SalesFile.xlsx` — raw sales data with units sold, pricing, discount bands,
and date fields.

## What I Did
- **Handled missing values**: Replaced NULLs in Units Sold, Sale Price,
  Sales, and Profit columns with 0
- **Fixed data types**: Converted Manufacturing Price, Sale Price, Sales,
  and Profit to Decimal Number; Units Sold and Month Number to Whole Number
- **Cleaned inconsistent entries**: Corrected invalid values in Discount
  Band (e.g. stray "1" → "None") and Units Sold (text "six hundred" → 600)
- **Standardized dates**: Converted Date column to proper Date type and
  filled empty dates with a default value
- **Removed duplicates**: Dropped duplicate rows from the dataset

## Tools
Power BI Desktop · Power Query Editor · M language (applied steps)

## Before / After
| | Before | After |
|---|---|---|
| Missing values | Present in 4 columns | 0 |
| Data types | Mixed/incorrect | Checked & Corrected across 6 columns |
| Duplicate rows | Present | Removed |

## Files
- `SalesFile.xlsx` — raw dataset (before)
- `SalesFile_Cleaned.pbix` — cleaned dataset (after)
- `screenshot/` — Power Query steps

<img width="1901" height="987" alt="Screenshot 2026-09-22 214040" src="https://github.com/user-attachments/assets/0002402c-46c6-4d13-84cc-ff49ca1f934c" />

## Key Takeaway
This project reinforced practical data-cleaning skills essential for
BI/Analyst roles — handling real-world messiness (nulls, wrong types,
inconsistent text vs numeric values, duplicates) using Power Query's
Applied Steps to build a repeatable, auditable transformation pipeline.
