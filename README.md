# Python and SQL Coding and Data Science About Customer Segmentation and Prediction Regarding the Incremental Sales Opportunities

*The report notebook (pdf, html, and ipynb versions are avaliable in the Root directory)*

## 1st Half:
### TASK 1 - [DS_SAMPLE.csv]
- Using the dataset provided in DS_SAMPLE.csv:
    1. For each "Type" in Column A:
        A- What is the count of "PO NUMBER" by "WHS"?
        B- What is the sum of "PALLET", "TOTAL CUBE", "TOTAL CASES", "TOTAL WGHT" by "VENDOR NUMBER"?
    2. Using the "SCHEDULE DATE":
        A- What is the mean of "PALLET" by day of the week?
        B- What is the average number of days between "CREATION DATE" & "SCHEDULE DATE"
        C- Using the information calculated in B, identify rows that you consider to be "outliers". Please comment on how you decided on what is and is not an outlier.
        D- Prepare a simple time series plot showing "TOTAL WGHT" over time
        E- For every "BYR", identify the "UPC" with the most "TOTAL CASES" ordered across time
 
### TASK 2 - [Basic OOP]
- Using Python:
    1. Design a class with two variables, checking account and savings account
        - Create Functions to Deposit, Withdraw, and Transfer money between accounts
        - Design it so every transaction is recorded into a dictionary with the date and time of the transaction as the key, with account(s) involved & amounts as the values
    2. Once you have done that, do the following:
        - Deposit 1000 dollars in checking and 500 into savings
        - Transfer 500 from checking to savings
        - Deposit 250 to checking
        - Withdraw 500 from savings
        - Output the dictionary with all transactions
 
### TASK 3- [SQL_SAMPLE.CSV]
The sample file [SQL_SAMPLE.csv] provides a dataset that is essentially joined from multiple sources - showing item data, yearly sales/cost data, location data and daily stocklevels.
Your goal is to:
  1. Insert the file into a SQLite database using Python
  2. Normalize the database within SQLite using SQL - create as many tables as you think are appropriate
  3. Utilize indexing on tables created in step 2
  4. Using SQL syntax (please write the SQL queries within Python in a string/docstring), answer the following questions:
     - What are the top 3 selling products by Branch and Item #?
     - Calculate the 3-day moving average of DailyStocklevel by Branch and UPC
     - What is the lowest selling item for each group?
     - What is the best selling item for each branch by department?
  5. What can you tell us about the association between Item #s, PrimaryUPCs and UPCs?
  6. Feel free to add any other insights you gathered during this exercise.


## 2nd Half:

•	The data is the information on possible incremental sales to customers by departments that we have identified. Each row is a unique customer while each column represents a category of products.
•	The values contained are the dollar amount potential incremental sales for a customer/category combination.

I am doing:
1.	Group together customers with similar potential sales opportunities - this would help our marketing teams create targeted campaigns for each group of customers
2.	Find sets of customers with similar properties with respect to their categories and sales opportunities
3.	Have an easy-to-understand way of describing a typical customer from each of the sets/groups that you devise
4.  Train model for grouping the customers (supervised learning, with model selection, variable selection, customer segmentation, parameter tuning, and evaluations)
5.  Build similarity algorithms for finding top similar customers for any specific customer based on the raw data
