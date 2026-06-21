## Project Overview

This project presents an interactive Power BI dashboard designed to analyze worldwide IT spending across multiple regions, business areas, and cost categories. The dashboard enables stakeholders to compare Actual vs Planned IT expenditures, identify overspending trends, monitor regional performance, and analyze spending distribution across IT functions.

The solution combines data modeling, DAX calculations, interactive visualizations, and business intelligence techniques to transform raw spending data into actionable insights.

---

## Business Problem

Organizations often struggle to:

- Track actual spending against planned budgets.
- Identify regions and departments responsible for overspending.
- Understand spending allocation across IT functions.
- Monitor monthly expenditure trends.
- Generate insights for strategic budget planning.

This dashboard addresses these challenges through an interactive reporting solution.

---

## Dataset Information

The project uses enterprise IT spending data containing:

- IT Spend Amounts
- Business Areas
- Cost Element Groups
- Cost Element Sub-Groups
- Departments
- Countries
- Sales Regions
- Monthly Spending Data
- Planned vs Actual Spending Scenarios

---

# Dashboard Pages

## 1. Home Dashboard

### Purpose

Provides an executive-level summary of worldwide IT spending.

### Key KPIs

| Metric | Value |
|----------|----------|
| Actual IT Spend | 858.42M |
| Planned IT Spend | 810.95M |
| Variance | +47.47M |
| Overspend % | 5.85% |

### Visualizations

#### KPI Cards

Displays:

- Total Actual IT Spend
- Total Planned IT Spend

#### IT Spend by Region and Scenario

Compares spending across:

- USA
- Europe
- Latin America
- Canada
- Australia & New Zealand
- Africa & Asia

Key Findings:

- USA contributes the largest share of IT spending.
- Europe is the second highest spending region.
- Latin America and Canada contribute relatively smaller amounts.

#### IT Spend by IT Area

Breakdown of spending across IT functions:

| IT Area | Spend |
|----------|----------|
| Functional | 555.95M |
| BU Support | 511.47M |
| Infrastructure | 418.80M |
| Governance | 98.22M |
| Enablement | 84.94M |

Insights:

- Functional IT activities account for the largest share.
- Governance and Enablement consume the smallest budgets.

#### Detailed Spend Table

Provides drill-down analysis using:

- Cost Element Group
- Cost Element Sub Group
- Month
- Scenario
- Spend Amount

---

## 2. Actual IT Spend Dashboard

### Purpose

Analyzes monthly spending behavior and budget variance.

### Visualizations

#### Actual IT Spend by Month

Monthly spending distribution:

| Month | Spend (M) |
|---------|----------|
| Dec | 93.91 |
| Jun | 73.46 |
| May | 73.11 |
| Nov | 72.72 |
| Jul | 72.67 |
| Mar | 72.21 |
| Sep | 71.55 |
| Oct | 69.56 |
| Aug | 68.61 |
| Apr | 66.36 |
| Feb | 65.63 |
| Jan | 58.62 |

Insights:

- December recorded the highest IT expenditure.
- January recorded the lowest expenditure.
- Spending remains relatively stable throughout the year.

#### IT Overspend Amount by Month

Tracks budget variance.

Highlights:

- December shows the highest overspend.
- January shows significant underspend.
- Most months remained within acceptable variance ranges.

#### Interactive Filters

Users can dynamically analyze data using:

##### Sales Region

- Africa & Asia
- Australia & NZ
- Canada
- Europe
- Latin America
- USA

##### Business Area

- BU
- Distribution
- Infrastructure
- Manufacturing
- Office & Administrative
- R&D
- Services

##### Cost Element Group

- Administrative
- CAPEX
- Depreciation & Amortization
- Hardware & Software
- Labor
- Other
- Shared Services

---

# Data Model

The dashboard follows a Star Schema architecture.

### Fact Table

#### IT_Spend

Contains:

- IT Spend Amount
- Business Area
- Cost Element Group
- Cost Element Sub Group
- Department
- Country
- IT Area
- Month

### Dimension Tables

#### Geography

Contains:

- Country
- Country ID
- Sales Region

#### IT_Area

Contains:

- IT Area
- IT Sub Area
- IT Area ID

#### Act_Pln_ByMonth

Contains:

- Month
- Scenario
- Month ID

### Relationships

- Geography → IT_Spend
- IT_Area → IT_Spend
- Act_Pln_ByMonth → IT_Spend

This structure enables efficient filtering and aggregation.

---

# Key Business Insights

### Spending Analysis

- Total Actual Spend exceeded Planned Spend by approximately 47.47M.
- Actual spending was 5.85% higher than budget.
- USA contributes the highest IT spending globally.
- Functional IT activities consume the largest budget share.
- Governance and Enablement receive comparatively lower investment.

### Monthly Trends

- Peak spending occurred in December.
- January had the lowest spending levels.
- Overspending was concentrated in a few months rather than throughout the year.

### Cost Management Opportunities

- Review high-spend Functional IT activities.
- Investigate December overspending.
- Optimize resource allocation across business units.

---

# Technical Skills Demonstrated

- Power BI
- Data Modeling
- Star Schema Design
- DAX Measures
- Interactive Dashboard Design
- KPI Development
- Data Visualization
- Business Intelligence Reporting
- Data Analysis
- Drill-through Analysis
- Cross Filtering
- Slicers and Dynamic Reporting

---

