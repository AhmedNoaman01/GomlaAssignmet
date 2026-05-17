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

## Screenshots

### 1 — Overview
<img width="1105" height="632" alt="Screenshot 2026-05-17 204819" src="https://github.com/user-attachments/assets/0928b418-6145-4483-9a17-7c25d163c8f2" />

### 2 — Sales Analysis
<img width="1111" height="627" alt="2" src="https://github.com/user-attachments/assets/7629da92-5a35-4daf-8310-ed85142b0e08" />

### 3 — Purchase Analysis
<img width="1112" height="632" alt="3" src="https://github.com/user-attachments/assets/51fd03c8-eb69-423d-9297-fc6d2db2744f" />

### 4 — Deadstock Items
<img width="1116" height="636" alt="4" src="https://github.com/user-attachments/assets/3df0d30d-36fd-433e-91a3-00e47ee70c7c" />

### 5 — Sales Tree
<img width="1131" height="631" alt="5" src="https://github.com/user-attachments/assets/1e047f0c-2147-4a77-99f8-6a012b67fa1c" />

---

> Built with SQL Server gold schema + Power BI Desktop
