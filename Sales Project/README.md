 # Ferns & Petals Excel Sales Analysis Project



## Dashboard 

![](/Sales%20Project/Dashboard%20Screenshots/Dashboard.png)



## 📌 Problem

Ferns & Petals (FNP) is a gifting company that delivers products for occasions like Diwali, Raksha Bandhan, Valentine’s Day, Birthdays, and Anniversaries.

The business has transactional data across:

- Customers

- Orders

- Products

- Delivery timelines



## 👉 The challenge:

Turn raw data into insights that improve sales strategy, delivery efficiency, and customer experience.



## 🎯 Objective

Build a dashboard to analyze:

- Sales trends

- Customer behavior

- Product performance

- Answer key business questions.



## ❓ Key Business Questions

1) Total revenue
2) Average order & delivery time
3) Monthly sales trends (2023)
4) Top products by revenue
5) Average customer spending
6) Top 5 product performance
7) Top 10 cities by orders
8) Order quantity vs delivery time
9) Revenue by occasion
10) Product popularity by occasion


## 📈 Key Insights



### 💰 Revenue

Total Revenue: R586,176

Average Order Value: R4,652



### 📦 Delivery Performance

Delivery time varies with order size

Larger orders → slightly longer fulfillment



### 📅 Sales Trends

Clear seasonality across months

Peaks align with gifting occasions



### 🛍️ Product Performance

Top categories: Sweets, Soft Toys



### 🎉 Occasion Insights

High revenue from Anniversaries & Raksha Bandhan



### 🌍 Customer Behavior

Certain cities dominate order volume



## 📊 Dashboard Features

- Revenue overview

- Monthly trends

- Product & category performance

- Occasion-based insights

- City-level analysis

- Delivery time tracking



## 🧮 Formulas Used (Excel)



💰 Total Revenue
```excel
=SUM(Revenue)
```


🧾 Average Order Value
```excel
=SUM(Revenue) / COUNT(Order_ID)
```


⏱️ Delivery Time (Days)
```excel
=Delivery_Date - Order_Date
```


📦 Average Delivery Time
```excel
=AVERAGE(Delivery_Time)
```


📅 Monthly Sales
```excel
=TEXT(Order_Date,"MMM")
```
(Used in Pivot Table for grouping by month)



🏆 Top Products by Revenue
```excel
=SUMIFS(Revenue, Product_Name, Selected_Product)
```


👤 Customer Spending
```excel
=SUMIFS(Revenue, Customer_ID, Selected_Customer)
```


🌍 Orders by City
```excel
=COUNTIFS(City, Selected_City)
```


🎉 Revenue by Occasion
```excel
=SUMIFS(Revenue, Occasion, Selected_Occasion)
```


📊 Order Quantity vs Delivery Time
```excel
=CORREL(Order_Quantity, Delivery_Time)
```


## 🛠️ Tools Used

- Excel (Dashboard + Data Cleaning)

- Pivot Tables

- Charts & Visualizations



## 🧠 What I Learned

Turning business questions into data analysis
Building dashboards that tell a story
Identifying trends in sales and customer behavior


## 💡 Final Thoughts

This project focuses on business impact, not just visuals.



It answers:

What drives revenue?
When do customers buy?
Where should the business focus?


👉 Data → Insights → Decisions