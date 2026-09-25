::: {align="center"}
# 📊 Customer Shopping Behavior Analysis

### End-to-End Data Analytics Portfolio Project

**Python · Pandas · PostgreSQL · SQL · Power BI · Jupyter**

`<br>`{=html}

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-SQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Power
BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

`<br>`{=html}

> **Turning raw customer shopping data into meaningful business insights
> through data cleaning, SQL analysis, and interactive visualization.**
:::

------------------------------------------------------------------------

## 📌 Project at a Glance

  -----------------------------------------------------------------------
      📊 Dataset         🔢 Records         🧩 Columns     🛠️ Core Tools
  ------------------ ------------------ ------------------ --------------
  Customer Shopping      **3,900**            **18**       Python ·
       Behavior                                            PostgreSQL ·
                                                           SQL · Power BI

  -----------------------------------------------------------------------

### 🎯 Business Objective

A retail company wants to better understand customer shopping behavior
to improve **sales, customer satisfaction, customer engagement, and
long-term loyalty**.

This project investigates how factors such as:

-   👥 Customer demographics
-   🛍️ Product categories and preferences
-   🏷️ Discounts and promotions
-   ⭐ Product reviews
-   🚚 Shipping preferences
-   💳 Payment behavior
-   🔁 Previous purchases
-   🔔 Subscription status

relate to purchasing behavior and customer segments.

------------------------------------------------------------------------

## 🔄 End-to-End Workflow

``` mermaid
flowchart LR
    A["📁 Raw CSV Data"] --> B["🐍 Python / Pandas"]
    B --> C["🧹 Data Cleaning"]
    C --> D["⚙️ Feature Engineering"]
    D --> E["🐘 PostgreSQL"]
    E --> F["🔎 SQL Business Analysis"]
    F --> G["📊 Power BI"]
    G --> H["💡 Insights"]
    H --> I["🎯 Recommendations"]
```

------------------------------------------------------------------------

## 🧰 Tech Stack

  Technology                Purpose
  ------------------------- ----------------------------------------------
  🐍 **Python**             Data preparation and exploratory analysis
  🐼 **Pandas**             Data manipulation and cleaning
  📓 **Jupyter Notebook**   Interactive analysis
  🐘 **PostgreSQL**         Database integration and structured analysis
  🔎 **SQL**                Business-question analysis
  📊 **Power BI**           Interactive dashboard and visualization
  🔗 **SQLAlchemy**         Python-to-database connection
  🐙 **GitHub**             Project version control and portfolio

------------------------------------------------------------------------

## 📂 Dataset

The dataset contains **3,900 purchase records** with **18 columns**.

### Main Data Categories

  Category          Examples
  ----------------- --------------------------------------------
  👤 Customer       Customer ID, Age, Gender, Location
  🛍️ Product        Item Purchased, Category, Size, Color
  💰 Purchase       Purchase Amount, Season
  🔁 Behavior       Previous Purchases, Frequency of Purchases
  ⭐ Reviews        Review Rating
  🔔 Subscription   Subscription Status
  🚚 Shipping       Shipping Type
  🏷️ Promotions     Discount Applied, Promo Code Used
  💳 Payment        Payment Method

### Data Quality

-   **3,900** rows
-   **18** columns
-   **37** missing values in `Review Rating`
-   Missing review ratings were imputed using the **median rating of
    each product category**

------------------------------------------------------------------------

# 🐍 1. Data Preparation with Python

The project starts by loading and exploring the raw dataset using
Pandas.

### 🔍 Exploration

``` python
df.head()
df.info()
df.describe(include="all")
df.isnull().sum()
```

### 🧹 Cleaning

The preparation process includes:

-   Checking the dataset structure
-   Inspecting data types
-   Checking missing values
-   Handling missing review ratings
-   Standardizing column names using `snake_case`
-   Checking data consistency
-   Removing the redundant `promo_code_used` column

### ⚙️ Feature Engineering

Two important features were created:

  -----------------------------------------------------------------------
  Feature                             Purpose
  ----------------------------------- -----------------------------------
  `age_group`                         Groups customers by age

  `purchase_frequency_days`           Converts purchase frequency into
                                      approximate day intervals
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 🗄️ 2. PostgreSQL & SQL Analysis

After cleaning the data in Python, the dataset was loaded into
**PostgreSQL** for business analysis.

### 🔎 Business Questions

The SQL analysis covers **10 business questions**:

  -----------------------------------------------------------------------
                       \#                      Business Question
  -------------------------------------------- --------------------------
                       01                      💰 What is the revenue
                                               generated by gender?

                       02                      🏷️ Which customers use
                                               discounts but still spend
                                               above average?

                       03                      ⭐ Which are the top 5
                                               products by average
                                               rating?

                       04                      🚚 How does Standard
                                               shipping compare with
                                               Express shipping?

                       05                      🔔 How do subscribers
                                               compare with
                                               non-subscribers?

                       06                      🏷️ Which products have the
                                               highest percentage of
                                               discounted purchases?

                       07                      👥 How many customers are
                                               New, Returning, and Loyal?

                       08                      🛍️ What are the top 3
                                               products in each category?

                       09                      🔁 What is the
                                               relationship between
                                               repeat buyers and
                                               subscriptions?

                       10                      👤 Which age groups
                                               contribute the most
                                               revenue?
  -----------------------------------------------------------------------

### 🧠 SQL Concepts Used

``` text
✓ GROUP BY
✓ Aggregate Functions
✓ CASE Statements
✓ Subqueries
✓ CTEs
✓ Window Functions
✓ Ranking
✓ Conditional Analysis
```

------------------------------------------------------------------------

# 📊 3. Power BI Dashboard

The cleaned and analyzed data was used to create an interactive
**Customer Behavior Dashboard**.

### 📌 Dashboard Includes

**KPI Cards**

-   👥 Number of Customers
-   💵 Average Purchase Amount
-   ⭐ Average Review Rating

**Visual Analysis**

-   Subscription status
-   Revenue by category
-   Sales by category
-   Revenue by age group
-   Sales by age group

**Interactive Filters**

-   Subscription Status
-   Gender
-   Category
-   Shipping Type

> 💡 The dashboard is included in `customer_behavior_dashboard.pbix`.

------------------------------------------------------------------------

# 🔎 4. Key Findings

### 💰 Revenue by Gender

  Gender         Revenue
  -------- -------------
  Male       **157,890**
  Female      **75,191**

### 🚚 Shipping Comparison

  Shipping Type     Average Purchase
  --------------- ------------------
  Standard                 **58.46**
  Express                  **60.48**

Express-shipping customers had a higher average purchase amount in the
analyzed dataset.

### ⭐ Top-Rated Products

The SQL analysis identified:

1.  🥇 Gloves
2.  🥈 Sandals
3.  🥉 Boots
4.  Hat
5.  Skirt

### 🏷️ Highest Discount-Dependent Products

  Product      Discount Rate
  ---------- ---------------
  Hat             **50.00%**
  Sneakers        **49.66%**
  Coat            **49.07%**
  Sweater         **48.17%**
  Pants           **47.37%**

### 👥 Customer Segmentation

  Segment          Customers
  -------------- -----------
  🟢 Loyal         **3,116**
  🟡 Returning       **701**
  🔵 New              **83**

### 💵 Revenue by Age Group

  Age Group          Revenue
  ------------- ------------
  Young Adult     **62,143**
  Middle-aged     **59,197**
  Adult           **55,978**
  Senior          **55,763**

------------------------------------------------------------------------

# 💡 5. Business Recommendations

### 🔔 01 --- Boost Subscription Adoption

Promote exclusive benefits and offers for subscription customers.

### 🤝 02 --- Strengthen Customer Loyalty

Reward repeat buyers and encourage movement toward the Loyal customer
segment.

### 🏷️ 03 --- Review Discount Strategy

Balance promotional discounts with customer value and business
profitability.

### ⭐ 04 --- Improve Product Positioning

Highlight highly rated and frequently purchased products in marketing
campaigns.

### 🎯 05 --- Use Targeted Marketing

Use age groups, purchasing behavior, and shipping preferences to design
targeted campaigns.

------------------------------------------------------------------------

# 📁 Project Structure

``` text
customer-shopping-behavior-analysis/
│
├── 📄 Business Problem Document.pdf
├── 📄 Customer Shopping Behavior Analysis.pdf
├── 📊 Customer-Shopping-Behavior-Analysis.pptx
│
├── 🐍 Customer_Shopping_Behavior_Analysis.ipynb
├── 🗄️ customer_behavior_sql_queries.sql
├── 📊 customer_behavior_dashboard.pbix
├── 📁 customer_shopping_behavior.csv
│
└── 📘 README.md
```

------------------------------------------------------------------------

# 🚀 How to Run

### 1️⃣ Clone the Repository

``` bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd customer-shopping-behavior-analysis
```

### 2️⃣ Install Python Libraries

``` bash
pip install pandas sqlalchemy psycopg2-binary
```

### 3️⃣ Open the Notebook

Open:

``` text
Customer_Shopping_Behavior_Analysis.ipynb
```

Run the notebook to perform:

``` text
Data Loading
    ↓
Data Exploration
    ↓
Data Cleaning
    ↓
Feature Engineering
    ↓
PostgreSQL Integration
```

### 4️⃣ Configure PostgreSQL

Create a PostgreSQL database and configure the database connection in
the notebook.

Example:

``` python
from sqlalchemy import create_engine

engine = create_engine(
    "postgresql+psycopg2://username:password@localhost:5432/customer_behavior"
)
```

⚠️ **Never commit database passwords or credentials to GitHub.**

### 5️⃣ Run SQL Analysis

Open:

``` text
customer_behavior_sql_queries.sql
```

Run the queries against the cleaned customer table.

### 6️⃣ Open Power BI

Open:

``` text
customer_behavior_dashboard.pbix
```

Refresh the data connection if required.

------------------------------------------------------------------------

# 📄 Project Files

  ---------------------------------------------------------------------------------
  File                                          Description
  --------------------------------------------- -----------------------------------
  `customer_shopping_behavior.csv`              Customer shopping dataset

  `Customer_Shopping_Behavior_Analysis.ipynb`   Python data preparation and
                                                analysis

  `customer_behavior_sql_queries.sql`           SQL business analysis

  `customer_behavior_dashboard.pbix`            Power BI dashboard

  `Customer Shopping Behavior Analysis.pdf`     Detailed project report

  `Customer-Shopping-Behavior-Analysis.pptx`    Project presentation

  `Business Problem Document.pdf`               Business problem and project
                                                deliverables
  ---------------------------------------------------------------------------------

------------------------------------------------------------------------

# 🎓 Skills Demonstrated

::: {align="center"}
     🐍 Python       🐼 Pandas       🗄️ SQL
  --------------- --------------- ------------
   Data Analysis   Data Cleaning   PostgreSQL

   📊 Power BI    📈 Visualization    💡 Business Insights
  -------------- ------------------- ----------------------
   Dashboarding   Data Storytelling     Recommendations
:::

------------------------------------------------------------------------

# 📚 What This Project Demonstrates

This project demonstrates the ability to take a business problem and
move through the complete analytics lifecycle:

**Raw Data → Cleaning → Transformation → Database → SQL → Visualization
→ Insights → Business Recommendations**

It combines technical data-analysis skills with business-focused
interpretation.

------------------------------------------------------------------------

::: {align="center"}
## 👨‍💻 Author

### **Meghan Gowda B Y**

**Data Analytics \| Python \| SQL \| Power BI**

`<br>`{=html}

⭐ **Customer Shopping Behavior Analysis**

*Turning customer data into actionable business insights.*
:::
