# Retail Profit Optimization  
## Inventory, Demand & Pricing Sensitivity Analytics

---

## 📌 Project Overview

This project began as an operational analytics initiative focused on inventory efficiency and demand forecasting.

During analysis, the system exhibited structural stability across inventory and demand metrics. Rather than forcing artificial insights, the project evolved into a **driver-based pricing optimization simulation**, introducing elasticity-driven What-If modeling to evaluate profit sensitivity under varying market conditions.

The final solution transitions from descriptive reporting to prescriptive financial modeling.

---

## 🎯 Business Objectives

- Evaluate inventory health and capital efficiency  
- Measure demand stability and forecast accuracy  
- Quantify revenue leakage and volatility exposure  
- Model pricing sensitivity under varying elasticity assumptions  
- Identify profit-maximizing price levels  

---

## 📊 Dashboard Structure

### Page 1 – Executive Summary
- Total Revenue  
- Gross Profit  
- Gross Profit Margin  
- Closing Inventory  
- Stock Pressure Rate  
- Stock Pressure Count  
- Revenue Contribution by Category  
- Revenue Trend Over Time  

---

### Page 2 – Inventory Efficiency
- Inventory Velocity  
- Days of Cover  
- Inventory Value  
- Capital-Adjusted Margin %  
- Inventory Allocation by Category  
- Inventory Coverage by Category  
- Days of Cover by Store  
- Inventory Volume vs Value Analysis  

---

### Page 3 – Demand & Forecast Stability
- Forecast Accuracy %  
- Demand Volatility  
- Lost Revenue %  
- Lost Units  
- Actual vs Forecast Sales Trend  
- Revenue Leakage by Category  
- Demand Volatility by Category  

---

### Page 4 – What-If Pricing Simulation (Core Feature)

Interactive simulation engine allowing users to:

- Adjust **Price Change %**
- Modify **Elasticity Assumption**
- Observe impact on:
  - Simulated Revenue
  - Simulated Gross Profit
  - Simulated Margin %
  - Revenue Impact
  - Profit Impact
  - Optimal Price Change %

Includes a dynamic profit optimization curve:

> Profit = f(Price Change %, Elasticity)

---

## 🧠 Key Insights

- Operational metrics indicate a structurally stable system.
- Inventory turnover and demand forecasting show low variance.
- Profitability is highly sensitive to demand elasticity assumptions.
- Under moderate elasticity (-1), price increases maximize profit.
- Under high elasticity (-3), optimal pricing converges near baseline (~+2%).
- Margin expansion does not necessarily imply profit maximization.
- Pricing strategy must be elasticity-aware.

---

## 🏗 Data Model

**Grain:** Daily × Store × Product  

### Fact Table  
`fact_inventory_sales_daily`

Includes:
- Units Sold  
- Inventory Levels  
- Pricing & Discounts  
- Demand Forecast  
- Derived Revenue & Profit Metrics  

### Dimension Tables
- `dim_date`
- `dim_product`
- `dim_store`

---

## 🛠 Tools & Technologies

- SQL (Staging, Dimensional Modeling, Views, QA Validation)
- Power BI (DAX, What-If Parameters, Simulation Modeling)
- Driver-Based Financial Modeling
- Elasticity-Based Demand Simulation

---

## 🔬 Modeling Enhancements

- Fixed unit cost modeling (decoupled from price)
- Elasticity-driven unit adjustment
- Non-negativity constraint on simulated demand
- Separate scenario-based and curve-based measures
- Profit optimization curve visualization

---

## 📈 Analytical Progression

Descriptive Analytics → Diagnostic Insights → Prescriptive Modeling  

This project demonstrates how operational analysis can evolve into decision-focused strategy modeling using structured driver logic.

---

## 📂 Repository Structure

- `readme.md`
- `sql` -
- `sql/01_stagging`
- `sql/02_dim_&_fact_transformation.sql`
- `sql/03_profitability_view.sql`
- `Airline_Profitability_&_Cost_Driver_Analytics_v1`
- `screenshot` -
- `screenshot/01_Profitability_Deep_Dive`
- `screenshot/02_Cost_Drivers_&_Efficiency`
- `screenshot/03_Network_Performence_Route_Carrier`


---

## 👤 Author
**Indranil Mukherjee** 
Data Analyst | SQL | Power BI | Business Modeling  

Focused on transforming data into structured decision frameworks.
