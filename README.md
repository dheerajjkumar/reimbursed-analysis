# reimbursed-analysis
 # What i done in this
 # Import the data and open the Power Query
 # The expense type column has some spelling and punctuation errors, correct them
 # Project names are not uniform, make it uniform.
 # The Currency column has some missing values, based on the amount, create a new custom column.
 # Condition: amount >= 1000, = INR; amount < 1000, = USD; else = EURO
 # Formula: (if [Currency] = null and [Amount] >= 1000 then "INR" else if [Currency] = null and [Amount] < 1000 then "USD" else [Currency] )
 # Normalize the amount column into INR based on the currency column.
 # Create a measure to calculate the sum of reimbursed amount in INR.
 # Use the calculate function and check the total reimbursed amount for Project_B
 PROJECT B = CALCULATE([sum inr],reimbursement[Project_Name]="Project_B")
 # Create a measure to check the count of declined requests.
 declined = CALCULATE(COUNTROWS(reimbursement),reimbursement[Approval_Status]="Declined")
 # Create a slicer visual for the Project and employee
 # Create a bar chart for employees and reimbursement amount.
 # Create a pie chart for Project vs reimbursement amount.
