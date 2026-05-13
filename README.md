# Gomla Market — Power BI Report
**File:** `Gomla_Report.pbix`  
**Database:** SQL Server — `GOMLA` (gold schema)  
**Period:** June 2024 – April 2025 | **Branches:** 52

---

## Data Model

| Layer | Tables |
|---|---|
| Dimensions | `gold.Dim_Item`, `gold.Dim_Branch`, `gold.Dim_Department`, `gold.Dim_Group`, `gold.Dim_SubGroup` |
| Facts | `gold.Fact_Sales`, `gold.Fact_Purchase` |

---

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

## Key Measures

| Measure | Logic |
|---|---|
| `Gross Profit` | Total Sales Value − Net Purchase Value |
| `Turnover Ratio` | Net Sales Qty ÷ Net Purchase Qty |
| `Days of Inventory` | 335 ÷ Turnover Ratio |
| `Is Deadstock` | Calculated column — "Deadstock" if Sales Qty = 0 or blank |
| `Movement Category` | Fast / Medium / Slow / Deadstock based on turnover ratio |

---

## How to Connect

1. Open `Gomla_Report.pbix` in Power BI Desktop
2. Go to **Home → Transform data → Data source settings**
3. Update the SQL Server name to your server
4. Database: `GOMLA`
5. Click **Refresh**

---

> Built with SQL Server gold schema + Power BI Desktop
