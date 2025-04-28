# Alt-Mobility-Data-Analyst-Internship-Assignment
"Analyzed customer orders and payments to uncover sales trends, customer behavior, and payment success rates. Built SQL-driven insights and visualized customer retention using cohort analysis to recommend data-backed strategies for Alt Mobility."


PROBLEM SPACE:
You are provided with two datasets:

payments.csv → Payment data

customer_orders.csv → Order data

You need to use SQL to perform these tasks:

1. Order and Sales Analysis
Analyze order status (e.g., completed, pending, canceled) and sales trends.

Identify key metrics like:

Fulfillment rates.

Revenue trends over time.

2. Customer Analysis
Explore customer behaviors such as:

Repeat ordering.

Segmentation (possibly by geography, vehicle type, or usage).

Trends over a timeline (monthly, quarterly).

3. Payment Status Analysis
Investigate payment success/failure rates.

Identify issues or patterns (e.g., failures on certain days or for certain payment methods).

4. Order Details Report
Create a detailed report linking:

Order info + Payment details.

Key operational metrics.

VISUALIZATION TASK:
5. Customer Retention Analysis
Visualize how many customers from each cohort (e.g., customers who signed up in January) made repeat purchases in later months.

Use a BI visualization tool (such as Power BI, Tableau, Looker Studio, etc.).

Explain clearly how the visualization shows customer retention trends (e.g., retention matrix, cohort analysis graph).



FEATURES of the Assignment:

Feature	Details
Skill Test Areas	SQL, Data Analysis, BI Visualization
Focus Topics	Order Analysis, Customer Behavior, Payment Status, Retention
Deliverables	SQL Code (GitHub), Visualizations (Images), Summary Report
Tools Mentioned	Any SQL environment, any BI tool (e.g., Tableau, Power BI)
Evaluation Factors	Accuracy, Data Cleaning, Visualization, Code, Documentation

📂 Assumed Datasets Structure
customer_orders.csv

order_id	customer_id	order_date	status	amount
101	C001	2024-01-15	completed	25000
102	C002	2024-02-20	cancelled	15000
103	C001	2024-03-10	completed	20000
payments.csv

payment_id	order_id	payment_date	payment_status	payment_amount
5001	101	2024-01-16	success	25000
5002	102	2024-02-21	failed	0
5003	103	2024-03-11	success	20000
