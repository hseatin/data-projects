# 📊 Data Projects Portfolio

A curated collection of end-to-end data analytics and business intelligence projects, spanning interactive Power BI dashboards and Python-driven data pipelines with Looker Studio reporting. Each project addresses a real-world business problem — from raw, fragmented data to actionable insights.

> 🚧 This portfolio is actively growing. New projects will be added over time.

---

## 📁 Repository Structure

```
data-projects/
├── power-bi projects/
│   ├── adventure-works-sales-returns-powerbi/
│   └── maven-market-retail-performance-powerbi/
└── python projects/
    └── energy-consumption-python-looker/
```

---

## 🟡 Power BI Projects

Interactive, self-service Business Intelligence solutions built in Microsoft Power BI. Each report integrates multiple data sources into a unified analytical platform, enabling stakeholders to monitor KPIs, explore trends, and make confident, data-driven decisions.

---

### 1. Adventure Works — Sales & Returns BI Report

> **Tools:** Microsoft Power BI · DAX · Power Query  
> **Domain:** Retail / Manufacturing  
> **Data Period:** 2020 – 2022

**Overview**

A comprehensive Business Intelligence solution for Adventure Works, a global bicycle manufacturing company. The report integrates transactional data across sales, returns, customers, products, and territories into a single, unified analytical platform — replacing fragmented CSV files with an interactive, self-service reporting experience.

**Business Problem**

Key business data was scattered across multiple disconnected source files, making it nearly impossible to track core KPIs in a unified view, compare regional and product performance, identify drivers of profit loss or elevated return rates, or perform meaningful time-based analysis.

**Key Features**

- Unified data model consolidating Sales, Returns, Customers, Products, and Territories
- Core KPI tracking: Revenue, Profit, Orders, and Return Rate
- Time intelligence: Year-to-Date (YTD) and month-over-month comparisons
- Cross-filtering across regions, product lines, and customer segments
- Interactive, self-service report design for senior management and regional teams

**Stakeholders:** Senior management · Regional sales managers · Product teams

🔗 [View Project](https://github.com/hseatin/data-projects/tree/main/power-bi%20projects/adventure-works-sales-returns-powerbi)

---

### 2. Maven Market — Retail Performance Dashboard

> **Tools:** Microsoft Power BI · DAX · Power Query  
> **Domain:** Retail / Grocery  
> **Geography:** United States · Canada · Mexico

**Overview**

An end-to-end Business Intelligence solution for Maven Market, a multinational grocery retailer operating across North America. The report delivers a 360° analytical view of revenue performance, profitability, customer demographics, product returns, and time-based growth trends — all within a single, interactive reporting environment.

**Business Problem**

Without a centralised reporting solution, extracting meaningful insights from raw, siloed data was time-consuming and inefficient. Revenue and profitability were tracked manually, store and regional performance lacked standardisation, and time-based KPI tracking required manual calculation.

**Key Features**

- 360° view across revenue, profitability, customer behaviour, and store performance
- Multi-country and multi-store performance comparison
- Product return rate and margin trend monitoring
- Customer demographic analysis
- Time intelligence: Year-over-Year (YoY), Month-over-Month (MoM), and YTD KPI tracking
- Strategic revenue target tracking

**Stakeholders:** Executive leadership · Regional managers · Commercial and operations teams

🔗 [View Project](https://github.com/hseatin/data-projects/tree/main/power-bi%20projects/maven-market-retail-performance-powerbi)

---

## 🐍 Python Projects

Data engineering and analytics pipelines built in Python, combining data ingestion, cleaning, feature engineering, and KPI calculation — with final dashboards published in Google Looker Studio.

---

### 1. Energy Consumption & Solar PV Analytics Pipeline

> **Tools:** Python · Pandas · Google Looker Studio  
> **Domain:** Residential Energy / Renewable Energy  
> **Type:** End-to-End Data Pipeline

**Overview**

A complete end-to-end energy data analytics pipeline combining electricity consumption data, solar PV production data, and weather information into a unified reporting system. The pipeline spans data ingestion, cleaning, feature engineering, KPI calculation, and dashboard publication in Google Looker Studio.

Developed as a real-world personal energy monitoring solution, this project also serves as a portfolio demonstration of Python data engineering and business intelligence skills.

**Business Problem**

Rising energy costs and growing adoption of residential solar systems create a genuine need for granular energy monitoring. Standard supplier portals provide only summary-level data and do not differentiate between smart tariff periods — making it difficult to understand actual energy costs and solar efficiency.

**Key Questions Addressed**

- How much electricity is imported from the grid, and when (day vs. night smart tariff)?
- How much energy is generated by the solar PV system daily and monthly?
- What proportion of solar production is self-consumed versus exported to the grid?
- How does weather (temperature, sunshine, precipitation) correlate with solar output?
- What is the actual cost of electricity after factoring in smart tariffs and solar export revenue?

**Key Features**

- Automated data ingestion from multiple sources (consumption, solar, weather)
- Data cleaning, transformation, and feature engineering in Python/Pandas
- Smart tariff period segmentation (day vs. night rates)
- Solar self-consumption and export revenue calculation
- Weather correlation analysis
- Interactive Looker Studio dashboard for ongoing monitoring

**Stakeholders:** Residential energy consumers · Energy analysts · Renewable energy professionals

🔗 [View Project](https://github.com/hseatin/data-projects/tree/main/python%20projects/energy-consumption-python-looker)

---

## 🛠️ Tools & Technologies

| Category | Tools |
|---|---|
| Business Intelligence | Microsoft Power BI |
| Query & Modelling | DAX, Power Query (M) |
| Programming | Python |
| Data Manipulation | Pandas |
| Reporting | Google Looker Studio |

---

## 👤 About

This portfolio is maintained by [Hector Martin](https://github.com/hseatin) and reflects a focus on practical, business-driven data analytics — building solutions that turn raw data into clear, actionable insights.

Feel free to explore the individual project folders for full documentation, data models, and report screenshots.
