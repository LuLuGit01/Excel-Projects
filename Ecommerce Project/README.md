# 📊 Ecommerce Data Analysis Project



## Dashboard 

![](/Ecommerce%20Project/Dashboard%20Screenshots/Ecommerce%20Project%20Dashboard%20Screenshot.jpg)



## 📌 Overview

This project explores transactional sales data to uncover insights into customer behavior, product performance, and delivery efficiency.



Using Excel, the analysis transforms raw data into actionable insights through formulas, pivot tables, and KPI tracking.



---



## 🎯 Objectives

- Analyze sales trends and product demand  

- Understand customer purchasing patterns  

- Evaluate delivery performance  

- Build KPI-driven insights  



---



## 📂 Dataset

The dataset includes ~2,400 transactions with:



- Transaction ID  

- Product  

- Quantity  

- Days to Deliver  

- Week Number  

- Gender  

- Channel  

- Rating  

- Amount  



---



## 🛠️ Tools Used

- **Excel** – Data cleaning & analysis  

- **Pivot Tables** – Aggregation & summarization  

- **Data Visualization** – Charts & dashboards  



---



## 🧮 Formulas Used



### 📊 Core KPIs



Total Orders:
```excel
=COUNTA(Data[TX ID])
```


Total Quantity:
```excel
=SUM(Data[Quantity])
```


Total Revenue:
```excel
=SUM(Data[Amount])
```


Average Rating:
```excel
=AVERAGE(Data[Rating])
```




**🚚 Delivery Metrics**

Average Delivery Time:
```excel
=AVERAGE(Data[Days to Deliver])
```


Fast Deliveries (≤1 Day):
```excel
=COUNTIF(Data[Days to Deliver], "<=1")
```


**📦 Order Insights**

Most Common Order Size (Example - Qty 2):
```excel
=COUNTIF(Data[Quantity], 2)
```


Large Orders (>3 Items):
```excel
=COUNTIF(Data[Quantity], ">3")
```


**📱 Segment Analysis**

Orders by Channel (App):
```excel
=COUNTIF(Data[Channel], "App")
```


Revenue by Channel:
```excel
=SUMIF(Data[Channel], "App", Data[Amount])
```


Average Rating (Female Customers):
```excel
=AVERAGEIF(Data[Gender], "Female", Data[Rating])
```


### 📊 Pivot Tables

Pivot tables were used to summarize and explore the dataset:

**🔹 Sales by Channel & Gender**

- Rows: Channel

- Columns: Gender

- Values: Count of Orders

- Insight: Channel performance varies across customer segments

**🔹 Product Performance**

- Rows: Product

- Columns: Gender

- Values: Sum of Quantity

- Insight: Identifies top-performing products

**🔹 Order Size Distribution**

- Rows: Quantity

- Values: Count of Orders

- Insight: Most orders fall between 1–3 items

**🔹 Delivery Time Analysis**

- Rows: Days to Deliver

- Values: Count of Orders

- Insight: Majority of deliveries occur within 1–2 days



### 📈 Key Insights

- Most customers purchase 1–3 items per order

- Average delivery time is ~2 days

- Certain products significantly outperform others

- Sales channels show different performance across genders



### 📊 KPIs

- Total Orders: ~2,400

- Total Quantity Sold: ~11,997

- Average Rating: ~4.0

- Average Delivery Time: ~2 days