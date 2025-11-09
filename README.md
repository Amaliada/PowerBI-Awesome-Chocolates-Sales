# 🍫 Power BI – Awesome Chocolates Sales Dashboard

An interactive **Power BI dashboard** built to analyze the sales performance of the fictional company *Awesome Chocolates*.  
The report provides insights into **sales trends, shipments, profit margins, and regional performance** across multiple markets.  
It demonstrates strong **data modeling, DAX calculations, and data visualization** skills for business analytics.

---

## 🧭 Project Overview

This dashboard was designed to provide a complete view of business performance by tracking:
- 📦 Shipments over time
- 💰 Total Sales and Profit
- 🌍 Regional performance (Australia, Canada, India, New Zealand, UK, USA)
- 🧑‍💼 Salesperson-level performance and KPIs
- ⚙️ Key operational metrics such as *Total Boxes*, *Total Shipments*, and *Profit %*

Each visual and metric is interactive, allowing users to filter and drill down by product category, region, or salesperson.

---

## 🧩 Key Features

- 📊 **Dynamic KPIs:** Total Sales, Profit, Shipments, and Boxes with month-over-month variance  
- 🗺️ **Regional Insights:** Compare performance across six global markets  
- 📈 **Trend Analysis:** Track shipments and sales by month using line and bar charts  
- 💼 **Salesperson Performance:** Evaluate individual sales contribution and profit margins  
- ⚡ **DAX Measures:** Used for profitability ratios, MoM percentage changes, and performance gauges  
- 🧠 **Interactive Filters:** Segment by product type (*Bars, Bites, Other*) or by country  

---

## 🧱 Data Modeling

- **Data Source:** Provided dataset from the fictional *Awesome Chocolates* company  
- **Data Model:** Star schema — fact tables for sales & shipments linked to dimension tables (Products, Salesperson, Country)  
- **Data Transformation:** Cleaned and reshaped using **Power Query (M language)**  
- **Key DAX Measures:**
  ```DAX
  Total Sales = SUM(FactSales[Sales])
  Total Profit = SUM(FactSales[Profit])
  Profit % = DIVIDE([Total Profit], [Total Sales])
  MoM Sales % = 
      VAR PrevMonth = CALCULATE([Total Sales], DATEADD(DimDate[Date], -1, MONTH))
      RETURN DIVIDE([Total Sales] - PrevMonth, PrevMonth)

  🧰 Tools & Technologies
Category	Tools Used
Data Visualization	Power BI Desktop
Data Preparation	Power Query
Data Modeling	Star Schema
Formulas & Measures	DAX
Report Design	Bookmarks, Buttons, Filters, Custom Visuals

📊 Dashboard Preview
🖼️ Sales Overview Page

📦 Shipments & Trend Analysis

💼 Salesperson Performance


📈 Insights Summary

Total Sales: $2M

Total Shipments: 323

Average Profit Margin: ~60%

Top-performing Region: India

Highest Salesperson Profit %: 80.8%

Weakest Region by MoM Growth: -3.7%

The dashboard highlights how sales volumes and profit percentages vary by geography and salesperson efficiency.

💡 Learning Outcomes

Through this project, the following data analytics and BI skills were applied:

Data cleaning and transformation with Power Query

DAX formula creation for metrics and KPIs

Visual storytelling and report design in Power BI

Performance analysis and business insight presentation

🪪 License

This project is for educational and portfolio purposes only.
© 2025 Dana Nica

👩‍💻 Author

Dana Nica
📍 Lugoj, Romania
🔗 GitHub Profile

“Transforming business data into actionable insights through Power BI and data storytelling.”
