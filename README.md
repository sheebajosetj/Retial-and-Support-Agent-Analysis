# 🛒Retial and Support Agent Analysis using SQL

Fliipazon Retail is a multinational company that operates a chain of retail stores across different regions. They sell a wide range of products and want to analyse their sales data to gain insights into their business performance and make informed decisions.
## 📌 Project Objective
To analyze data from a retail company operating across multiple regions to extract meaningful insights and generate actionable reports. The focus areas included:

- 👥 Customer behavior
- 🧑‍💼 Agent performance
- 💰 Sales trends and commission logic

---

## 🧾 Dataset Overview

The dataset represents a fictional retail chain and consists of three main tables:

- **Customers Table**: Details about customers (e.g., `cust_code`, location, outstanding amount).
- **Orders Table**: Includes order-specific information such as order amount and payment.
- **Agents Table**: Agent details including codes and commission structure.

🔗 **Foreign Key Relationships:**

- `cust_code` → joins Customers with Orders
- `agent_code` → joins Agents with Orders

---

## 🧹 Steps Followed

### 1. Data Cleaning

- Identified schema, tables, and respective columns.
- Counted the number of records in each table.
- Handled missing, inconsistent, and non-numeric values.
- Verified data types to ensure integrity.

### 2. Basic SQL Analysis

- Calculated:
  - Total orders
  - Total revenue
  - Average order value
- Identified agents with the highest number of high-grade customers (grade = 3).
- Determined the most active cities by total order value.

---

## 👤 Customer Analysis

- Found total number of customers.
- Identified top-spending customers by order value.
- Calculated repeat customer percentage to evaluate **customer retention**.

---

## 👨‍💼 Agent Performance & Commission Analysis

- Ranked top-performing agents based on:
  - Total orders handled
  - Total order amount
- Segregated agents based on **advance payments collected**.

📐 **Commission Logic (Using SQL CASE WHEN):**

| Order Value       | Commission Rate        |
|------------------|------------------------|
| `< 750`          | No Commission          |
| `750 - 1000`     | 1.5x old commission    |
| `> 1000`         | 2x old commission       |

---

## 🌍 Segment Analysis

- Identified the customer with the **maximum outstanding amount** in every country/region segment.

---

## 🔍 Exploratory Analysis

### 1. Gender-Based Purchase Patterns

- Compared number of male vs. female buyers.
- Checked whether higher income influences bike purchases.

### 2. Distance vs. Purchase Behavior

- Analyzed whether customers living farther commute more and are more likely to purchase.
- 🔧 Faced issues due to entries like `"10+ miles"` — resolved through preprocessing.

---

## 🛠️ Tools & Technologies Used

- SQL (PostgreSQL/MySQL) for data querying
- Excel/Google Sheets for profiling and validation
- *(Optional)* Power BI for dashboard creation and visualization

---

## ✅ Outcome

- 💡 Identified top agents and sales contributors
- 🗺️ Region-wise and customer-wise segmentation
- 💼 Created a logical commission system for agents
- 📊 Built a foundation for business intelligence dashboarding

---

> 📂 *Perfect for adding as a case study project in your Data Analyst/Data Science GitHub portfolio.*
