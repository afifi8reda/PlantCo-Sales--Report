# 🌿 Performance Plant Co. — Power BI Dashboard

> A full end-to-end Business Intelligence project built with Power BI, covering data modeling, DAX measures, and interactive visualizations for a plant distribution company.

---

## 📸 Preview

| Home | Overview | Details |
|------|----------|---------|
| Home Page | Overview Page | Details Page |

---

## 📁 Project Structure

```
Performance-Plant-Co-PowerBI/
│
├── 📊 PlantCo_Dashboard.pbix     # Main Power BI file
├── 📄 README.md
└── 📸 Screenshots/
    ├── home.png
    ├── overview_2022.png
    ├── overview_2023.png
    ├── overview_2024.png
    └── details.png
```

---

## 🗂️ Data Model

**Star Schema Design:**
- `Fact_Sales` — Core transaction table
- `Dim_Product` — Product hierarchy (Family → Group → Name)
- `Dim_Accounts` — Customer accounts with country mapping
- `Calendar_Table` — Date table with PYTD flag (Inpast column)
- `_Measures` — Dedicated measures table (organized in folders)
- `_Slicer_Values` — Disconnected table for dynamic metric switching

---

## 📐 DAX Measures

### Base Metrics
| Measure | Description |
|---------|-------------|
| `Sales` | Total sales revenue |
| `Gross Profit` | Sales minus COGS |
| `QTY` | Total quantity sold |
| `COGS` | Cost of goods sold |

### YTD Measures
| Measure | Description |
|---------|-------------|
| `YTD_Sales` | Year-to-date sales |
| `YTD_GP` | Year-to-date gross profit |
| `YTD_QTY` | Year-to-date quantity |
| `GP Margin %` | Gross profit margin percentage |

### PYTD Measures
| Measure | Description |
|---------|-------------|
| `PYTD_Sales` | Prior year-to-date sales |
| `PYTD_GP` | Prior year-to-date gross profit |
| `PYTD_QTY` | Prior year-to-date quantity |

### KPIs
| Measure | Description |
|---------|-------------|
| `YoY Growth` | Year-over-year absolute growth |
| `YoY Growth %` | Year-over-year percentage growth |

---

## 📊 Report Pages

### 1. Home
Navigation landing page with links to all report sections.

### 2. Overview
Sales performance dashboard with:
- KPI cards (PYTD, YTD, YoY Growth, YoY Growth %)
- Stacked bar chart — Sales by Month & Product Type
- Scatter plot — Account Profitability (GP% vs YTD Sales)
- Waterfall chart — Sales Drivers by Month/Country/Product
- Dynamic AI-generated insights text

### 3. Details
Drill-through decomposition view with:
- Decomposition tree — YTD by Country → Product Group → Product Type
- Cross-filtering with Country, Product Group, and Product Type slicers

### 4. About
Company overview and business context page.

---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **DAX** (Data Analysis Expressions)
- **Power Query** (M Language)

---

## 📈 Key Findings

- **2024**: YTD = 4M | PYTD = 3.71M | YoY Growth = -3.67%
- **2023**: YTD = 13M | PYTD = 13.51M | YoY Growth = -3.79%
- **Outdoor** segment consistently leads in average YTD across all years
- Top account in 2023: **Labadie Group** with 163K units and 73K GP

---

## 🚀 How to Use

1. Clone the repository
2. Open `PlantCo_Dashboard.pbix` in Power BI Desktop
3. Use the year slicer to switch between 2022, 2023, and 2024
4. Use the metric slicer to toggle between Sales, Gross Profit, and Quantity

---

## 👤 Author

Afifi Elkady
LinkedIn 
https://www.linkedin.com/in/afifi8reda/

## 📄 License
This project is for portfolio and educational purposes only.
