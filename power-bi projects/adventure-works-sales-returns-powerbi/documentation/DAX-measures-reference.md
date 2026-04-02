# DAX Measures Reference

This document lists all calculated measures created in the Adventure Works Power BI report.

---

## Core Measures

| Measure | Description |
|---|---|
| `Total Revenue` | Sum of order quantity × retail price across all transactions |
| `Total Cost` | Sum of order quantity × product cost |
| `Total Profit` | Total Revenue − Total Cost |
| `Total Orders` | Count of distinct order numbers |
| `Quantity Returned` | Sum of return quantities from the Returns table |
| `Total Customers` | Count of distinct customers with at least one order |

---

## Time Intelligence Measures

| Measure | Description |
|---|---|
| `YTD Revenue` | Year-to-date revenue using `DATESYTD()` |
| `Previous Month Revenue` | Revenue for the prior calendar month |
| `Previous Month Orders` | Order count for the prior calendar month |
| `Previous Month Returns` | Return count for the prior calendar month |
| `Previous Month Profit` | Profit for the prior calendar month |
| `10-Day Rolling Revenue` | Rolling 10-day revenue sum using `DATESINPERIOD()` |
| `90-Day Rolling Profit` | Rolling 90-day profit sum using `DATESINPERIOD()` |

---

## Ratio & Efficiency Measures

| Measure | Description |
|---|---|
| `Return Rate %` | Quantity Returned / Total Orders |
| `Profit Margin %` | Total Profit / Total Revenue |
| `% of All Orders` | Orders for current context / Total Orders (using `ALL()`) |
| `% of All Returns` | Returns for current context / Total Returns (using `ALL()`) |
| `Revenue per Customer` | Total Revenue / Total Customers |

---

## Target & Gap Measures

| Measure | Description |
|---|---|
| `Order Target` | Defined monthly order target |
| `Revenue Target` | Defined monthly revenue target |
| `Profit Target` | Defined monthly profit target |
| `Order Target Gap` | Total Orders − Order Target |
| `Revenue Target Gap` | Total Revenue − Revenue Target |
| `Profit Target Gap` | Total Profit − Profit Target |

---

## What-If & Dynamic Measures

| Measure | Description |
|---|---|
| `Price Adjustment %` | Numeric range parameter (slider input: 0% to 100%) |
| `Adjusted Price` | Overall Retail Price × (1 + Price Adjustment %) |
| `Total Profit Adjusted` | Recalculated profit using Adjusted Price |

---

## Key DAX Patterns Used

```dax
-- YTD Revenue
YTD Revenue =
CALCULATE(
    [Total Revenue],
    DATESYTD('Calendar'[Date])
)

-- Previous Month Revenue
Previous Month Revenue =
CALCULATE(
    [Total Revenue],
    DATEADD('Calendar'[Date], -1, MONTH)
)

-- Return Rate %
Return Rate % =
DIVIDE(
    [Quantity Returned],
    [Total Orders]
)

-- % of All Orders
% of All Orders =
DIVIDE(
    [Total Orders],
    CALCULATE([Total Orders], ALL('Sales Data'))
)

-- Total Profit Adjusted (What-If)
Total Profit Adjusted =
SUMX(
    'Sales Data',
    'Sales Data'[OrderQuantity] *
    (
        RELATED('Product Lookup'[ProductPrice]) * (1 + 'Price Adjustment'[Price Adjustment Value])
        - RELATED('Product Lookup'[ProductCost])
    )
)
```

---

*Reference document — Adventure Works Sales & Returns Analysis*  
*Created by: Hector Martin | Data Analyst | Ireland*
