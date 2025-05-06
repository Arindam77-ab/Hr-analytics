
 Project Title: HR Analytics Dashboard using Power BI
 
Objective:

The HR Analytics Dashboard provides a comprehensive overview of key human resource metrics to help HR managers and leadership teams make data-driven decisions. It visualizes workforce trends and performance indicators in an intuitive and interactive format, focusing on critical HR domains such as recruitment, employee performance, diversity, retention, and overall workforce planning.
To develop an interactive dashboard to monitor and analyze key HR metrics such as employee attrition, promotion, retrenchment, salary distribution, and demographic patterns. The goal is to aid HR decision-making by identifying trends and areas needing intervention.

Data Sources & Preparation
Data Source: Excel/CSV files (employee records)

Fields included: Gender, Age, Department, Job Role, Marital Status, Education Field, Performance Rating, Salary, Business Travel, etc.

Tools Used: Power BI Desktop

Data Preparation Steps:

Import Data: Load the dataset into Power BI from Excel/CSV.

Data Cleaning:

Removed duplicates and blanks.
Converted data types (e.g., dates, numbers).
Standardized column names.
Data Transformation (Power Query):
Created custom columns like Age Category, Attrition Flag, Promotion Eligibility.
Calculated KPIs: Attrition Rate, Monthly Income, Performance Score.
Used DAX for measures (e.g., Total Employees, Attrition %, Avg Salary).

Data Modeling:

Defined relationships between tables.
Created Date Table for time-based analysis (if applicable).
Set up filter tables for slicers.

 Dashboard Pages & Visuals
 
1️) Executive Summary
Total Employees: 1470
Active Employees: 1233
Attrition Rate: 16.12%
Average Age: 36.92

Visuals:

Pie Chart: Active employees by gender.
Bar Chart: Active employees by department.
Bar Chart: Active employees by education field.
Pie Chart: Performance rating by gender.
Bar + Donut Chart: Performance by department and education field.

2️) Salary Summary
Total Monthly Income: 10M
Avg Monthly Income: 6.5K

Visuals:

Pie Chart: Monthly income by gender.
Bar Chart: Monthly income by marital status.
Donut Chart: Monthly income by department.
Bar Chart: Monthly income by education field and job role.
Pie Chart: Monthly income by business travel.

3️) Attrition Summary
Attrition Rate: 16.12%
Attrition Value: 237 employees

Visuals:

Pie Chart: Attrition by gender.
Donut Chart: Attrition by marital status.
Bar Chart: Attrition by department.
Bar Charts: Attrition by education field and job role.
Pie Chart: Attrition by business travel.

4️) Promotion & Retrenchment Summary
Due for Promotion: 72 employees
Will be Retrenched: 117 employees

Visuals:
Pie Chart: Promotion by gender.
Bar Chart: Promotion by marital status.
Donut Chart: Promotion by department.
Bar Chart: Retrenchment by gender and marital status.
Pie Chart: Retrenchment by department.

 Key KPIs & DAX Measures:
 
Total Employees = COUNT(EmployeeID)
Attrition Rate = DIVIDE(Attrition Count, Total Employees)
Avg Monthly Income = AVERAGE(MonthlyIncome)
Employees Due for Promotion = CALCULATE(COUNT(EmployeeID), [PromotionEligible] = TRUE)
Retrenchment Count = CALCULATE(COUNT(EmployeeID), [WillBeRetrenched] = TRUE)

Insights & Recommendations:
Gender Gap: Males dominate promotions and income, suggesting potential bias.
High Attrition in departments like Sales and roles like Lab Technicians—consider retention strategies.
Married Employees show higher promotion and retrenchment rates—review policies or job satisfaction factors.

Business Travel correlates with higher income and lower attrition—possibly linked to job role seniority or perks.

Departmental Trends: R&D dominates headcount and promotions, while HR has the lowest in all metrics.


