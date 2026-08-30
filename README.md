# Customer Churn Analysis for MTN Nigeria
A beginner-to-professional data analytics portfolio project covering Excel,
PostgreSQL, and Tableau, built around a real MTN Nigeria customer transaction
dataset (974 transactions, 496 unique customers, 35 states).
## Project Overview
MTN Nigeria's retention team lacked a structured, data-driven view of who
churns, what they were using, why they left, and how much revenue is at
risk. This project quantifies churn (29.16% overall), identifies the
highest-risk states, devices, and plans, and translates the findings into
six concrete retention recommendations.
## Tools Used- **Excel** — data cleaning, pivot tables, calculated columns, charts- **PostgreSQL** — relational modeling (4NF-normalized schema), 42 SQL queries,
views, indexes- **Tableau** — interactive dashboard with KPI cards, filters, actions, and
a story page
## Dataset
`mtn_customer_churn.csv` — 974 rows / 17 columns. See the full data
dictionary in the Project Guide (`Documentation/Project_Guide.pdf`, Section 3).
## Methodology
Ask → Prepare → Process → Analyze → Share → Act. Full lifecycle documented
in `Documentation/Project_Guide.pdf`.
## Results
| KPI | Value |
|---|---|
| Total Revenue Analyzed | ₦199,348,200 |
| Unique Customers | 496 |
| Overall Churn Rate | 29.16% |
| Highest-Churn State | Adamawa (61.1%) |
| Top Stated Churn Reason | High Call Tariffs (54 customers) |
## Dashboard
See `tableau/Dashboard_Screenshots/` for exported images of the live
Tableau dashboard, or open `tableau/Dashboard.twbx` in Tableau Desktop /
Tableau Public.
## Insights
1. Churn is heavily concentrated geographically (Adamawa, Imo, Akwa Ibom).
2. Pricing (tariffs + data cost) is the single largest addressable churn
driver.
3. Satisfaction score and tenure are weak standalone predictors of churn.
4. Revenue exposure from churn is broad, not limited to low-value accounts.
## Recommendations
See `reports/Final_Report.pdf`, Section 7.4, for the six prioritized
business recommendations.
## Folder Structure
See the "Project Structure" section of `Documentation/Project_Guide.pdf`
for the complete annotated folder tree.
## Installation Instructions
1. Clone this repository.
2. Load `data/cleaned/mtn_customer_churn_cleaned.csv` into Excel to explore
`excel/Cleaning.xlsx`, `excel/PivotTables.xlsx`, and `excel/Charts.xlsx`.
3. Create a local PostgreSQL database and run the scripts in `sql/` in this
order: `create_database.sql` → `create_tables.sql` → `import_data.sql` →
`views.sql` → `indexes.sql` → `analysis_queries.sql`.
4. Open [`tableau/Dashboard.twbx`](https://public.tableau.com/app/profile/queen.ameh/viz/MTNNigeriaCustomerChurnAnalysis/MTNCustomerChurnDashboard?publish=yes) in Tableau Desktop or Tableau Public (no live database connection required — the extract is packaged in the file).
5. Read `Documentation/Project_Guide.pdf` for the full step-by-step lab manual.
   Author Ameh Queen Lovina
Data Analytics Essentials — Capstone Portfolio Project.
