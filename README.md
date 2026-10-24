# 🏦 Financial Loan Analysis — Power BI & SQL

## 📌 Executive Summary
This project delivers an end-to-end financial loan analysis report designed to evaluate loan portfolio performance, track risk categories, and uncover key lending trends. Using **SQL** for data preparation and **Power BI** for visual storytelling, this dashboard empowers financial decision-makers with real-time insights into good vs. bad loans.

---

## 🛠️ Tools & Technologies Used
* **Data Extraction & Transformation:** SQL Server / MS SQL (SQL Queries)
* **Data Visualization & Dashboarding:** Power BI Desktop (DAX, Power Query)
* **Documentation:** MS Word / Excel

---

## 📊 Dashboard Showcase

### Page 1: Executive Summary
> *High-level KPIs including total loan applications, funded amounts, total received amounts, interest rates, and Good vs. Bad loan breakdown.*
![Executive Summary](Screenshot%202026-10-24%20200743.png)

---

### Page 2: Borrower Demographics & Regional Trends (Overview)
> *Geographic distribution of loans across US states, monthly loan application trends, homeownership status, and employment length breakdown.*
![Overview Trends](Screenshot%202026-10-24%20201614.png)

---

### Page 3: Loan Details Grid
> *A granular table view providing borrower-level details, loan grades, loan terms, and specific repayment statuses.*
![Loan Details](Screenshot%202026-10-24%20200937.png)

## 🔍 SQL Queries & Documentation
The full database queries and validation results are documented in the uploaded `SQL_Queries & Results - Financial Loan_Analysis.docx` file in this repository.

<details>
<summary><b>Click to expand sample SQL query (KPI Extraction)</b></summary>

```sql
-- Total Funded Amount vs Total Received Amount
SELECT 
    SUM(loan_amount) AS Total_Funded_Amount,
    SUM(total_payment) AS Total_Amount_Received,
    AVG(int_rate) * 100 AS Avg_Interest_Rate,
    AVG(dti) * 100 AS Avg_DTI
FROM financial_loan_data;

## 🚀 How to View This Project
1. **Download the `.pbix` file** (`Financial Loan Dashboard.pbix`) from this repository.
2. Open it in **Power BI Desktop** to interact with the fully functioning data model and dashboards locally.
