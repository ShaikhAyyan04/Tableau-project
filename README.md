# 📊 Tableau Inventory Management & Shipment Performance Dashboard

## 📌 Project Overview

This project is an interactive **Inventory Management and Shipment Performance Dashboard built using Tableau**. It analyzes inventory levels, order shipments, delivery delays, storage costs, warehouse performance, and supply-demand balance.

The goal is to turn operational data into meaningful business insights that can help businesses monitor inventory, identify shipment delays, control overstock costs, and improve supply chain efficiency.

## 🎯 Project Objectives

- Analyze inventory balance and warehouse inventory levels.
- Monitor shipment delays and delivery performance.
- Calculate average shipment delay days.
- Analyze delay rates by market, country, and shipment mode.
- Compare inventory levels with product demand.
- Identify overstock and understock situations.
- Analyze storage costs by product category.
- Track inventory balance and overstock costs over time.
- Support data-driven inventory and supply chain decisions.

## 🏢 Business Problem

Businesses need to maintain sufficient inventory while ensuring that customer orders are delivered on time. Excess inventory increases storage costs, while insufficient inventory can affect product availability. Shipment delays can also reduce operational efficiency and customer satisfaction.

This Tableau project provides a visual way to analyze inventory, shipment performance, and supply-demand balance to identify areas that require attention.

## 📊 Dashboard Overview

### 1. Inventory Balance Dashboard

Analyzes inventory levels and stock balance to help understand whether warehouse inventory is sufficient to meet demand.

Key analysis:
- Average Inventory Balance KPI
- Average Inventory Balance by Category
- Monthly Inventory Balance
- Supply vs. Demand Analysis
- Overstock and Understock Status
- Overstock Storage Cost KPI
- Overstock Cost by Month

### 2. Shipment Performance Dashboard

Analyzes shipment delays and delivery performance across different dimensions.

Key analysis:
- Average Delay Days
- Delay Order Item Percentage
- Delay Rate by Market
- Delay Rate by Shipment Mode
- Delay Rate by Country
- Shipment Delay Trend by Month
- Shipment Status Analysis
- Warehouse Performance by Country

### 3. Inventory and Shipment Analysis

The workbook also contains supporting worksheets for monthly trends, shipment filters, order-year filtering, inventory calculations, and supply-to-demand comparisons.

## 🔍 Key Business Questions

This project helps answer the following questions:

1. What is the average inventory balance?
2. Which categories have higher inventory levels?
3. How does inventory balance change over time?
4. Is inventory sufficient to meet order demand?
5. How much inventory is overstocked or understocked?
6. What are the storage costs associated with excess inventory?
7. What is the average shipment delay?
8. What percentage of order items experience delays?
9. Which countries, markets, and shipment modes have higher delay rates?
10. How do shipment delays change month by month?
11. Which areas require improvements in inventory and delivery operations?

## 🧮 Calculated Fields and Business Logic

The Tableau workbook includes calculated fields for inventory, shipment delays, and supply-demand analysis.

### Shipment Delay Days

```text
DATEDIFF('day', [Order Date], [Shipment Date])
```

This calculates the number of days between the order date and shipment date. The workbook also compares the result with scheduled shipment days to calculate delay days.

### Delay Status

The workbook classifies shipment performance into categories such as:

- Early
- On Time
- 1–5 days late
- More than 5 days late

### Inventory Balance

```text
SUM([Warehouse Inventory])
-
SUM([Order Quantity])
```

This compares warehouse inventory with order quantity to calculate the inventory balance.

### Supply-to-Demand Ratio

```text
SUM([Warehouse Inventory])
/
SUM([Order Quantity])
```

This measures inventory relative to demand.

The workbook uses this ratio to classify supply conditions as oversupply, undersupplied, or aligned.

### Delay Rate

The workbook calculates the proportion of distinct orders with positive delay days relative to all distinct orders.

These formulas represent the business logic found in the workbook; field names and calculations should be checked against the final dataset before reuse.

## 🛠️ Tools and Technologies

- **Tableau Desktop**
- Tableau Calculated Fields
- Data Visualization
- KPI Cards
- Trend Analysis
- Interactive Filters
- Inventory Analysis
- Shipment Performance Analysis
- Supply Chain Analytics
- Business Intelligence

## 🔄 Project Workflow

```text
Inventory, Orders and Shipment Data
                  ↓
          Data Connection
                  ↓
        Data Preparation
                  ↓
       Calculated Fields
                  ↓
       Inventory Analysis
                  ↓
       Shipment Analysis
                  ↓
       Tableau Dashboards
                  ↓
       Business Insights
```

## 💡 Business Value

This project supports operational decision-making by helping businesses:

- Identify inventory imbalances.
- Monitor shipment delays.
- Track excess inventory and storage costs.
- Understand differences in delivery performance.
- Compare stock availability with order demand.
- Identify areas where supply chain operations may need improvement.

## 📁 Repository Structure

```text
Tableau-Inventory-Shipment-Analysis/
│
├── Tableau/
│   └── Tableau project.twb
│
├── Dataset/
│   ├── orders_and_shipments.csv
│   ├── inventory.csv
│   └── fulfillment.csv
│
├── Screenshots/
│   ├── Inventory_Balance.png
│   ├── Shipment_Performance.png
│   └── Business_Insights.png
│
└── README.md
```

*Note: The dataset files are referenced by the workbook. Add them to the repository only if you have the actual files and permission to share them.*

## 🚀 How to Use

1. Clone or download this repository.
2. Open `Tableau project.twb` using Tableau Desktop.
3. Connect the workbook to the required CSV files if Tableau cannot locate them.
4. Update the data-source paths if necessary.
5. Review the Inventory Balance and Shipment Performance dashboards.
6. Explore the available filters and worksheets to analyze different operational dimensions.

## 📚 Skills Demonstrated

- Tableau Dashboard Development
- Data Analysis
- Calculated Fields
- KPI Development
- Inventory Management Analytics
- Shipment Delay Analysis
- Supply-Demand Analysis
- Trend Analysis
- Data Visualization
- Business Intelligence

## 🎯 Project Outcome

This project demonstrates how Tableau can be used to analyze inventory and shipment operations through interactive dashboards and calculated business metrics.

It brings together inventory balance, shipment delays, storage costs, and supply-demand analysis to support better visibility into supply chain performance.

## 👨‍💻 Author

**Shaikh Mohmmad Ayyan**

Aspiring Data Analyst / Data Science Professional

**Skills:** Tableau | Power BI | Excel | SQL | Data Analytics | Data Visualization

---

⭐ If you find this project useful, feel free to explore the repository and give it a star!
# Tableau-project
