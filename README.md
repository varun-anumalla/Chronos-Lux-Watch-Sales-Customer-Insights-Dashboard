# ⌚ Chronos Lux – Watch Sales & Customer Insights Dashboard (Power BI)

This project is a complete end-to-end data analytics and BI solution designed to analyze the sales performance, profitability, customer behavior, and return patterns of **Chronos Lux**, a fictional premium watch brand operating across India.

I built this project to understand how businesses use Power BI to drive decision-making through data-driven insights and interactive dashboards.  
The report consists of **three professional dashboards**, designed with a luxury-themed color palette to match the brand’s identity.

---
## 🖼 Dashboard Screenshots

### 📌 Dashboard 1 – Executive Sales Overview  
![Dashboard 1](https://github.com/varun-anumalla/Chronos-Lux-Watch-Sales-Customer-Insights-Dashboard/blob/main/Dashboard%20images/Dashboard-1.png)

---

### 📌 Dashboard 2 – Buyer Behavior & Product Insights  
![Dashboard 2](https://github.com/varun-anumalla/Chronos-Lux-Watch-Sales-Customer-Insights-Dashboard/blob/main/Dashboard%20images/Dashboard-2.png)

---

### 📌 Dashboard 3 – Detailed Performance Insights  
![Dashboard 3](https://github.com/varun-anumalla/Chronos-Lux-Watch-Sales-Customer-Insights-Dashboard/blob/main/Dashboard%20images/Dashboard-3.png)

---

## 🎥 YouTube Video Explanation
📌 **Watch Full Dashboard Walkthrough:**  
https://youtu.be/YOUR-LINK-HERE

---

## Business Problem Statement — No Insights Into Customer Behavior & Return Issues

"The company was facing frequent product returns and inconsistent customer ratings. But they had no way to understand which age groups were buying more, which sales channels were performing best, why customers were returning products, or which models had quality issues.

So I built Dashboard to analyze customer demographics, ratings, return reasons, and channel performance. This helps the business reduce returns, improve product quality, and create better marketing strategies."

This project focuses on solving important business questions such as:

- What are the total sales, profit, and units sold?
- Which watch models generate the highest sales?
- Which states and cities contribute the most revenue?
- How are sales and profit trending month-over-month?

- What is the average customer rating?
- Which age groups and genders purchase the most?
- How many orders are being returned and why?
- Which models have the highest return count?

- Which models are underperforming?
- How do sales compare between 2023 and 2024?
- How do customer ratings distribute?

The dashboard i created answers all these questions through clean ghaph visuals.

---

# 🛠 Tools & Technologies Used

### **1. Microsoft Excel**
- Initial cleaning  
- Formula-based columns  
- Structuring raw data  

### **2. Power Query**
- Data transformation  
- Removing nulls & fixing formats  
- Merging and shaping data  

### **3. Power BI**
- Data modeling  
- DAX calculations  
- Interactive visuals  
- Navigation buttons  
- Custom image slicers for watch models  

### **4. DAX (Data Analysis Expressions)**
Used for KPIs, calculated metrics, and analytical measures.

---

# 📊 Dataset Information

The dataset contains **10,000 rows** of realistic watch sales across India.

### **Columns Included**
- Order_ID  
- Order_Date  
- Product_ID  
- Model_Name  
- Unit_Price  
- Cost_Price  
- Quantity_Sold  
- Total_Sales  
- Total_Cost  
- Profit  
- Customer_ID  
- Customer_Age_Group  
- Customer_Gender  
- State  
- City  
- Sales_Channel  
- Customer_Rating  
- Return_Status  
- Return_Reason  

### **Model Names & Prices**
- Vector — ₹1000  
- Kinetic — ₹1500  
- Greenwich — ₹2000  
- Clarity — ₹3000  
- Elegance — ₹4000  
- Zenith — ₹5000  
- Eclipse — ₹6000  
- Tribute — ₹7000  
- Imperial — ₹9000  
- The Icon — ₹12000  

---

# 📐 Dashboard Structure

The project contains **three dashboards**, each targeting a different analytical purpose.


# 🧭 **Dashboard 1: Executive Sales Overview**

This dashboard gives a complete snapshot of company performance.

### **KPIs**
- Total Sales  
- Total Profit  
- Total COGS  
- Total Units Sold  
- Total Customers  

### **Visuals**
- Total Sales by State  
- Top 5 Best-Selling Models  
- Sales & Profit Trend by Month  
- Sales by Channel (Donut Chart)  
- Return Count by Model  
- Vertical watch image slicer  

---

# 🧭 **Dashboard 2: Buyer Behavior & Product Insights**

Focused on customer demographics, buying trends, and return reasons.

### **KPIs**
- Average Rating  
- Total Returned Orders  
- Avg Profit per Order  
- Average Order Value  
- Return Rate %  

### **Visuals**
- Map: Sales by State  
- Sales by City  
- Return Count by Reason (Treemap)  
- Sales by Customer Age Group  
- Watch image slicer panel  

---

# 🧭 **Dashboard 3: Detailed Performance Insights**

Deep-dive analytical page for trend and performance evaluation.

### **Visuals**
- Total Profit by Model  
- Total Customers by Gender  
- Sales by Year (2023 vs 2024)  
- Customer Rating Distribution  
- Bottom 5 Least Selling Models  

---


## 🧮 Key DAX Measures Used



```dax
DAshboard - 1
Total Sales = SUM('Watch sales'[Total_Sales])

Total Profit = SUM('Watch sales'[Profit])

Total COGS = SUM('Watch sales'[Total_Cost])

Total Units Sold = SUM('Watch sales'[Quantity_Sold])

Total Customers = DISTINCTCOUNT('Watch sales'[Customer_ID])

Dashboard -2 
Average Rating = AVERAGE('Watch sales'[Customer_Rating])

Total Returned Orders = CALCULATE(COUNTROWS('Watch sales'),'Watch sales'[Return_Status] = "Returned")

Avg Profit per Order = DIVIDE([Total Profit], COUNTROWS('Watch sales'))

Average Order Value (AOV) = DIVIDE([Total Sales], COUNTROWS('Watch sales'))

Return Rate % = DIVIDE([Total Returned Orders], COUNTROWS('Watch sales'), 0)

```

## 🔍 Key Usefull Insights From the Dashboards

### 🔥 Sales & Profit Insights
- The company generated **₹53M in total sales** and **₹21M profit**.
- **The Icon** is the top-selling and highest revenue-contributing model.
- Top-performing regions include **Maharashtra, Uttar Pradesh, Karnataka, and Tamil Nadu**.
- Sales trends peak during **March, May, and December**, indicating strong seasonal demand.

---

### 🛒 Customer Behavior Insights
- The average customer rating is **3.99**, showing good overall satisfaction.
- The **26–35 age group** accounts for the largest share of purchases.
- **Male customers** contribute the most to total sales.
- While **5-star ratings dominate**, there are noticeable low-rating clusters that may highlight quality issues.

---

### 📦 Return Insights
- The overall **return rate is 10.50%**, which is within acceptable retail ranges but still requires attention.
- Most common return reasons:
  - Poor Quality  
  - Color Mismatch  
  - Wrong Item  
  - Item Doesn’t Fit  
- Certain models experience slightly higher return frequencies and should be monitored closely.

---

### 🏆 Product Performance Insights
- **The Icon** and **Imperial** stand out as the most profitable models.
- **Vector, Kinetic, and Greenwich** are among the bottom-selling models.
- Year-over-year performance shows improvement, with **2024 sales higher than 2023**.

---





