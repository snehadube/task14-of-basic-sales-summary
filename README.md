# Basic Sales Summary — Veda Technology Internship (Data Analytics Track)

## Objective
Calculate **Total Sales**, **Average Sales**, and **Transaction Count** from a raw sales dataset and present them as a clean, formula-driven summary.

## Dataset
Sample Superstore-style sales dataset — 10,194 order-line records (Order ID, Order Date, Customer, Segment, Region, Category, Sales, Quantity, Discount, Profit).

## Tools
- Microsoft Excel (built with openpyxl, verified with LibreOffice recalculation)

## Approach
1. Loaded the raw dataset into a `Raw Data` sheet, unedited.
2. Built a `Summary` sheet with three live KPIs, each driven by a formula (not a hardcoded number):
   - **Total Sales** → `=SUM(...)`
   - **Average Sale Value** → `=AVERAGE(...)`
   - **Transaction Count** → `=COUNT(...)`
3. Added a manual verification block: an independent `SUMPRODUCT` cross-check for the total, and a `Total ÷ Count` recomputation of the average, with a `Match` flag.

## Results
| KPI | Value |
|---|---|
| Total Sales | $2,326,534.35 |
| Average Sale Value | $228.23 |
| Transaction Count | 10,194 |

Transaction Count = number of order-line rows (each product sold), not unique orders (5,111 unique Order IDs — one order can include multiple line items). Called out explicitly in the workbook.

## Verification
Manual cross-check formulas match the KPI formulas exactly — `Match?` cell returns `OK`.

## Files
- `Basic_Sales_Summary.xlsx` — the workbook (Raw Data + Summary sheets)
- `Basic_Sales_Summary_Report.pdf` — project report

## Author
Sneha Dubey — Veda Technology Data Analytics Internshipy
