# 📊 Superstore Sales Analysis

This project analyzes sales performance using the [Superstore Dataset] ("https://www.kaggle.com/datasets/vivek468/superstore-dataset-final") to uncover patterns in profitability, product performance, discounts, and customer behavior. The aim is to generate actionable insights that drive smarter decisions for sales, marketing, and operations.

---

## 📁 Dataset Overview

The dataset contains 9,994 records of customer transactions, including:
- **Order Details**: Row ID, Order ID, Order Date, Ship Date, Sales, Quantity, Discount, Profit
- **Customer Info**: Customer ID, Customer Name, Segment, Region, State, City, Country, Postal Code
- **Product Info**: Product ID, Product Name, Sub-Category, Category
- **Shipping**: Ship Mode

---

## 🔍 Exploratory Data Analysis (EDA)

### 🧹 Data Preprocessing
- Removed nulls and duplicates
- Standardized column names
- Extracted Year, Month, and Day from Order Date
- Added profit margin, shipping duration, and mapped date features for trend analysis

### 📦 Univariate & Bivariate Analysis
##### 💰 Sales, Profit & Discount
- Sales and profit show high variance with extreme outliers.
- Discounts are mostly below 20%, but higher discounts (>30%) often lead to losses.
  
##### 📦 Quantity
- Most orders are small in size (1–5 items), but large quantity orders show diverse profit outcomes.
- No strong correlation between quantity and profit—some high-quantity orders result in losses.

### 📆 Time-based Trends
- 📆 Yearly: Orders grew from ~7.9K in 2014 to ~12.3K in 2017, showing strong business expansion.
- 📅 Monthly: November and December are peak months in both quantity and sales.
- 📅 Daily: End-of-month ordering spikes are frequent (except the 31st, which sees a drop).

### 👥 Segment, Region & Shipping Analysis
- Consumer Segment dominates in both sales and profit.
- West and East Regions lead in profitability; South underperforms in profit.
- Standard Class is the most used shipping method; profitability across modes is relatively even.

### 🛍️ Category & Sub-category Performance
- Technology is the top-performing category in both sales and profit.
- Tables sub-category has high sales but consistent losses—indicating pricing or cost issues.
- Phones and Copiers are highly profitable products with steady performance.

### 💳 Discount Strategy Insights
- High discounts (>30%) often lead to losses
- Low discounts still maintain high sales, showing deep discounting isn't always needed

### 🔁 Relationship Analysis
- Sales vs. Quantity: Positive trend, but variability indicates different price points.
- Profit vs. Quantity: No clear pattern—losses occur at nearly all quantity levels.
- Discount vs. Quantity: No linear trend, but high discounts can drive volume at the cost of margin.

### 👤 Customer Insights
- Top customers by quantity are not the same as those by profit or sales.
- High-volume buyers may not be high-value buyers—indicating potential for segmentation and targeted strategies.

### 🌍 Geographical Insights
- California is the top contributor to both sales and profit.
- Texas, despite high sales, has poor profitability—possibly due to discounting or operational inefficiencies.
- Some states (e.g., Ohio, Pennsylvania) yield losses, demanding a pricing or delivery strategy review.
  
---

## 📌 Actionable Business Conclusions

1. ✅ Technology & Phones/Copiers drive both sales and profitability — prioritize them in marketing and inventory.
2. ⚠️ Tables need cost evaluation or pricing revision — consistently results in losses.
3. 💡 Customer Segmentation: Volume buyers ≠ high-margin buyers. Differentiate loyalty and rewards based on profit, not quantity alone.
4. 🛑 Limit Discounts over 30% unless part of strategic clearance — they heavily hurt margins.
5. 📍 Texas and Ohio require deeper analysis — either change fulfillment strategies or adjust discounts and pricing.
6. 📦 Standard Class shipping is preferred — can continue being a default mode unless express delivery is explicitly requested.
7. 📈 End-of-month sales surge could indicate influence of monthly targets/promotions — explore expanding mid-month incentives.

---

## 🛠️ Tools Used

- Python: pandas, numpy, datetime
- Visualization: matplotlib, seaborn
- Notebook : VSCode

---

## 📁 Folder Structure

