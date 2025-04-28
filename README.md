Alt Mobility - Data Analyst Assignment

🚗 About Alt Mobility

Alt Mobility is a full-stack electric vehicle (EV) leasing and asset management company, managing a fleet of 20,000 EVs. Backed by investors like Shell Ventures and Eurazeo, Alt Mobility focuses on providing accessible financing solutions to accelerate EV adoption across India.

---

 📋 Assignment Overview

This assignment aims to demonstrate data analysis skills by analyzing EV leasing data. The objective was to extract actionable insights related to order fulfillment, customer behavior, payment patterns, and customer retention.

The tasks included SQL-based analysis, data visualization, and business recommendations to enhance Alt Mobility’s operational strategies.

---

  📚 Datasets Provided

Two datasets were shared for analysis:

- customer_orders.csv
  - `order_id`: Unique identifier for each order
  - `customer_id`: Unique identifier for each customer
  - `order_date`: Date when the order was placed
  - `order_amount`: Amount of the order
  - `shipping_address`: Customer’s shipping address
  - `order_status`: Current status of the order (pending, shipped, delivered)

- payments.csv
  - `payment_id`: Unique identifier for each payment
  - `order_id`: Linked order ID for payment
  - `payment_date`: Date when payment was made
  - `payment_amount`: Amount paid
  - `payment_method`: Payment method used (e.g., PayPal, Credit Card)
  - `payment_status`: Status of payment (completed, failed)

---

   🎯 Tasks and Solutions

 1. Order and Sales Analysis

- Objective: Analyze order statuses and overall sales trends.
- Solution:
  - Grouped orders by `order_status` to understand fulfillment patterns.
  - Calculated total sales revenue.
  - Analyzed month-over-month sales trends.

 2. Customer Analysis

- Objective: Understand customer behavior including repeat purchase rates and segmentation.
- Solution:
  - Identified repeat customers.
  - Compared new vs returning customers monthly.
  - Segmented customers based on order activity.

 3. Payment Status Analysis

- Objective: Investigate payment success/failure rates.
- Solution:
  - Calculated counts and percentages of successful and failed payments.
  - Highlighted areas for improving payment success.

 4. Order Details Report

- Objective: Build a comprehensive report combining orders and payments.
- Solution:
  - Created a SQL join between `customer_orders` and `payments`.
  - Consolidated key metrics like order amount, payment status, and payment method into a single view.

 5. Customer Retention Visualization

- Objective: Visualize customer retention rates across months.
- Solution:
  - Performed cohort analysis based on the customer's first order month.
  - Generated a retention matrix showing repeat purchase patterns over subsequent months.
  - Created a heatmap visualization to clearly display customer retention behavior.

---

 🛠 Technologies and Tools Used

- Python 3.8
- SQLite3 (In-memory database for running SQL queries)
- Pandas (for data manipulation and processing)
- Matplotlib and Seaborn (for cohort analysis visualization)
- Jupyter Notebook (for interactive coding and visualization)
- VSCode / GitHub (for project management and version control)

---

 📈 SQL Query Highlights

- Analyzed order status distribution using `GROUP BY`.
- Calculated total and monthly sales using date functions.
- Identified repeat customers using window functions (`RANK()`).
- Analyzed payment success/failure patterns.
- Built an enriched dataset joining orders with payment information.

_All SQL queries are included inside Python scripts using SQLite._

---

 📊 Visualization Highlights

- Cohort Heatmap:
  - Displays percentage of customers retained over several months after their first purchase.
  - Helps visualize churn rates and retention problems.
  
  ![Cohort Heatmap](visualization/customer_retention_cohort.png)

---

 📂 Project Structure

order_id | customer_id | order_date | status | amount
101 | C001 | 2024-01-15 | completed | 25000
102 | C002 | 2024-02-20 | cancelled | 15000
103 | C001 | 2024-03-10 | completed | 20000


payment_id | order_id | payment_date | payment_status | payment_amount
5001 | 101 | 2024-01-16 | success | 25000
5002 | 102 | 2024-02-21 | failed | 0
5003 | 103 | 2024-03-11 | success | 20000
