# 📊 Customer Churn Analysis using Python & SQLite

## 📌 Project Overview

Customer churn is one of the most important business metrics for subscription-based companies. It helps businesses understand **which customers are leaving, why they are leaving, and what factors influence customer retention**.

In this project, I built an end-to-end **Customer Churn Analysis** pipeline using **Python, SQLite, Pandas, NumPy, Matplotlib, and Seaborn**. The project involves loading customer data from multiple database tables, cleaning and transforming the data, creating business metrics, performing exploratory data analysis (EDA), and visualizing customer churn patterns to generate meaningful business insights.

---

## 🎯 Project Objectives

* Analyze customer churn behavior.
* Identify factors that contribute to customer churn.
* Calculate important business KPIs related to customer retention.
* Perform data cleaning and feature engineering.
* Create visualizations to understand customer behavior.
* Generate actionable insights that can help businesses improve customer retention.

---

## 🛠️ Technologies Used

* Python
* Google Colab
* SQLite
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## 📂 Dataset

The project uses a SQLite database named **`customer_churn.db`** containing three relational tables:

### 1. Customer Table (`db_customer`)

Contains customer demographic information such as:

* Customer ID
* Customer Name
* Gender
* Date of Birth
* State
* Country

### 2. Subscription Table (`db_subscription`)

Contains subscription-related information including:

* Subscription Start Date
* Renewal Date
* Cancellation Date
* Plan Type
* Contract Type
* Monthly Charges
* Customer Lifetime Value (CLTV)
* Churn Score

### 3. Support Table (`db_support`)

Contains customer support information such as:

* Complaint Date
* Escalation Status
* CSAT Score

---

# Data Cleaning

The following preprocessing steps were performed before analysis:

* Loaded all database tables into Pandas DataFrames.
* Renamed columns for better readability.
* Removed unnecessary columns with excessive missing values.
* Converted date columns into datetime format.
* Standardized inconsistent gender values.
* Filled missing country values using state information.
* Removed duplicate support records by keeping the latest complaint.
* Calculated complaint count for every customer.
* Created a churn flag based on cancellation status.

---

# Data Integration

After cleaning, all three tables were merged using **Customer ID** to create a single dataset for analysis.

---

# Feature Engineering

Several new features were created to improve the analysis:

* Customer Age
* Customer Tenure (Days)
* Churn Flag
* Complaint Count
* Churn Risk Category (Low, Medium, High)

---

# Business KPIs Calculated

The project calculates multiple business metrics including:

* Customer Churn Rate
* Customer Retention Rate
* Average Revenue Per User (ARPU)
* Revenue at Risk
* Average Customer Tenure
* Escalation Rate
* Average Complaints per Customer
* Correlation between Escalations and Churn

---

# Exploratory Data Analysis (EDA)

Performed data analysis using:

* GroupBy Operations
* Aggregations
* Pivot Tables
* Correlation Analysis

---

# Data Visualizations

The following visualizations were created:

* Monthly Customer Churn Trend
* Churn Rate by Subscription Plan
* Churn Rate by State
* Correlation Heatmap
* Pair Plot
* Monthly Charges Distribution
* Customer Segmentation based on Churn Risk

These visualizations help identify customer behavior, high-risk customer groups, and business trends.

---

# SQLite Operations

Apart from analysis, this project also demonstrates SQL database operations such as:

* Connecting Python with SQLite
* Reading SQL tables into Pandas
* Creating sample tables
* Inserting records
* Removing duplicate records
* Performing SQL aggregation queries

---

# Key Learnings

Through this project, I gained hands-on experience with:

* Working with relational databases using SQLite
* SQL and Python integration
* Data cleaning and preprocessing
* Feature engineering
* Exploratory Data Analysis (EDA)
* Business KPI calculation
* Customer churn analysis
* Data visualization using Matplotlib and Seaborn
* Business insight generation from real-world datasets

---

# Project Workflow

1. Load data from SQLite database
2. Clean and preprocess the data
3. Merge multiple tables
4. Perform feature engineering
5. Calculate business KPIs
6. Conduct exploratory data analysis
7. Create visualizations
8. Generate business insights

---

# Business Value

This project demonstrates how customer data can be transformed into actionable insights. By identifying churn patterns and customer risk levels, businesses can:

* Improve customer retention
* Reduce revenue loss
* Identify high-value customers
* Prioritize customers with high churn risk
* Make data-driven business decisions

---

# Future Improvements

* Build a Machine Learning model to predict customer churn.
* Create an interactive dashboard using Power BI or Tableau.
* Deploy the project as a web application using Streamlit.
* Perform advanced customer segmentation using clustering techniques.
