## Financial Performance Dashboard — Power BI

> An interactive, month-level financial dashboard built in Power BI for **The Finance Group**, enabling real-time monitoring of revenue, profitability, cash flow, and operational KPIs across regions and product categories.

---

## Project Overview

| Field | Details |
| :--- | :--- |
| **Client** | The Finance Group |
| **Role** | Data Analyst |
| **Tool** | Microsoft Power BI Desktop |
| **Data Period** | January 2023 – December 2024 |
| **Dataset Size** | 480 rows × 14 columns |
| **Dashboard Type** | Interactive, Monthly-Level Financial Dashboard |

---

## Project Structure

```text
financial-dashboard/
│
├── 📊 Financial_Analysis_Dashboard.pbix     # Power BI dashboard file
├── 📄 PowerBI Case Study.pdf                # Requirements & Project Brief
├── 📂 data/
│   └── Data_Analyst_Case_Study_Data.csv     # Source dataset (480 rows)
└── 📖 README.md                             # This file
```

---

## Dataset Columns

| Column | Type | Description |
| :--- | :--- | :--- |
| `Month` | Date | Time period (YYYY-MM format) |
| `Region` | Text | Geographic region (North, South, East, West) |
| `Product/Service` | Text | Product or service category |
| `Revenue` | Integer | Actual revenue earned |
| `COGS` | Decimal | Cost of Goods Sold |
| `Gross Profit` | Decimal | Revenue minus COGS |
| `Opex` | Integer | Operating Expenses |
| `EBITDA` | Decimal | Earnings Before Interest, Tax, Depreciation & Amortization |
| `Cash Inflows` | Integer | Money received into business |
| `Cash Outflows` | Integer | Money paid out of business |
| `Receivables Aging (Days)` | Integer | Days customers owe money |
| `Payables Aging (Days)` | Integer | Days owed to suppliers |
| `Revenue Budget` | Integer | Planned/targeted revenue |
| `Budget Variance %` | Decimal | Actual vs Budget percentage difference |

---

## Data Model

```text
Date Table  ──────────────────────────────────────────────  FinData
(Year-Month) ──[One-to-Many Relationship]──  (Month column)

_Measures  (Dedicated DAX measures table)
├── Total Revenue
├── Gross Margin %
├── EBITDA %
└── Net Cash
```

---

## DAX Measures

### Total Revenue
```dax
Total Revenue = SUM(FinData[Revenue])
```

### Gross Margin %
```dax
Gross Margin % = 
DIVIDE(
    SUM(FinData[Gross Profit]), 
    SUM(FinData[Revenue]), 
    0
)
```

### EBITDA %
```dax
EBITDA % = 
DIVIDE(
    SUM(FinData[EBITDA]), 
    SUM(FinData[Revenue]), 
    0
)
```

### Net Cash
```dax
Net Cash = SUM(FinData[Cash Inflows]) - SUM(FinData[Cash Outflows])
```

---

## Dashboard Design

### Color Theme — Classic Finance
| Element | Hex Code |
| :--- | :--- |
| **Background** | `#0D1B2A` |
| **Cards/Charts** | `#1B2A3B` |
| **Accents** | `#C9A84C` |
| **Success/Positive** | `#2ECC71` |
| **Warning/Negative** | `#E74C3C` |

This is a high-quality, professional README structure. It balances technical documentation with business context, making it perfect for a portfolio or a corporate repository.

Since you like this specific style—clean headers, clear tables, and structured DAX blocks—I have refined your project details into a final, copy-paste-ready version. I have also ensured the formatting is optimized for GitHub's Markdown rendering.

***

## Financial Performance Dashboard — Power BI

> An interactive, month-level financial dashboard built in Power BI for **The Finance Group**, enabling real-time monitoring of revenue, profitability, cash flow, and operational KPIs across regions and product categories.

---

## Project Overview

| Field | Details |
| :--- | :--- |
| **Client** | The Finance Group |
| **Role** | Data Analyst |
| **Tool** | Microsoft Power BI Desktop |
| **Data Period** | January 2023 – December 2024 |
| **Dataset Size** | 480 rows × 14 columns |
| **Dashboard Type** | Interactive, Monthly-Level Financial Dashboard |

---

## Project Structure

```text
financial-dashboard/
│
├── 📊 Financial_Analysis_Dashboard.pbix     # Power BI dashboard file
├── 📄 PowerBI Case Study.pdf                # Requirements & Project Brief
├── 📂 data/
│   └── Data_Analyst_Case_Study_Data.csv     # Source dataset (480 rows)
└── 📖 README.md                             # This file
```

---

## Dataset Columns

| Column | Type | Description |
| :--- | :--- | :--- |
| `Month` | Date | Time period (YYYY-MM format) |
| `Region` | Text | Geographic region (North, South, East, West) |
| `Product/Service` | Text | Product or service category |
| `Revenue` | Integer | Actual revenue earned |
| `COGS` | Decimal | Cost of Goods Sold |
| `Gross Profit` | Decimal | Revenue minus COGS |
| `Opex` | Integer | Operating Expenses |
| `EBITDA` | Decimal | Earnings Before Interest, Tax, Depreciation & Amortization |
| `Cash Inflows` | Integer | Money received into business |
| `Cash Outflows` | Integer | Money paid out of business |
| `Receivables Aging (Days)` | Integer | Days customers owe money |
| `Payables Aging (Days)` | Integer | Days owed to suppliers |
| `Revenue Budget` | Integer | Planned/targeted revenue |
| `Budget Variance %` | Decimal | Actual vs Budget percentage difference |

---

## Data Model

```text
Date Table  ──────────────────────────────────────────────  FinData
(Year-Month) ──[One-to-Many Relationship]──  (Month column)

_Measures  (Dedicated DAX measures table)
├── Total Revenue
├── Gross Margin %
├── EBITDA %
└── Net Cash
```

---

## DAX Measures

### Total Revenue
```dax
Total Revenue = SUM(FinData[Revenue])
```

### Gross Margin %
```dax
Gross Margin % = 
DIVIDE(
    SUM(FinData[Gross Profit]), 
    SUM(FinData[Revenue]), 
    0
)
```

### EBITDA %
```dax
EBITDA % = 
DIVIDE(
    SUM(FinData[EBITDA]), 
    SUM(FinData[Revenue]), 
    0
)
```

### Net Cash
```dax
Net Cash = SUM(FinData[Cash Inflows]) - SUM(FinData[Cash Outflows])
```

---

## Dashboard Design

### Color Theme — Classic Finance
| Element | Hex Code |
| :--- | :--- |
| **Background** | `#0D1B2A` |
| **Cards/Charts** | `#1B2A3B` |
| **Accents** | `#C9A84C` |
| **Success/Positive** | `#2ECC71` |
| **Warning/Negative** | `#E74C3C` |

![image alt](https://github.com/vnandini879/Financial-Analysis/blob/d79fe6e2fba8a9f56bae1e85a427a5da9102ab94/financial%20dashboard.png)

---

## Dashboard Visuals

| # | Visual | Fields Used | Purpose |
| :--- | :--- | :--- | :--- |
| 1 | **KPI Cards** | Revenue, Gross Margin, EBITDA, Net Cash | High-level health snapshot |
| 2 | **Line Chart** | Revenue Trend | Analyze growth over 24 months |
| 3 | **Waterfall Chart** | Cash Inflows vs Outflows | Visualize liquidity movement |
| 4 | **Bar Chart** | Product Performance | Identify top-grossing categories |
| 5 | **Clustered Bar** | Receivables Aging | Monitor collection efficiency & risk |
| 6 | **Slicers** | Region, Product, Date | Enable granular data exploration |

!Dashboard(C:\Users\RAJ NANDINI\Downloads\internship projects/financial dashboard.png)
---

## How to Use

1. **Filtering:** Use the slicers on the left/top to narrow down data by specific regions or timeframes.
2. **Drill-Down:** Right-click on a specific month in the trend chart to see a deeper breakdown of product performance for that period.
3. **Cross-Filtering:** Click on any segment in the "Product Performance" chart to automatically update all other visuals to reflect that specific category.

---

## Key Insights

* **Regional Dominance:** The North region consistently leads in revenue generation.
* **Product vs. Service:** Product C and Service X are the primary drivers of the gross margin.
* **Liquidity:** While Net Cash remains positive (~39K), significant fluctuations suggest a need for tighter Opex management.
* **Collection Risk:** A notable portion of receivables is entering the 30-60 day bracket, signaling potential future cash flow hurdles.

---

## Setup Instructions

1.  Download and install **Power BI Desktop**.
2.  Clone this repository to your local machine.
3.  Open `Financial_Analysis_Dashboard.pbix`.
4.  If the data link is broken, go to `Transform Data > Data Source Settings` and point it to the included `Data_Analyst_Case_Study_Data.csv`.
5.  Hit **Refresh** to populate the visuals.

---

## Deliverables

* [x] **Power BI Dashboard (.pbix)**
* [x] **Cleaned Dataset (.csv)**
* [x] **Technical Documentation**
* [x] **README Guide**
---

## Dashboard Visuals

| # | Visual | Fields Used | Purpose |
| :--- | :--- | :--- | :--- |
| 1 | **KPI Cards** | Revenue, Gross Margin, EBITDA, Net Cash | High-level health snapshot |
| 2 | **Line Chart** | Revenue Trend | Analyze growth over 24 months |
| 3 | **Waterfall Chart** | Cash Inflows vs Outflows | Visualize liquidity movement |
| 4 | **Bar Chart** | Product Performance | Identify top-grossing categories |
| 5 | **Clustered Bar** | Receivables Aging | Monitor collection efficiency & risk |
| 6 | **Slicers** | Region, Product, Date | Enable granular data exploration |

---

## How to Use

1. **Filtering:** Use the slicers on the left/top to narrow down data by specific regions or timeframes.
2. **Drill-Down:** Right-click on a specific month in the trend chart to see a deeper breakdown of product performance for that period.
3. **Cross-Filtering:** Click on any segment in the "Product Performance" chart to automatically update all other visuals to reflect that specific category.

---

## Key Insights

* **Regional Dominance:** The North region consistently leads in revenue generation.
* **Product vs. Service:** Product C and Service X are the primary drivers of the gross margin.
* **Liquidity:** While Net Cash remains positive (~39K), significant fluctuations suggest a need for tighter Opex management.
* **Collection Risk:** A notable portion of receivables is entering the 30-60 day bracket, signaling potential future cash flow hurdles.

---

## Setup Instructions

1.  Download and install **Power BI Desktop**.
2.  Clone this repository to your local machine.
3.  Open `Financial_Analysis_Dashboard.pbix`.
4.  If the data link is broken, go to `Transform Data > Data Source Settings` and point it to the included `Data_Analyst_Case_Study_Data.csv`.
5.  Hit **Refresh** to populate the visuals.

---

## Deliverables

* [x] **Power BI Dashboard (.pbix)**
* [x] **Cleaned Dataset (.csv)**
* [x] **Technical Documentation**
* [x] **README Guide**
