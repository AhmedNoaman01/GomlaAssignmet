# Gomla Market — Power BI Report
**File:** `Gomla_Report.pbix`  
**Database:** SQL Server — `GOMLA` (gold schema)  
**Period:** June 2024 – April 2025 | **Branches:** 52

---
## Important Notes

Dont forget to handle Excel file before use Sql Code

## Data Model

| Layer | Tables |
|---|---|
| Dimensions | `gold.Dim_Item`, `gold.Dim_Branch`, `gold.Dim_Department`, `gold.Dim_Group`, `gold.Dim_SubGroup` |
| Facts | `gold.Fact_Sales`, `gold.Fact_Purchase` |

---
<img width="918" height="727" alt="DB" src="https://github.com/user-attachments/assets/53750ff8-75a5-49e0-bc2b-9e6b01fceedc" />

## Report Pages

### 1 — Overview
High-level KPIs: total sales, gross profit, gross profit margin, return rate, deadstock count and capital locked. Includes department sales bar chart and movement category breakdown.

### 2 — Sales Analysis
Top 10 products by value and quantity. Department and branch performance. Slicers for branch and department filtering.

### 3 — Purchase Analysis
Purchase quantities and values per item. Return rates and bonus quantities from suppliers. Net purchase cost breakdown.

### 4 — Deadstock Items
Items purchased but never sold. Ranked by capital locked. Includes `Is Deadstock` column filter and total deadstock value card.

### 5 — Sales Tree
Drill-down hierarchy: Department → Main Group → Sub Group → Item. Shows contribution of each level to total sales value.


---

> Built with SQL Server gold schema + Power BI Desktop
