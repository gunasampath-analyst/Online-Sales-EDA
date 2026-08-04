# 📊 Online Sales Data Analysis | Exploratory Data Analysis (EDA)

> **Turning raw sales transactions into actionable business insights using Python, statistical analysis, and data visualization.**

![Python](https://img.shields.io/badge/Python-Data%20Analysis-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-purple)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)

---

# 📖 Executive Summary

In today's competitive retail landscape, organizations collect millions of sales transactions but often struggle to transform raw data into strategic business decisions. Effective data analysis enables businesses to identify profitable products, optimize pricing strategies, improve customer retention, reduce operational costs, and maximize revenue.

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on an online sales dataset containing over **51,000 transactions**. Using Python and industry-standard analytics libraries, the analysis explores sales performance, profitability, customer purchasing behavior, product performance, discount strategies, shipping costs, and regional trends.

The project demonstrates an end-to-end analytics workflow—from data cleaning and feature engineering to business insight generation and data storytelling.

---

# 🎯 Business Problem

Retail organizations face several critical business challenges:

- Which products and categories generate the highest profit?
- How do discounts influence profitability?
- Which customers contribute the greatest share of revenue?
- Which regions and markets perform best?
- How do shipping costs affect operational efficiency?

Without analytical insights, pricing, inventory, and marketing decisions rely on assumptions rather than evidence.

---

# 🎯 Project Objectives

The primary objective of this project is to transform transactional sales data into actionable business intelligence that supports strategic decision-making.

### Objectives

- Analyze overall sales and profit performance
- Identify the most and least profitable product categories
- Discover top-performing and loss-making products
- Evaluate the relationship between discounts and profitability
- Analyze customer purchasing behavior using the Pareto (80/20) Principle
- Compare business performance across markets and regions
- Evaluate shipping costs across different shipping modes
- Measure profit margins across categories and markets
- Generate business recommendations based on analytical findings

---

# 📂 Dataset Overview

| Attribute | Details |
|-----------|---------|
| Dataset | Online Sales Dataset |
| Source | Kaggle |
| Records | **51,290** |
| Features | **24+ Columns** |
| Data Type | Retail Sales Transactions |

### Dataset Includes

- Customer Information
- Product Information
- Sales & Profit
- Quantity & Discount
- Shipping Cost
- Order Details
- Category & Sub-Category
- Market & Region
- Order & Shipping Dates

### Feature Types

| Type | Examples |
|------|----------|
| Numerical | Sales, Profit, Quantity, Discount, Shipping Cost |
| Categorical | Category, Segment, Market, Region, Ship Mode |
| Date | Order Date, Ship Date |

---

# 🛠 Tech Stack

| Technology | Purpose |
|------------|----------|
| Python | Data Analysis |
| Pandas | Data Cleaning & Manipulation |
| NumPy | Numerical Computing |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Jupyter Notebook | Development Environment |

---

# 🔄 Project Workflow

```text
Raw Dataset
      │
      ▼
Data Understanding
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Statistical Analysis
      │
      ▼
Data Visualization
      │
      ▼
Business Insights & Recommendations
```

---

# 🧹 Data Preparation

The dataset was cleaned and prepared using industry-standard preprocessing techniques.

### Data Cleaning

- Inspected dataset structure and data types
- Removed duplicate records
- Checked for missing values
- Converted date columns into datetime format
- Validated numerical and categorical variables

### Feature Engineering

Additional analytical features were created, including:

- Profit Margin
- Order Year
- Week Number
- Monthly Sales Trend

These engineered features enabled deeper trend analysis and business reporting.

---

# 📊 Business Questions Addressed

## 💰 Sales & Profit Analysis

- Which categories generate the highest revenue?
- Which products produce the highest profit?
- Which products consistently generate losses?

---

## 👥 Customer Analytics

- Which customers contribute the highest revenue?
- Does the business follow the Pareto (80/20) Principle?
- Which customer segments create the greatest business value?

---

## 📦 Product Performance

- Which products drive business growth?
- Which products reduce overall profitability?
- Which categories have the strongest profit margins?

---

## 🚚 Operational Analysis

- How do shipping costs vary across markets?
- Which shipping modes incur the highest costs?
- Does higher shipping cost correlate with higher sales?

---

## 🌍 Market Analysis

- Which markets generate the highest sales?
- Which regions contribute the greatest profitability?
- Where should future business expansion focus?

---

# 📈 Exploratory Analysis

The project includes comprehensive analysis across multiple business dimensions:

- Data Cleaning
- Descriptive Statistics
- Sales Performance
- Profit Analysis
- Customer Analysis
- Product Performance
- Category Analysis
- Market & Regional Analysis
- Discount Analysis
- Shipping Cost Analysis
- Correlation Analysis
- Profit Margin Analysis
- Pareto Analysis (80/20 Rule)

---

# 💡 Key Business Insights

## 📈 Revenue Performance

- Technology products generated the highest overall profit.
- Sales performance varied significantly across categories and regions.

---

## 💰 Profitability

- Higher discount levels generally reduced profit margins.
- Several products generated strong sales but produced negative profits.

---

## 👥 Customer Insights

- A relatively small group of customers contributed a significant portion of total revenue, consistent with the Pareto Principle.

---

## 🚚 Operational Insights

- Shipping costs differed substantially across markets and shipping modes.
- Certain shipping methods incurred higher operational expenses without proportional profit gains.

---

## 🌍 Regional Performance

- Regional analysis identified both high-performing markets and underperforming regions requiring strategic attention.

---

# 📌 Business Recommendations

- Optimize discount policies for low-margin products.
- Prioritize inventory for high-profit product categories.
- Strengthen retention initiatives for high-value customers.
- Review pricing strategies for consistently loss-making products.
- Optimize shipping methods to reduce logistics costs.
- Expand investment in high-performing markets while improving weaker regions.

---

# 📷 Project Visualizations

### 📈 Sales vs Profit Analysis
![Sales vs Profit Analysis](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/0f65966418904ad1cf95a557a5eb274b29dc8990/sales_vs_profit_analysis.png)

### 🌍 Region-wise Sales and Profit
![Region-wise Sales and Profit](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/0f65966418904ad1cf95a557a5eb274b29dc8990/region_wise_sales_profit.png)

### 🚚 Shipping Cost Analysis
![Shipping Cost Analysis](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/0f65966418904ad1cf95a557a5eb274b29dc8990/shipping_cost_analysis.png)

### 🔥 Correlation Heatmap
![Correlation Heatmap](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/0f65966418904ad1cf95a557a5eb274b29dc8990/correlation_heatmap.png)

### 🌍 Average Profit Margin by Market
![Average Profit Margin by Market](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/30626f7591c1a85212b54e4c48d4daddd5d7cef9/avg_profit_by_market.png)

### 📉 Discount Distribution
![Discount Distribution](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/30626f7591c1a85212b54e4c48d4daddd5d7cef9/dicount.png)

### 📈 Yearly Profit by Category
![Yearly Profit by Category](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/30626f7591c1a85212b54e4c48d4daddd5d7cef9/profit_by_category.png)

### 📦 Sales by Category
![Sales by Category](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/30626f7591c1a85212b54e4c48d4daddd5d7cef9/sales_by_category.png)

### 📉 Top Loss-Making Products
![Top Loss-Making Products](https://github.com/gunasampath-analyst/Online-Sales-EDA/blob/30626f7591c1a85212b54e4c48d4daddd5d7cef9/top_10_loss_products.png)

---

# 📁 Project Structure

```text
Online-Sales-EDA
│
├── data
│   └── online_sales_dataset.csv
│
├── notebooks
│   └── online_sales_eda.ipynb
│
├── images
│   ├── monthly_sales_profit_trend.png
│   ├── category_analysis.png
│   ├── sales_vs_profit.png
│   ├── discount_vs_profit.png
│   ├── correlation_heatmap.png
│   ├── pareto_chart.png
│   ├── shipping_cost_analysis.png
│   └── region_analysis.png
│
├── requirements.txt
│
└── README.md
```

---

# 🚀 Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Statistical Analysis
- Data Visualization
- Business Storytelling
- Customer Analytics
- Profitability Analysis
- Python Programming
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

# 🔮 Future Enhancements

- Build an interactive Power BI dashboard
- Develop a Streamlit analytics application
- Implement sales forecasting models
- Perform customer segmentation using clustering
- Apply machine learning for profit prediction
- Integrate SQL-based business analysis
- Create automated KPI dashboards

---

# ▶️ How to Run the Project

Clone the repository:

```bash
git clone https://github.com/yourusername/Online-Sales-EDA.git
```

Navigate to the project directory:

```bash
cd Online-Sales-EDA
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and run all cells.

---

# 👨‍💻 Author

## Guna Sampath

**Aspiring Data Analyst | MCA Student**

Passionate about transforming raw business data into actionable insights through **Python, SQL, Power BI, Excel, and Business Intelligence**.

### Technical Skills

- Python
- SQL
- Power BI
- Excel
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Data Visualization
- Business Intelligence
- Exploratory Data Analysis (EDA)

---

# 📄 License

This project is licensed under the **MIT License**.

---

## ⭐ If you found this project useful, consider giving it a Star!
