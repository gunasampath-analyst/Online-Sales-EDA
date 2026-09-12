# Global Superstore Sales & Profitability Analysis

> Exploratory analysis of 51K+ global sales transactions to identify sales drivers, profitability patterns, loss-making products, market performance, shipping costs, and potential areas for business improvement.

---

## 📌 Project Overview

Businesses generate large volumes of transactional data, but raw sales records do not immediately reveal which products, markets, categories, or regions are driving business performance.

This project performs **Exploratory Data Analysis (EDA)** on the Global Superstore dataset to understand sales and profitability patterns across products, categories, markets, customers, shipping modes, and regions.

The analysis combines data cleaning, feature engineering, statistical analysis, correlation analysis, and data visualization to turn transactional sales data into business-oriented insights.

---

## 🎯 Business Problem

Management needs to understand:

- Which markets and countries generate the most sales?
- Which product categories and sub-categories drive revenue?
- Which products contribute significantly to sales?
- Where are loss-making products appearing?
- How are shipping costs distributed across markets?
- Which regions contribute the most sales and profit?
- How are discounts distributed across transactions?
- What relationships exist between sales, profit, quantity, and shipping cost?

The goal is to move beyond simply reporting sales and identify **patterns that can support better commercial and operational decisions**.

---

## 🎯 Business Objectives

The analysis focuses on:

- Analyzing overall sales and profit performance
- Identifying high-performing categories and products
- Identifying loss-making products
- Evaluating discount patterns
- Understanding customer purchasing behavior
- Comparing market and regional performance
- Analyzing shipping costs
- Examining sales and profit relationships
- Identifying correlations between important business variables
- Generating actionable business observations

---

## ❓ Key Business Questions

1. Which countries generate the highest sales?
2. Which product categories contribute the most revenue?
3. Which sub-categories and products are the strongest sales contributors?
4. Which markets generate the highest sales?
5. How is order volume distributed across shipping modes?
6. Which products generate negative profit?
7. How are shipping costs distributed across global markets?
8. How does profit change across product categories over time?
9. What is the relationship between sales, profit, quantity, and shipping cost?
10. Which regions contribute the most sales and profit?

---

# 📊 Dataset

### Dataset: Global Superstore

The project uses a transactional Global Superstore sales dataset.

| Attribute | Details |
|---|---|
| Rows | **51,290** |
| Columns | **27** |
| Time period | **2011–2014** |
| Data type | Transactional sales data |
| Categories | Furniture, Office Supplies, Technology |
| Markets | APAC, EU, US, LATAM, EMEA, Africa, Canada |
| Customer segments | Consumer, Corporate, Home Office |
| Shipping modes | Standard Class, Second Class, First Class, Same Day |

### Important Fields

- Order Date
- Ship Date
- Order ID
- Customer ID
- Customer Name
- Product ID
- Product Name
- Category
- Sub-Category
- Sales
- Profit
- Quantity
- Discount
- Shipping Cost
- Market
- Region
- Country
- Segment
- Ship Mode
- Order Priority

---

# 🧹 Data Preparation

The notebook begins by inspecting the structure and quality of the dataset before performing analysis.

### Data Quality Checks

- Dataset dimensions were examined.
- Column information and data types were reviewed.
- Missing values were analyzed.
- Duplicate records were checked.
- Statistical summaries were generated for numerical variables.

### Duplicate Check

The dataset contains:

**0 duplicate records**

This provides a clean basis for the subsequent exploratory analysis.

---

# 🧮 Feature Engineering

A **Profit Margin** field was created at the transaction level using:

`Profit / Sales × 100`

This was used to explore profitability patterns across transactions and business dimensions.

The analysis also derives grouped metrics such as:

- Total Sales
- Total Profit
- Sales by Category
- Sales by Market
- Sales by Country
- Sales by Product
- Sales by Sub-Category
- Profit by Category and Year
- Shipping Cost by Market
- Regional Sales
- Regional Profit
- Average transaction-level Profit Margin

---

# 📈 Exploratory Analysis

## 🌍 Country Sales Performance

The analysis identifies the **United States** as the highest-sales country, followed by:

1. United States — **$2.30M**
2. Australia — **$925.26K**
3. France — **$858.93K**
4. China — **$700.59K**
5. Germany — **$628.86K**

The United States is therefore the largest individual country market by sales in the dataset.

---

## 📦 Category Sales Performance

Total sales by category:

| Category | Sales |
|---|---:|
| Technology | **$4.74M** |
| Furniture | **$4.11M** |
| Office Supplies | **$3.79M** |

### Business Insight

**Technology is the largest revenue-generating category**, followed by Furniture and Office Supplies.

This makes Technology an important category for understanding the drivers of overall revenue performance.

---

## 🗂️ Sub-Category Sales Performance

The highest-selling sub-categories include:

| Sub-Category | Sales |
|---|---:|
| Phones | **$1.71M** |
| Copiers | **$1.51M** |
| Chairs | **$1.50M** |
| Bookcases | **$1.47M** |
| Storage | **$1.13M** |
| Appliances | **$1.01M** |

### Business Insight

Phones are the strongest individual sub-category by sales, followed by Copiers and Chairs.

This suggests that a relatively small group of sub-categories contributes a substantial share of overall revenue.

---

# 🛍️ Top Products by Sales

The top-selling products include:

| Product | Sales |
|---|---:|
| Apple Smart Phone, Full Size | **$86.94K** |
| Cisco Smart Phone, Full Size | **$76.44K** |
| Motorola Smart Phone, Full Size | **$73.16K** |
| Nokia Smart Phone, Full Size | **$71.90K** |
| Canon imageCLASS 2200 Advanced Copier | **$61.60K** |

### Business Insight

Smartphone products dominate the highest-selling product list, indicating strong revenue concentration among technology products.

---

# 🌐 Market Performance

Sales by market:

| Market | Sales |
|---|---:|
| APAC | **$3.59M** |
| EU | **$2.94M** |
| US | **$2.30M** |
| LATAM | **$2.16M** |
| EMEA | **$806.18K** |
| Africa | **$783.78K** |
| Canada | **$66.93K** |

### Business Insight

**APAC is the largest market by sales**, followed by EU and US.

This makes APAC a key market for further analysis of product mix, profitability, shipping costs, and customer behavior.

---

# 🚚 Shipping Mode Analysis

Order distribution by shipping mode:

| Ship Mode | Orders |
|---|---:|
| Standard Class | **30,775** |
| Second Class | **10,309** |
| First Class | **7,505** |
| Same Day | **2,701** |

### Business Insight

Standard Class accounts for the majority of orders, while Same Day represents a comparatively small portion of overall order volume.

This provides useful context for understanding the company's shipping and fulfillment mix.

---

# 📈 Profit Trend by Category

The analysis examines yearly profit performance across:

- Furniture
- Office Supplies
- Technology

From 2011 to 2014, profit increased across all three categories in the dataset.

Technology consistently generated the highest annual profit among the three categories, while Office Supplies also showed substantial profit growth.

### Business Insight

Technology represents an important contributor to both **sales and profit**, making it a key category for continued performance monitoring.

---

# 📉 Discount Analysis

The project examines the distribution of discounts across transactions.

The purpose is to understand how frequently different discount levels are applied and provide a basis for investigating whether discounting may be associated with profitability differences.

### Next Analytical Opportunity

A deeper analysis could compare:

**Discount % → Sales → Profit → Profit Margin**

at product, category, and market level to determine whether higher discounts are associated with weaker profitability.

---

# 🚢 Shipping Cost Analysis

Total shipping costs by market were analyzed.

| Market | Shipping Cost |
|---|---:|
| APAC | **$387.17K** |
| EU | **$309.42K** |
| US | **$238.17K** |
| LATAM | **$234.13K** |
| EMEA | **$88.38K** |
| Africa | **$88.14K** |
| Canada | **$7.41K** |

### Business Insight

APAC has the highest total shipping cost, followed by EU and US.

Because APAC is also the highest-sales market, further analysis should examine **shipping cost relative to sales** rather than using total shipping cost alone.

---

# 📉 Loss-Making Products

The analysis identifies products with negative total profit after aggregating profit by product.

Examples of products appearing in the negative-profit analysis include:

- Stiletto Ruler, Serrated
- Acco PRESSTEX Data Binder with Storage Hooks
- Rubber Band Ball
- Brites Rubber Bands
- Eldon Gobal File Keepers
- Hon Color Coded Labels
- Avery Framed View Binder
- Round Ring Binders

### Business Insight

Not every high-volume or frequently sold product necessarily contributes positively to profitability.

Loss-making SKUs should therefore be evaluated using:

- Selling price
- Discount
- Product cost
- Shipping cost
- Sales volume
- Total contribution

before decisions are made about pricing or product assortment.

> **Note:** Two products in the raw calculation produce values extremely close to zero because of floating-point precision. They should not be treated as materially loss-making without applying an appropriate numerical threshold.

---

# 📊 Sales vs Profit Analysis

A scatter analysis was used to examine the relationship between transaction-level Sales and Profit.

This helps identify:

- High-sales / high-profit transactions
- High-sales / low-profit transactions
- Low-sales / negative-profit transactions
- Category-level patterns

The analysis demonstrates that **higher sales do not automatically guarantee proportionally higher profit**.

This is important because revenue should be evaluated together with profitability rather than treated as the sole measure of performance.

---

# 🔗 Correlation Analysis

Correlation analysis was performed across:

- Sales
- Profit
- Quantity
- Shipping Cost

Key correlations include:

| Variable Pair | Correlation |
|---|---:|
| Sales ↔ Profit | **0.485** |
| Sales ↔ Quantity | **0.314** |
| Sales ↔ Shipping Cost | **0.768** |
| Profit ↔ Quantity | **0.104** |
| Profit ↔ Shipping Cost | **0.354** |
| Quantity ↔ Shipping Cost | **0.273** |

### Key Insight

Sales and Shipping Cost show a relatively strong positive correlation of approximately **0.77**.

This is expected to some extent because larger sales transactions can involve larger shipment values or quantities, but the relationship warrants further investigation at product and market level.

The Sales–Profit correlation of approximately **0.48** indicates a moderate positive relationship, but it also demonstrates that higher sales do not perfectly translate into higher profit.

> **Important:** Correlation indicates association, not causation.

---

# 💰 Profitability Analysis

The project calculates transaction-level Profit Margin using:

**Profit Margin = Profit / Sales × 100**

The analysis then attempts to compare average transaction-level margins across categories and markets.

However, some records contain zero sales, resulting in infinite values during the raw calculation. Therefore, the category and market average-margin outputs from the notebook should **not be treated as final business findings without additional data validation and handling of zero-sales records**.

### Recommended Improvement

A more reliable profitability measure would be calculated at the aggregated level:

**Profit Margin % = Total Profit / Total Sales × 100**

This prevents individual zero-sales records from distorting the analysis.

---

# 🌍 Regional Sales & Profit

The analysis compares total Sales and Profit across regions.

### Highest Sales Regions

| Region | Sales |
|---|---:|
| Central | **$2.82M** |
| South | **$1.60M** |
| North | **$1.25M** |
| Oceania | **$1.10M** |
| Southeast Asia | **$884.44K** |

### Highest Profit Regions

| Region | Profit |
|---|---:|
| Central | **$311.40K** |
| North | **$194.60K** |
| Southeast Asia | **$178.52K** |
| North Asia | **$165.58K** |
| Central Asia | **$132.48K** |

### Business Insight

Central is the strongest region in both total sales and total profit.

However, high sales should still be evaluated alongside profitability and cost-to-serve before concluding that a region is operationally optimal.

---

# 🔎 Key Business Insights

### 1. Technology is the largest sales category.

Technology generated approximately **$4.74M** in sales, making it the largest of the three major categories.

**Business implication:** Technology should remain a key focus area for product and revenue analysis.

---

### 2. APAC is the largest market by sales.

APAC generated approximately **$3.59M** in sales.

**Business implication:** Because APAC represents the largest sales market, even relatively small changes in product mix, profitability, or shipping efficiency could be commercially important.

---

### 3. Phones are the strongest sub-category by sales.

Phones generated approximately **$1.71M**, ahead of Copiers and Chairs.

**Business implication:** High-performing sub-categories should be evaluated not only for revenue contribution but also for profitability and discount behavior.

---

### 4. Shipping costs are strongly associated with sales.

The correlation between Sales and Shipping Cost is approximately **0.77**.

**Business implication:** Shipping economics deserve deeper investigation, particularly across high-volume markets and products.

---

### 5. Revenue and profit are related, but not perfectly.

Sales and Profit have a correlation of approximately **0.48**.

**Business implication:** Revenue growth alone cannot be used as a complete measure of business performance. Product economics, discounts, shipping costs, and other factors need to be considered.

---

### 6. Loss-making products require product-level investigation.

The analysis identifies multiple products with negative total profit.

**Business implication:** Management should investigate pricing, discounting, product costs, and shipping economics before deciding whether these products should be repriced, optimized, or removed from the portfolio.

---

# 💡 Business Recommendations

| Priority | Observation | Recommended Action | Business Owner |
|---|---|---|---|
| High | Technology is the largest sales category | Analyze Technology profitability at product and sub-category level to identify the strongest profit contributors | Product / Commercial |
| High | APAC generates the highest sales and shipping cost | Analyze shipping cost as a percentage of sales and investigate high-cost product/region combinations | Operations |
| High | Multiple products generate negative total profit | Review pricing, discounts, product costs, and shipping costs for loss-making SKUs | Product / Pricing |
| Medium | Phones are the highest-selling sub-category | Evaluate whether high sales volume is translating into proportional profit | Commercial / Finance |
| Medium | Sales and shipping cost have a strong positive correlation | Investigate shipping economics by product, quantity, market, and ship mode | Operations |
| Medium | Discount levels vary across transactions | Compare discount bands against profit margin to identify potentially unprofitable discount practices | Sales / Pricing |

---

# ⚠️ Analytical Limitations & Data Quality Notes

This project is exploratory and should be treated as a starting point for deeper analysis.

### Profit Margin Calculation

The notebook's transaction-level margin calculation produces infinite values for records where Sales equals zero.

A production analysis should handle these records explicitly before calculating average margins.

### Market Profit Analysis

The notebook section titled **"Profit by Market"** currently groups the `Sales` column rather than the `Profit` column.

Therefore, the market-level output from that specific analysis should be interpreted as **market sales**, not market profit.

### Correlation

Correlation measures association and does not establish causality.

For example, the strong Sales–Shipping Cost relationship does not prove that higher shipping costs cause higher sales.

### Dataset Scope

The analysis is based on the fields available in the dataset. It does not include information such as:

- Marketing spend
- Customer acquisition cost
- Inventory availability
- Competitor pricing
- Product return reasons
- Operational labor cost
- Customer lifetime value

These variables would be required for more advanced profitability and causal analysis.

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

# 🛠️ Tools & Technologies

### Python

- Python
- Jupyter Notebook

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn

### Analytical Techniques

- Exploratory Data Analysis
- Data Cleaning
- Feature Engineering
- Descriptive Statistics
- GroupBy Analysis
- Correlation Analysis
- Profitability Analysis
- Trend Analysis
- Business Data Visualization

---

# ⭐ Project Highlights

- **51,290 transactional records analyzed**
- Sales analysis across global markets and countries
- Category and sub-category performance analysis
- Top-product sales analysis
- Product-level loss analysis
- Regional sales and profit comparison
- Shipping cost analysis
- Discount distribution analysis
- Sales vs Profit relationship analysis
- Correlation analysis
- Profit-margin exploration
- Business-oriented recommendations
- Data quality validation and analytical limitations documented

---

# 👤 Project Role

**Data Analyst — End-to-End Exploratory Analysis**

Responsible for:

- Loading and inspecting the dataset
- Performing data-quality checks
- Analyzing missing values and duplicate records
- Preparing data for analysis
- Performing exploratory data analysis
- Creating business-focused aggregations
- Developing statistical and correlation analysis
- Creating visualizations
- Identifying business patterns
- Translating analytical observations into business recommendations

---
