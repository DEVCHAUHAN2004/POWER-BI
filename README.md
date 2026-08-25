# 📊 Power BI Business Intelligence & Analytics
  
<p align="center"> 



 
<img src="https://img.shields.io/badge/Microsoft%20Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/DAX-Analytics-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Power%20Query-ETL-green?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Data%20Analytics-Insights-purple?style=for-the-badge"/>

</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/microsoft/PowerBI-Icons/main/SVG/PowerBI.svg" width="110"/>
</p>

<h2 align="center">Turning Raw Data into Actionable Insights 🚀</h2>

<p align="center">
  An end-to-end Power BI analytics project focused on
  <b>Data Cleaning, Data Modeling, DAX, Visualization and Business Intelligence.</b>
</p>

---

## 🖥️ Dashboard Preview

<p align="center">
  <img src="assets/dashboard-preview.png" width="900"/>
</p>

> 💡 **Replace `assets/dashboard-preview.png` with your actual Power BI dashboard screenshot.**

---

# 🧠 About The Project

This project demonstrates a complete **Business Intelligence workflow using Microsoft Power BI**.

The objective is to transform raw and unstructured business data into an **interactive analytical dashboard** that allows users to monitor KPIs, identify trends, compare performance and discover actionable business insights.

### 🎯 Main Goals

| Goal         | Description                     |
| ------------ | ------------------------------- |
| 📊 Analyze   | Understand business performance |
| 🧹 Clean     | Prepare high-quality data       |
| 🔄 Transform | Create analysis-ready datasets  |
| 🧩 Model     | Build an efficient data model   |
| 🧮 Calculate | Create meaningful DAX measures  |
| 📈 Visualize | Build interactive dashboards    |
| 💡 Discover  | Generate actionable insights    |

---

# 🔥 Analytics Workflow

<p align="center">
  <img src="assets/analytics-workflow.png" width="850"/>
</p>

```text
        RAW DATA
           │
           ▼
    ┌──────────────┐
    │ Power Query  │
    │ Data Cleaning│
    └──────┬───────┘
           │
           ▼
    ┌──────────────┐
    │ Transformation│
    └──────┬───────┘
           │
           ▼
    ┌──────────────┐
    │ Data Modeling│
    └──────┬───────┘
           │
           ▼
       ┌───────┐
       │  DAX  │
       └───┬───┘
           │
           ▼
    ┌──────────────┐
    │ Visualization│
    └──────┬───────┘
           │
           ▼
    ┌──────────────┐
    │   INSIGHTS   │
    └──────────────┘
```

---

# 🛠️ Tech Stack

<p align="center">

<img src="https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/DAX-000000?style=flat-square"/>
<img src="https://img.shields.io/badge/Power%20Query-217346?style=flat-square"/>
<img src="https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoftexcel&logoColor=white"/>

</p>

---

# 🧹 Data Preparation

Data preparation was performed using **Power Query**.

### 🔧 Data Cleaning

* Removed duplicate records
* Handled missing values
* Corrected data types
* Removed unnecessary columns
* Renamed columns
* Standardized categorical values
* Created conditional columns
* Created custom columns

### 🔄 Data Transformation

* Filtering
* Merging queries
* Appending queries
* Grouping
* Pivot / Unpivot
* Date transformation
* Column splitting
* Data type conversion

---

# 🧩 Data Modeling

<p align="center">
  <img src="assets/data-model.png" width="850"/>
</p>

The dashboard follows a structured **Star Schema** wherever applicable.

```text
                   ┌──────────────┐
                   │ Date         │
                   │ Dimension    │
                   └──────┬───────┘
                          │
                          │
┌──────────────┐    ┌────▼─────┐    ┌──────────────┐
│ Customer     │    │          │    │ Product      │
│ Dimension    ├────►   FACT   ◄────┤ Dimension    │
└──────────────┘    │   TABLE  │    └──────────────┘
                    │          │
                    └────┬─────┘
                         │
                         ▼
                  ┌──────────────┐
                  │ Region       │
                  │ Dimension    │
                  └──────────────┘
```

### 📌 Benefits

* Better performance
* Cleaner relationships
* Easier DAX calculations
* Improved filtering
* Scalable analytical model

---

# 🧮 DAX & Measures

One of the major parts of this project is creating reusable DAX measures.

### 💰 Total Sales

```DAX
Total Sales =
SUM(Sales[SalesAmount])
```

### 💵 Total Profit

```DAX
Total Profit =
SUM(Sales[Profit])
```

### 📦 Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(Sales[OrderID])
```

### 📈 Profit Margin

```DAX
Profit Margin =
DIVIDE(
    [Total Profit],
    [Total Sales],
    0
)
```

### 📊 Average Sales

```DAX
Average Sales =
AVERAGE(Sales[SalesAmount])
```

---

# 📊 Dashboard Highlights

<p align="center">
  <img src="assets/kpi-dashboard.png" width="850"/>
</p>

### 🚀 KPI Cards

The dashboard provides quick access to important business metrics:

**💰 Total Sales**
**💵 Total Profit**
**📦 Total Orders**
**👥 Customers**
**📈 Growth %**
**🎯 Profit Margin**

---

# 📈 Visual Analytics

The dashboard includes:

| Visual         | Purpose               |
| -------------- | --------------------- |
| 📊 Bar Chart   | Category comparison   |
| 📈 Line Chart  | Time-series trends    |
| 🍩 Donut Chart | Contribution analysis |
| 🗺️ Map        | Geographic analysis   |
| 📋 Matrix      | Detailed breakdown    |
| 🎯 KPI         | Target vs Actual      |
| 📑 Table       | Record-level analysis |
| 🎛️ Slicer     | Interactive filtering |

---

# 🎛️ Interactive Features

Users can dynamically explore the dashboard using:

```text
🎛️ Slicers
     ↓
🔍 Filters
     ↓
📊 Visual Interaction
     ↓
🔎 Drill Through
     ↓
📋 Detailed Analysis
```

### Available interactions

* Date filtering
* Region filtering
* Product filtering
* Category filtering
* Customer filtering
* Drill-through pages
* Interactive tooltips
* Cross-filtering
* Page navigation

---

# 💡 Business Insights

The dashboard helps answer questions such as:

### 📈 Performance

* How are sales performing over time?
* Which month generated the highest revenue?
* What is the overall profit margin?

### 🏆 Products

* Which products are performing best?
* Which categories generate the most revenue?
* Which products have low profitability?

### 🌍 Geography

* Which regions generate the most sales?
* Which locations are underperforming?

### 👥 Customers

* Who are the top customers?
* Which customer segments contribute the most revenue?

---

# 📸 Dashboard Gallery

## 🏠 Executive Overview

<p align="center">
  <img src="assets/executive-dashboard.png" width="900"/>
</p>

---

## 📈 Sales Performance

<p align="center">
  <img src="assets/sales-analysis.png" width="900"/>
</p>

---

## 💰 Profit Analysis

<p align="center">
  <img src="assets/profit-analysis.png" width="900"/>
</p>

---

# 📂 Repository Structure

```text
📦 Power-BI-Analytics
│
├── 📁 Dataset
│   ├── sales_data.csv
│   └── customer_data.csv
│
├── 📁 Dashboard
│   └── PowerBI_Dashboard.pbix
│
├── 📁 Assets
│   ├── dashboard-preview.png
│   ├── analytics-workflow.png
│   ├── data-model.png
│   ├── kpi-dashboard.png
│   ├── executive-dashboard.png
│   ├── sales-analysis.png
│   └── profit-analysis.png
│
├── 📁 Documentation
│   └── Project_Documentation.pdf
│
└── README.md
```

---

# 🚀 How To Run

### 1. Clone Repository

```bash
git clone https://github.com/DEVCHAUHAN2004/Power-BI-Analytics.git
```

### 2. Open Power BI

Open:

```text
Dashboard/PowerBI_Dashboard.pbix
```

using **Power BI Desktop**.

### 3. Update Data Source

If required, update the dataset path from:

```text
Home → Transform Data → Data Source Settings
```

### 4. Refresh

Click:

```text
Home → Refresh
```

### 5. Explore 🎯

Interact with the dashboard using slicers, filters and drill-through features.

---

# 📚 What I Learned

Through this project, I strengthened my practical knowledge of:

* 📊 Power BI
* 🧮 DAX
* 🔄 Power Query
* 🧩 Data Modeling
* ⭐ Star Schema
* 📈 Data Visualization
* 📊 KPI Design
* 🔍 Exploratory Data Analysis
* 💼 Business Intelligence
* 💡 Data Storytelling

---

# 🔮 Future Enhancements

```text
Current
   │
   ├── Power BI Dashboard
   ├── DAX Analytics
   ├── Data Modeling
   └── Power Query
          │
          ▼
Future
   │
   ├── 🤖 Machine Learning
   ├── 🔮 Predictive Analytics
   ├── ☁️ Power BI Service
   ├── 🔄 Automated Refresh
   ├── 📱 Mobile Dashboard
   └── ⚡ Performance Optimization
```

---

# 👨‍💻 Author

<p align="center">

<img src="https://img.shields.io/badge/DEV%20CHAUHAN-Data%20Analyst-blue?style=for-the-badge"/>

</p>

### **Dev Chauhan**

🎓 B.Tech CSE — Data Science
📊 Aspiring Data Analyst
💻 Python • SQL • Power BI • Tableau • Excel
🤖 Data Analytics • Machine Learning • Data Visualization

---

# 🌐 Connect With Me

<p align="center">

<a href="https://github.com/DEVCHAUHAN2004">
<img src="https://img.shields.io/badge/GitHub-DEVCHAUHAN2004-black?style=for-the-badge&logo=github"/>
</a>

</p>







---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ **Star**.

<p align="center">

### ⭐ Star this repository if you like it!

### 📊 Data → Insights → Decisions 🚀

</p>

---

<p align="center">
  <b>Built with Microsoft Power BI • Designed for Data-Driven Decision Making</b>
</p>
