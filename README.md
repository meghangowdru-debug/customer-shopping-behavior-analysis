<div align="center">

# 📊 Customer Shopping Behavior Analysis

### End-to-End Data Analytics Portfolio Project

**Python · Pandas · MySQL · SQL · Power BI · Jupyter**

<p>
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/MySQL-SQL-4169E1?logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white" alt="Jupyter">
</p>

<p>
Turning raw customer shopping data into meaningful business insights through
<strong>data cleaning, SQL analysis, customer behavior analysis, and interactive visualization.</strong>
</p>

</div>

---

## 📌 Project at a Glance

| Area | Details |
|---|---|
| **Project Type** | End-to-End Data Analytics |
| **Dataset** | Customer Shopping Behavior |
| **Records** | 3,900 purchases |
| **Columns** | 18 |
| **Python** | Pandas, NumPy |
| **Database** | MySQL |
| **Visualization** | Power BI |
| **SQL Analysis** | Revenue, customers, products, subscriptions, discounts |
| **Deliverables** | Python notebook, SQL queries, Power BI dashboard, report and presentation |

---

## 🎯 Business Problem

A retail company wants to understand customer shopping behavior to improve:

- 📈 Sales performance
- 🤝 Customer engagement
- 💳 Subscription adoption
- 🎁 Discount and promotional strategies
- ⭐ Product performance
- 🔁 Customer loyalty and repeat purchases

### Main Business Question

> **How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?**

---

## 🔄 Project Workflow

```text
Raw Customer Data
       │
       ▼
Data Cleaning & Preparation
       │
       ▼
Exploratory Data Analysis
       │
       ▼
Feature Engineering
       │
       ▼
MySQL Database
       │
       ▼
SQL Business Analysis
       │
       ▼
Power BI Dashboard
       │
       ▼
Business Insights & Recommendations
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| 🐍 **Python** | Data cleaning and analysis |
| 🐼 **Pandas** | Data manipulation |
| 🔢 **NumPy** | Numerical operations |
| 🐬 **MySQL** | Data storage and querying |
| 🧮 **SQL** | Business analysis |
| 📊 **Power BI** | Interactive dashboard |
| 📓 **Jupyter Notebook** | Python analysis workflow |
| 📁 **CSV** | Source dataset |

---

## 📂 Dataset

The dataset contains **3,900 customer purchases** across **18 columns**.

Important attributes include:

- Customer demographics
- Age and gender
- Location
- Subscription status
- Product and category
- Purchase amount
- Season
- Size and color
- Discount information
- Previous purchases
- Purchase frequency
- Review rating
- Shipping type

The dataset contains **37 missing values in the Review Rating field**.

---

## 🐍 1. Python Data Analysis

The Python notebook performs the main data preparation and exploratory analysis.

### Key steps

- Imported the customer shopping dataset using Pandas
- Inspected data types and descriptive statistics
- Identified missing values
- Imputed missing `Review Rating` values using the median by product category
- Standardized column names using snake_case
- Created an `age_group` feature
- Created a `purchase_frequency_days` feature
- Checked redundancy between discount and promotional-code fields
- Prepared the cleaned data for MySQL analysis

### Notebook

📓 `Customer_Shopping_Behavior_Analysis.ipynb`

---

## 🐬 2. MySQL & SQL Analysis

The cleaned data was loaded into MySQL for structured business analysis.

### Business Questions Answered

1. Revenue by gender
2. High-spending customers using discounts
3. Top products based on ratings
4. Shipping type comparison
5. Subscribers vs. non-subscribers
6. Products strongly associated with discounts
7. Customer segmentation
8. Top products within each category
9. Repeat buyers and subscription behavior
10. Revenue by age group

### SQL File

📄 `customer_behavior_sql_queries.sql`

---

## 📊 3. Power BI Dashboard

The Power BI dashboard converts the analysis into interactive business visuals.

### Dashboard Focus

- Customer purchase behavior
- Revenue trends
- Product performance
- Customer demographics
- Subscription behavior
- Discount usage
- Category-level insights
- Purchase patterns

📊 **Power BI File:** `customer_behavior_dashboard.pbix`

---

## 💡 Key Business Insights

The analysis highlights several areas that can support business decision-making:

- Subscription customers can be analyzed separately to understand loyalty and purchasing behavior.
- Discount usage can be evaluated to identify products and customer groups that depend heavily on promotions.
- Customer segmentation helps identify different purchasing patterns.
- Product-level analysis helps identify strong-performing products within categories.
- Age-group analysis provides another dimension for targeted marketing.
- Shipping and purchase behavior can be compared to understand customer preferences.

---

## 🚀 Business Recommendations

Based on the analysis, the project focuses on:

### 1. Increase Subscription Adoption
Use targeted offers and loyalty benefits to encourage customers to join subscription programs.

### 2. Strengthen Customer Loyalty
Develop loyalty strategies based on repeat purchases and customer segments.

### 3. Review Discount Strategy
Identify products and customer groups where discounts are frequently used and evaluate their impact on revenue.

### 4. Improve Product Positioning
Use product and category-level performance to support inventory and marketing decisions.

### 5. Enable Targeted Marketing
Use demographic and behavioral segments to create more relevant customer campaigns.

---

## 📁 Project Structure

```text
customer-shopping-behavior-analysis/
│
├── 📄 Business Problem Document.pdf
├── 📄 Customer Shopping Behavior Analysis.pdf
├── 📊 Customer-Shopping-Behavior-Analysis.pptx
├── 📊 customer_behavior_dashboard.pbix
├── 🧮 customer_behavior_sql_queries.sql
├── 📓 Customer_Shopping_Behavior_Analysis.ipynb
├── 📁 customer_shopping_behavior.csv
└── 📖 README.md
```

---

## ▶️ How to Use This Project

### 1. Clone the repository

```bash
git clone https://github.com/meghangowdru-debug/customer-shopping-behavior-analysis.git
cd customer-shopping-behavior-analysis
```

### 2. Python Analysis

Open:

```text
Customer_Shopping_Behavior_Analysis.ipynb
```

Run the notebook in Jupyter Notebook, JupyterLab, Google Colab, or VS Code.

### 3. SQL Analysis

Open:

```text
customer_behavior_sql_queries.sql
```

Run the queries in MySQL after loading the cleaned dataset.

### 4. Power BI

Open:

```text
customer_behavior_dashboard.pbix
```

in Power BI Desktop to explore the dashboard.

---

## 📚 Project Deliverables

| Deliverable | File |
|---|---|
| Business Problem | `Business Problem Document.pdf` |
| Data Analysis Report | `Customer Shopping Behavior Analysis.pdf` |
| Python Analysis | `Customer_Shopping_Behavior_Analysis.ipynb` |
| SQL Analysis | `customer_behavior_sql_queries.sql` |
| Power BI Dashboard | `customer_behavior_dashboard.pbix` |
| Presentation | `Customer-Shopping-Behavior-Analysis.pptx` |
| Dataset | `customer_shopping_behavior.csv` |

---

## 🧠 Skills Demonstrated

**Data Analytics**
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Customer Behavior Analysis

**SQL**
- Aggregations
- Filtering
- Joins
- Subqueries
- Window Functions
- Business KPI Analysis

**Visualization**
- Power BI
- Interactive Dashboards
- Business Reporting

**Tools**
- Python
- MySQL
- Jupyter
- Git & GitHub

---

<div align="center">

### 📊 From Data → Analysis → Insights → Business Decisions

**Customer Shopping Behavior Analysis**

</div>
