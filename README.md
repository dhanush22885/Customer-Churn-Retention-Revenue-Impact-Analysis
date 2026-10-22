# 📊 Customer Churn, Retention & Revenue Impact Analysis
End-to-end Data Analytics project for identifying customer churn drivers, quantifying revenue at risk, and generating data-driven retention strategies.

## 🚀 Project Overview

ChurnLens is an end-to-end customer churn analytics project built to transform raw customer, subscription, and support data into actionable business insights.

The project analyzes an OTT subscription business to answer three critical business questions:

* **Who** is most likely to churn?
* **Why** are customers leaving?
* **When** does churn become a significant business risk?

The analysis integrates data from multiple relational tables, performs data cleaning and feature engineering, calculates business KPIs, identifies high-risk customer segments, and translates analytical findings into actionable retention recommendations.

---

## 🎯 Business Problem

Customer churn directly impacts recurring revenue and customer lifetime value.

The objective of this project is to:

* Measure the overall customer churn rate
* Identify customer segments with high churn
* Compare churn across subscription and contract types
* Analyze customer tenure and behavior
* Identify geographical churn patterns
* Understand the relationship between support escalations and churn
* Quantify revenue and CLTV at risk
* Recommend targeted customer-retention strategies

---

## 🛠️ Tech Stack

| Category              | Technologies                        |
| --------------------- | ----------------------------------- |
| Programming           | Python                              |
| Database              | SQLite / SQL                        |
| Data Manipulation     | Pandas, NumPy                       |
| Data Visualization    | Matplotlib, Seaborn                 |
| Database Connectivity | SQLite3                             |
| Analytics             | EDA, KPI Analysis, Segmentation     |
| Reporting             | Business Insights & Recommendations |

The project follows a SQL → Python → Analysis → Visualization → Business Insight workflow.

---

## 🗂️ Data Architecture

The analysis works with three relational datasets:

### `db_customer`

Contains customer-level information such as:

* Customer ID
* Name
* Country
* State
* Gender
* Date of Birth
* Interests
* Pincode

### `db_subscription`

Contains subscription and revenue information:

* Customer ID
* Subscription start date
* Subscription type
* Renewal date
* Plan type
* Contract type
* Cancellation date
* Cancellation reason
* Monthly charges
* CLTV
* Churn score

### `db_support`

Contains customer-support information:

* Customer ID
* Complaint date
* Escalations
* CSAT score
* Comments

These tables form the foundation for customer, subscription, revenue, and support-level analysis.

---

## 🔄 Analytics Workflow

```text
Raw Customer Data
       ↓
SQL Database
       ↓
SQL Queries
       ↓
Python + Pandas
       ↓
Data Cleaning
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
KPI Calculation
       ↓
Customer Segmentation
       ↓
Data Visualization
       ↓
Business Insights
       ↓
Retention Recommendations
```

---

## 📈 Key KPIs

The project calculates business-focused metrics including:

* **Churn Rate**
* **Retention Rate**
* **Churn by Plan Type**
* **Churn by Geography**
* **Average Customer Tenure**
* **ARPU**
* **Revenue at Risk**
* **Escalation Rate**
* **Average Complaints per Customer**
* **Support Escalation vs. Churn**

These KPIs were derived from customer, subscription, and support data to evaluate both customer behavior and business impact.

---

## 🔍 Key Findings

### 📌 Customer Churn

* **Overall Churn Rate:** 28.6%
* **Retention Rate:** 71.4%
* **Average Customer Tenure:** 1,451 days

### 💰 Revenue Impact

* **Total Revenue:** 395
* **Revenue Lost to Churn:** 74
* **Revenue Loss:** 18%
* **CLTV Lost:** 2,047

### 📅 Contract Analysis

A major churn difference was observed between contract types:

| Contract Type | Churn Rate |
| ------------- | ---------: |
| Monthly       |  **55.6%** |
| Annual        |   **8.3%** |

Monthly subscribers showed approximately **6.7× higher churn** than annual subscribers.

---

## 🧠 Customer Risk Analysis

Customers were evaluated using multiple behavioral and subscription signals, including:

* Subscription tenure
* Plan type
* Contract type
* Churn score
* Monthly charges
* Customer lifetime value
* Support escalations
* Complaints

This enabled the identification of **High, Medium, and lower-risk customer segments** and helped prioritize customers for retention campaigns.

---

## 💡 Business Insights

The analysis identified several areas requiring business attention:

### 1. Monthly Subscribers Are High Risk

Monthly-contract customers showed substantially higher churn than annual subscribers.

**Recommendation:**
Create targeted incentives to migrate high-value monthly customers toward annual contracts.

### 2. Karnataka Requires Investigation

Karnataka showed the highest concentration of churn in the analyzed dataset.

**Recommendation:**
Investigate regional pricing changes, customer complaints, technical issues, and competitor activity.

### 3. Basic Plan Has High Churn Volume

A significant amount of churn came from Basic-plan customers.

**Recommendation:**
Analyze whether pricing, product limitations, or customer expectations are contributing to cancellations.

### 4. Support Experience May Influence Churn

Support escalations were analyzed alongside subscription and churn information to identify potential relationships between customer-service interactions and cancellations.

**Recommendation:**
Prioritize customers with repeated complaints or escalations for proactive retention outreach.

### 5. High-Risk Customers Should Be Prioritized

Customers with high churn scores should be evaluated alongside their LTV before launching retention campaigns.

**Recommendation:**

```text
High Churn Risk
      +
High Customer LTV
      ↓
Priority Retention Segment
```

The project recommends targeted outreach through email, SMS, calls, and issue resolution for valuable high-risk customers.

---

## 📊 Analytical Techniques Used

### Data Extraction

* SQL queries
* Relational table joins
* Python-SQL integration
* Pandas `read_sql`

### Data Cleaning

* Missing-value handling
* Data-type correction
* Column selection and renaming
* Data-quality checks

### Feature Engineering

* Customer tenure
* Churn indicators
* Revenue-related metrics
* Customer risk segmentation
* Calculated business metrics

### Exploratory Data Analysis

* GroupBy analysis
* Aggregations
* Pivot tables
* Segment comparisons
* Correlation analysis

### Visualization

* Matplotlib
* Seaborn
* Business KPI visualization
* Customer segment analysis

The overall workflow follows the project's documented SQL extraction, cleaning, feature-engineering, EDA, visualization, and insight-generation process.

---

## 📌 Business Impact

This project demonstrates how a Data Analyst can move beyond simply creating charts and instead connect analytical findings to business decisions.

The analysis quantified:

* **28.6% overall churn**
* **55.6% monthly-contract churn**
* **8.3% annual-contract churn**
* **Revenue leakage of approximately 74**
* **CLTV loss of 2,047**


## 🎯 Skills Demonstrated

**Data Analytics**

* Exploratory Data Analysis
* KPI Development
* Customer Segmentation
* Churn Analysis
* Revenue Analysis
* Business Intelligence
* Insight Generation

**Technical**

* Python
* SQL
* Pandas
* NumPy
* SQLite
* Matplotlib
* Seaborn

**Business**

* Customer Retention
* Revenue-at-Risk Analysis
* Customer Lifetime Value
* Risk Prioritization
* Data-Driven Decision Making
* Business Recommendations

---

## 👨‍💻 Author

**Dhanush R**

Data Science Graduate | Data Analyst | Python & SQL

Interested in transforming data into **actionable business insights and measurable decisions**.

---

⭐ If you found this project useful, consider giving the repository a star.
