# Reimbursed Analysis

## Overview
This repository contains a comprehensive analysis of reimbursement data. The following steps were undertaken to refine and derive insights:

1. *Import Data and Power Query*
   - Imported the dataset and utilized Power Query for subsequent operations.

2. *Cleanse Data*
   - Corrected spelling and punctuation errors in the Expense Type column.
   - Standardized and made project names uniform.

3. *Address Missing Values in Currency*
   - Created a new custom column based on amount conditions:
      - If amount >= 1000, currency = INR.
      - If amount < 1000, currency = USD.
      - Else, currency = EURO.

4. *Currency Normalization*
   - Developed a formula to normalize the amount column into INR based on the currency column.

5. *Measure Creation*
   - Formulated a measure to calculate the sum of reimbursed amounts in INR.
   - Utilized the CALCULATE function to check the total reimbursed amount for Project_B (PROJECT B).

6. *Declined Requests*
   - Created a measure (declined) to count the number of declined requests.

7. *Visualization*
   - Implemented a slicer visual for easy selection of Project and employee.
   - Constructed a bar chart illustrating employees and their respective reimbursement amounts.
   - Designed a pie chart showcasing the distribution of reimbursement amounts across projects.

## Usage
Feel free to explore and utilize the provided analysis for insights into the reimbursement data. Customize and adapt the measures and visualizations to suit your specific requirements.

### Measures
- PROJECT B: Total reimbursed amount for Project_B.
- declined: Count of declined reimbursement requests.

### Visualizations
- Slicer visual for flexible Project and employee selection.
- Bar chart for a clear overview of employees and their reimbursement amounts.
- Pie chart for a visual breakdown of reimbursement amounts by Project.

## Dependencies
- Power Query for data transformation.
- Visualization tools compatible with the Power BI environment.

## How to Use
1. Clone the repository.
2. Open the dataset in your preferred environment supporting Power Query.
3. Execute the queries to reproduce the cleaned and transformed dataset.
4. Utilize the measures and visualizations for insightful data exploration.

Feel free to contribute, report issues, or enhance the analysis. Happy analyzing! 📊🚀
