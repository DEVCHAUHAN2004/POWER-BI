# 📊 Power BI — Data Analytics & Business Intelligence

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Data%20Analytics-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/SQL-Advanced-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Excel-Analytics-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" />
  <img src="https://img.shields.io/badge/DAX-Data%20Modeling-107C41?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Power%20Query-ETL-742774?style=for-the-badge" />
</p>

<p align="center">
  <b>📈 Turning raw data into meaningful insights, interactive dashboards, and business decisions.</b>
</p>

---

## 🧑‍💻 About This Repository

Welcome to my **Power BI Analytics Repository** 🚀

This repository contains my learning journey and practical work in **Microsoft Power BI**, with a strong focus on:

* 📊 Interactive Dashboard Development
* 🧹 Data Cleaning & Transformation
* 🔄 ETL using Power Query
* 🧮 DAX & Measure Creation
* 🗂️ Data Modeling
* 📈 Business Intelligence
* 🔍 Exploratory Data Analysis
* 💡 Business Insights & KPI Analysis
* 📑 Real-world Analytics Projects

The goal of this repository is to demonstrate how I transform **raw datasets → clean data → data models → dashboards → actionable insights**.

---

## 🛠️ Tech Stack

| Technology             | Purpose                          |
| ---------------------- | -------------------------------- |
| 🟡 **Power BI**        | Dashboard & Data Visualization   |
| 🟢 **Power Query**     | Data Cleaning & ETL              |
| 🔵 **DAX**             | Measures, KPIs & Calculations    |
| 🟢 **Microsoft Excel** | Data Preparation & Analysis      |
| 🟣 **SQL**             | Data Extraction & Transformation |
| 🐍 **Python**          | Data Analysis & Preprocessing    |
| 🗄️ **PostgreSQL**     | Database Management              |

---

# 📚 Power BI Skills

## 1️⃣ Power Query — Data Transformation

I use **Power Query** to prepare raw data before analysis.

### Key Operations

* Data Cleaning
* Removing Duplicates
* Handling Null Values
* Changing Data Types
* Splitting & Merging Columns
* Filtering Rows
* Conditional Columns
* Custom Columns
* Merging Queries
* Appending Queries
* Data Transformation
* Basic ETL Processes

### 🔄 ETL Workflow

```text
Raw Data
   ↓
Extract
   ↓
Power Query
   ↓
Clean & Transform
   ↓
Data Model
   ↓
DAX Calculations
   ↓
Dashboard
   ↓
Business Insights
```

---

# 🗂️ Data Modeling

A strong data model is the foundation of a good Power BI report.

### Concepts Covered

* ⭐ Fact Tables
* ⭐ Dimension Tables
* ⭐ Star Schema
* ⭐ Relationships
* ⭐ One-to-Many Relationships
* ⭐ Primary & Foreign Keys
* ⭐ Date Tables
* ⭐ Cardinality
* ⭐ Filter Direction
* ⭐ Model Optimization

### ⭐ Star Schema

```text
                 ┌─────────────────┐
                 │   Dim Customer  │
                 └────────┬────────┘
                          │
                          │
┌──────────────┐    ┌─────▼──────┐    ┌──────────────┐
│  Dim Product │────│ Fact Sales │────│  Dim Date    │
└──────────────┘    └─────┬──────┘    └──────────────┘
                          │
                          │
                   ┌──────▼───────┐
                   │ Dim Location │
                   └──────────────┘
```

---

# 🧮 DAX

DAX (**Data Analysis Expressions**) is used to create calculated measures and analytical logic.

## Important DAX Functions

### Aggregation

```DAX
Total Sales =
SUM(Sales[SalesAmount])
```

```DAX
Total Quantity =
SUM(Sales[Quantity])
```

### COUNT

```DAX
Total Orders =
COUNT(Sales[OrderID])
```

### DISTINCTCOUNT

```DAX
Unique Customers =
DISTINCTCOUNT(Sales[CustomerID])
```

### CALCULATE

```DAX
Total Sales 2026 =
CALCULATE(
    [Total Sales],
    Sales[Year] = 2026
)
```

### DIVIDE

```DAX
Profit Margin =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
```

### Time Intelligence

```DAX
Previous Year Sales =
CALCULATE(
    [Total Sales],
    SAMEPERIODLASTYEAR('Date'[Date])
)
```

```DAX
YoY Growth % =
DIVIDE(
    [Total Sales] - [Previous Year Sales],
    [Previous Year Sales],
    0
)
```

---

# 📊 Dashboard Development

My dashboards focus on making complex datasets easy to understand.

### Dashboard Components

* 📌 KPI Cards
* 📊 Bar Charts
* 📈 Line Charts
* 🍩 Donut Charts
* 🗺️ Maps
* 📋 Tables
* 🎯 Slicers
* 🔢 Cards
* 📉 Trend Analysis
* 🔍 Drill-through
* 📝 Tooltips
* 🔄 Interactive Filters

---

# 🚀 Featured Power BI Projects

## 👥 1. HR Analytics Dashboard

An interactive HR dashboard designed to analyze employee data and workforce trends.

### 🔍 Key Analysis

* Total Employees
* Attrition Rate
* Average Salary
* Employee Distribution
* Department Analysis
* Gender Analysis
* Age Distribution
* Job Role Analysis
* Experience Analysis
* Employee Attrition

### 📌 Key KPIs

```text
👨‍💼 Total Employees
📉 Attrition Rate
💰 Average Salary
⏳ Average Experience
👥 Active Employees
```

### 🖼️ Dashboard Preview

> 📌 Add your HR Dashboard screenshot here.

```markdown
![HR Analytics Dashboard](images/hr-dashboard.png)
```

---

# 💰 2. Sales Analytics Dashboard

A business-focused dashboard for analyzing sales performance and revenue trends.

### 🔍 Key Analysis

* Total Sales
* Total Profit
* Total Orders
* Sales by Region
* Sales by Category
* Sales by Product
* Monthly Sales Trends
* Profitability Analysis
* Customer Performance

### 📌 Key KPIs

```text
💰 Total Sales
📈 Total Profit
🛒 Total Orders
👥 Customers
📊 Profit Margin
```

### 🖼️ Dashboard Preview

> 📌 Add your Sales Dashboard screenshot here.

```markdown
![Sales Analytics Dashboard](images/sales-dashboard.png)
```

---

# 📈 Business Intelligence Workflow

```text
                 RAW DATA
                    │
                    ▼
            ┌───────────────┐
            │ Data Sources  │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │ Power Query   │
            │ Cleaning/ETL  │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │ Data Modeling │
            │ Star Schema   │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │     DAX       │
            │ Measures/KPIs │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │  Dashboard    │
            │ Visualization │
            └───────┬───────┘
                    │
                    ▼
            ┌───────────────┐
            │   Insights    │
            │ & Decisions   │
            └───────────────┘
```

---

# 🎯 Important Power BI Concepts

### 📌 Data Preparation

* Data Cleaning
* Data Transformation
* Data Types
* Missing Values
* Duplicate Records
* Data Validation

### 📌 Data Modeling

* Relationships
* Fact & Dimension Tables
* Star Schema
* Date Tables
* Cardinality
* Filter Context

### 📌 DAX

* SUM
* COUNT
* DISTINCTCOUNT
* CALCULATE
* FILTER
* ALL
* ALLEXCEPT
* DIVIDE
* IF
* SWITCH
* SUMX
* AVERAGEX
* COUNTROWS
* RELATED
* Time Intelligence

### 📌 Visualization

* KPI Cards
* Bar Charts
* Line Charts
* Pie/Donut Charts
* Maps
* Tables
* Matrix
* Slicers
* Drill-through
* Tooltips
* Bookmarks

---

# 📁 Repository Structure

```text
Power-BI/
│
├── 📂 HR-Analytics/
│   ├── HR_Analytics.pbix
│   ├── dataset.csv
│   └── dashboard.png
│
├── 📂 Sales-Analytics/
│   ├── Sales_Dashboard.pbix
│   ├── dataset.csv
│   └── dashboard.png
│
├── 📂 Projects/
│   ├── Project-01/
│   ├── Project-02/
│   └── Project-03/
│
├── 📂 DAX/
│   ├── measures.md
│   └── dax-examples.md
│
├── 📂 Power-Query/
│   └── transformations.md
│
├── 📂 Images/
│   ├── hr-dashboard.png
│   ├── sales-dashboard.png
│   └── powerbi-workflow.png
│
└── README.md
```

---

# 🧠 What I Focus On

```text
Data
 ↓
Clean
 ↓
Transform
 ↓
Model
 ↓
Analyze
 ↓
Visualize
 ↓
Communicate
 ↓
Decision
```

My focus is not only on creating visually attractive dashboards, but also on understanding:

> **"What does the data tell us, and what business decision can we make from it?"**

---

# 📊 Analytics Areas

| Area         | Analysis                            |
| ------------ | ----------------------------------- |
| 👥 HR        | Employees, Attrition, Salary        |
| 💰 Sales     | Revenue, Profit, Orders             |
| 👤 Customers | Customer Segmentation & Performance |
| 📦 Products  | Product Performance                 |
| 🌍 Geography | Regional & Location Analysis        |
| ⏳ Time       | Monthly, Quarterly & Yearly Trends  |
| 🎯 KPIs      | Business Performance Metrics        |

---

# 💡 Dashboard Design Principles

I follow these principles while designing dashboards:

### 🎨 1. Clean Design

Avoid unnecessary visuals and focus on important information.

### 🎯 2. KPI First

Important business metrics should be visible immediately.

### 🔍 3. Interactive Analysis

Use slicers, filters and drill-through for deeper analysis.

### 📊 4. Consistent Visuals

Maintain consistent formatting, spacing and hierarchy.

### 📱 5. User-Friendly

Dashboards should be understandable even for non-technical users.

### 💼 6. Business-Oriented

Every visualization should answer a business question.

---

# ❓ Business Questions I Try to Answer

### HR

* What is the current employee count?
* Which department has the highest attrition?
* Which job roles have the highest turnover?
* How does salary vary across departments?
* What factors are associated with employee attrition?

### Sales

* What is the total revenue?
* Which products generate the highest sales?
* Which region performs best?
* What is the monthly sales trend?
* Which products generate the highest profit?
* How is the business performing compared with the previous year?

---

# 📈 Example KPI Layout

```text
┌────────────────┬────────────────┬────────────────┬────────────────┐
│  TOTAL SALES   │ TOTAL PROFIT   │ TOTAL ORDERS  │ PROFIT MARGIN  │
│                │                │                │                │
│   ₹12.5M       │    ₹2.8M       │    18,450     │     22.4%      │
└────────────────┴────────────────┴────────────────┴────────────────┘

┌───────────────────────────────────────────────────────────────────┐
│                       SALES TREND                                 │
│                                                                   │
│        📈 Monthly / Quarterly / Yearly Performance               │
│                                                                   │
└───────────────────────────────────────────────────────────────────┘
```

---

# 🏆 Learning Goals

* [x] Power BI Fundamentals
* [x] Power Query
* [x] Data Cleaning
* [x] Data Modeling
* [x] DAX Fundamentals
* [x] KPI Creation
* [x] Interactive Dashboards
* [x] Business Analysis
* [ ] Advanced DAX
* [ ] Advanced Data Modeling
* [ ] Power BI Service
* [ ] Row-Level Security
* [ ] Dashboard Deployment
* [ ] Advanced Performance Optimization

---

# 📚 My Data Analytics Journey

```text
Python
   ↓
SQL
   ↓
Excel
   ↓
Statistics
   ↓
Data Cleaning
   ↓
Power BI
   ↓
Tableau
   ↓
Machine Learning
   ↓
Business Intelligence
```

---

# 🔗 Connect With Me

<p align="center">

<a href="https://github.com/DEVCHAUHAN2004">
<img src="https://img.shields.io/badge/GitHub-DEVCHAUHAN2004-181717?style=for-the-badge&logo=github"/>
</a>

<a href="https://www.linkedin.com/">
<img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin"/>
</a>

</p>

---

# ⭐ If You Find This Useful

If you find this repository useful for learning **Power BI, Data Analytics, DAX or Business Intelligence**, consider giving it a ⭐.

<p align="center">

### 🚀 Learn → Analyze → Visualize → Communicate → Decide

**Made with 📊 and 💡 by Dev Chauhan**

</p>
