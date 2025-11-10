# 🚗 Car Sales Dashboard | Power BI Project
## 📊 Overview
This project presents an **interactive Car Sales Dashboard** built in **Power BI** to analyze car sales performance across different regions, brands, and time periods.  
It provides a complete picture of **sales trends, car model performance, and dealership insights**, empowering data-driven decisions.

The dashboard answers key business questions such as:
- Which **brands and dealers** generate the most sales?
- How do **sales trends** vary by **month or region**?
- What are the **YTD (Year-to-Date)** and **MTD (Month-to-Date)** growth metrics?
- Which **car colors and models** perform best in the market?

---

## 🧠 Project Goals
✅ Track **overall sales performance (YTD, MTD)**  
✅ Identify **top-performing car brands and models**  
✅ Analyze **dealer and regional sales distribution**  
✅ Visualize **KPIs** such as sales growth, average sales, and cars sold  
✅ Provide an **interactive experience** through filters and drill-downs  

---

## ⚙️ Tools & Technologies Used
| Tool | Purpose |
|------|----------|
| **Power BI** | Data modeling and visualization |
| **DAX (Data Analysis Expressions)** | Custom calculations and KPIs |
| **Excel / CSV Dataset** | Data source for car sales |
| **Power Query** | Data cleaning and transformation |

---

## 🧮 DAX Measures
Some of the key **DAX formulas** used in the project:

```DAX
-- Year-to-Date (YTD) Total Sales
YTD Total Sales = TOTALYTD(SUM(CarSales[Total Sales]), 'Calendar'[Date])

-- Month-to-Date (MTD) Total Sales
MTD Total Sales = TOTALMTD(SUM(CarSales[Total Sales]), 'Calendar'[Date])

-- Total Cars Sold
Total Cars Sold = COUNTROWS(CarSales)

-- YTD Average Sales
YTD Avg Sales = AVERAGEX(VALUES(CarSales[Dealer_Name]), [YTD Total Sales])

-- Sales Growth %
Sales Growth % = DIVIDE(([YTD Total Sales] - [MTD Total Sales]), [MTD Total Sales])


---

### 🚀 How to Use
1. Download the `.pbix` file from this repository.  
2. Open it in **Power BI Desktop**.  
3. Refresh the data connection if needed.  
4. Interact with filters and visuals to explore insights.

### 👨‍💻 Author
**Ravi Dhakad**  
📧 raviiidhakad@gmail.com  
🔗 https://www.linkedin.com/in/ravi-dhakad-9b3353245/
💻 [GitHub](https://github.com/raviiidhakad)

---

### 🏁 Conclusion
💡 This Power BI dashboard transforms raw car sales data into clear, actionable business insights, enabling data-driven decision-making.
🚀 It showcases my ability to design, model, and visualize data effectively — turning analytics into impact.
