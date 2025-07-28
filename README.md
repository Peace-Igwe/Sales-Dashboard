# 📊 Luson Blu Sales Dashboard — FMCG Distribution Insights

Welcome to the Luson Blu Sales Dashboard repository! This Power BI project provides actionable insights into product performance, customer behavior, and warehouse operations for Luson Blu, a leading FMCG distributor in Nigeria.

---

## 🏢 Client Overview

**Luson Blu** is a major distributor in the fast-moving consumer goods (FMCG) space, operating across multiple regions and serving diverse customer segments. Despite their scale, they faced data visibility challenges in:

- 📦 Warehouse capacity and stock risk
- 🛒 Product profitability and discount impact
- 📈 Regional sales trends and channel performance
- 👥 Customer loyalty segmentation

---

## 💼 Business Challenge

The leadership team needed a single source of truth to:

- Track sales performance year-to-date (YTD)
- Identify high-margin products beyond top revenue drivers
- Understand customer purchasing behavior
- Optimize warehouse efficiency and flag stock risks

---

## 🎯 My Role

As the **Data Analyst**, I was responsible for:

✔️ Cleaning and transforming raw sales data using **Power Query**  
✔️ Designing a **star schema** data model  
✔️ Writing advanced **DAX measures**  
✔️ Creating a visually engaging and interactive **Power BI dashboard**  
✔️ Delivering a concise one-page **business insight report**

---

## 🔧 Solution Breakdown

### 🔄 Power Query Data Transformation

- Removed duplicates in `Sales_Data`
- Cleaned nulls in `Discount` column and converted % strings to decimals
- Merged `Warehouse` data to calculate stock overflow
- Created calculated columns for loyalty scores and profit breakdowns

---

### 🧩 Data Modeling – Star Schema

- **Fact Table**: `Sales_Data`  
- **Dimension Tables**: `Customer`, `Product`, `Warehouse`, `Date`  
- Clean relationships enabled seamless cross-filtering and dynamic analysis

---

### 🧠 DAX Highlights

| Insight                     | DAX Logic                                                   |
|-----------------------------|-------------------------------------------------------------|
| **Profit Margin %**         | `DIVIDE(Gross Profit, Net Sales) * 100`                     |
| **Sales YTD**               | `TOTALYTD(Net Sales, Date)`                                 |
| **Top Product by Quantity** | Calculated using `TOPN()` and `SUMX()`                      |
| **Loyalty Score**           | Categorized based on cumulative purchase volume             |
| **% Capacity Used**         | Ratio of quantity sold to warehouse capacity                |

📄 View the full DAX formulas in the `Dax for Luson Blu Sales Analysis.docx` file.

---

## ✨ Key Insights

- 🔥 A mid-range product—not in the top 10 by volume or revenue—drove the **highest profit margin**, signaling a powerful bundling opportunity.
- 🧊 Some warehouses had high capacity usage with **low stock turnover**, indicating inventory risk.
- 🧑‍🤝‍🧑 Customers with mid-range loyalty scores contributed disproportionately to sales, revealing untapped retention strategies.

---

## 📦 Deliverables

- ✅ Power BI `.pbix` file with dynamic, ready-to-present visuals  
- ✅ Star-schema modeled dataset  
- ✅ Insight report (1-pager)  
- ✅ DAX calculation reference document  

---

## 📸 Screenshots

| 📍 Data Model                                    | 📈 Dashboard Sample               |
|--------------------------------------------------|-----------------------------------|
| ![Data Model](https://github.com/Peace-Igwe/Power-App-Request-Portal/blob/main/Sales-Dashboard/Luson-Blu-Analysis-Data-Model.png) | ![Dashboard](https://github.com/Peace-Igwe/Power-App-Request-Portal/blob/main/Sales-Dashboard/d8e571fa-07b8-41bb-bba7-74851884fd5c.png) |
|

---

## 📁 Repository Structure

