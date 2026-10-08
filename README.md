# 🥛 Dairy Sales Analysis – Power BI Dashboard

## 📌 Project Overview

An interactive Power BI dashboard that analyzes dairy **sales, production and stock** data. It shows how much is produced, how much is sold and how much stays in stock, so that wastage can be reduced and production can be planned better.

The dashboard tracks **total revenue, quantity produced, quantity sold, stock count and average shelf life**, broken down by year, date, sales channel and product name.

---

## 📂 Repository Structure

```
Dairy-Sales-Analysis-PowerBI/
├── Dairy_Sales.pbix        # Power BI dashboard file
├── dairy_sales_data.csv    # Dataset used in the report
├── Screenshots/            # Dashboard page images
└── README.md               # Project documentation
```

---

## 🗂️ Dataset Description

The dataset contains the following information:

- **Date / Year:** when the sale or production took place
- **Product Name:** dairy product (for example milk, curd, butter, cheese)
- **Sales Channel:** where the product was sold
- **Quantity Produced:** units produced
- **Quantity Sold:** units sold
- **Stock Count:** units remaining in stock
- **Shelf Life:** number of days the product stays fresh
- **Revenue:** total sales amount

> Update this list to match the exact columns in your file.

---

## 📈 Dashboard Pages and Insights

### 🔹 Page 1: Sales Overview
**Purpose:** Quick view of overall business performance.

- Total revenue
- Total quantity sold
- Total quantity produced
- Revenue trend by year and date

**Visuals:** KPI cards, line chart, column chart

### 🔹 Page 2: Product and Sales Channel Analysis
**Purpose:** Compare products and channels.

- Revenue by product name
- Revenue and quantity sold by sales channel
- Best-selling and low-performing products

**Visuals:** Bar charts, donut chart, tables

### 🔹 Page 3: Stock and Shelf Life Analysis
**Purpose:** Find overstocked products and spoilage risk.

- Stock count by product
- Average shelf life by product
- Gap between quantity produced and quantity sold

**Visuals:** Bar charts, comparison table with conditional formatting

---

## 🧮 Key DAX Measures

```dax
Total Revenue = SUM('Dairy'[Revenue])

Total Quantity Produced = SUM('Dairy'[Quantity Produced])

Total Quantity Sold = SUM('Dairy'[Quantity Sold])

Total Stock Count = SUM('Dairy'[Stock Count])

Average Shelf Life = AVERAGE('Dairy'[Shelf Life])

Unsold Quantity = [Total Quantity Produced] - [Total Quantity Sold]
```

> Change table and column names to match your model.

---

## 🛠 Tools and Technologies

- Microsoft Power BI Desktop
- DAX (Data Analysis Expressions)
- Power Query (data cleaning)
- CSV dataset

---

## 🎯 What This Project Achieves

- ✔ Clear view of revenue by year, date, product and sales channel
- ✔ Comparison of production against sales to spot overproduction
- ✔ Identification of overstocked products using stock count
- ✔ Shelf-life insight to reduce wastage of fast-spoiling products
- ✔ Clean, interactive visuals with filters for year, product and channel

---

## 🚀 How to Use

1. Clone or download this repository
2. Open `Dairy_Sales.pbix` in Power BI Desktop
3. If the data does not load, go to **Transform Data > Data source settings** and point it to `dairy_sales_data.csv`
4. Click **Refresh**
5. Use the slicers to explore the dashboard

---

## 👤 Author

Mohammad Vakar Hasan 
Electrical Engineering , MANIT Bhopal 

