# 📊 Superstore Sales Analysis

This project analyzes sales performance using the [Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) to uncover insights about profit, quantity, sales trends, discount impact, and customer behavior. The goal is to inform strategic decisions by identifying patterns in sales and profitability.

---

## 📁 Dataset Overview

The dataset contains transaction-level records of customer purchases across:
- **Order Details**: Date, Quantity, Sales, Profit, Discount
- **Customer Info**: Segment, Region, State, Customer Name, Customer ID
- **Product Info**: Category, Sub-Category, Product Name
- **Shipping**: Ship Mode, Shipping Cost

---

## 🔍 Exploratory Data Analysis (EDA)

### 🧹 Data Preprocessing
- Removed nulls and duplicates
- Standardized column names
- Extracted year, month, and day from order dates

### 📦 Univariate Analysis
- Profit and Sales show high variance with multiple outliers
- Discounts mostly fall between 0–20%
- Quantity typically ranges between 1 and 5

### 📆 Time-based Trends
- 📈 Consistent growth in orders from 2014 to 2017
- 🗓️ November and December are peak months
- 📉 End-of-month spikes in quantity, but 31st sees low orders

### 👥 Segment, Region & Shipping Analysis
- **Consumer segment** dominates in both sales and profit
- **West & East** regions are most profitable
- **Standard Class** is most widely used shipping method

### 📊 Category & Sub-category Performance
- **Technology** is the most profitable and highest-selling category
- **Tables** sub-category shows high losses despite high sales
- **Copiers** and **Phones** are consistently profitable

### 🧾 Discount Impact
- High discounts (>30%) often lead to losses
- Low discounts still maintain high sales, showing deep discounting isn't always needed

### 🔁 Sales, Profit & Quantity Relationships
- Positive correlation between Sales & Quantity
- No clear trend between Profit & Quantity; losses occur at all levels

### 👤 Top Customers Analysis
- Top 10 customers by quantity differ from those by sales or profit
- Indicates different customer value types (high volume vs. high margin)

---

## 📌 Key Business Insights

1. **Technology & Office Supplies** are high-margin categories.
2. **Heavy discounts** lead to losses—optimize discount strategy.
3. **Tables sub-category** needs cost/pricing evaluation.
4. **Focus marketing on high-quantity but low-revenue customers**.
5. **End-of-month surge in orders** suggests promotional influence.

---

## 🛠️ Tools Used

- **Python**
  - pandas, numpy
  - matplotlib, seaborn
- **Jupyter Notebook**

---

## 📁 Folder Structure

