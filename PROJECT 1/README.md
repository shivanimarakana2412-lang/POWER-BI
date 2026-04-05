~ 1. Data Extraction : 

Load an HTML table from a website

Load 3 Excel files : Sales_Jan.xlsx , Sales_Feb.xlsx , Sales_Mar.xlsx

Use Append Queries from Folder to combine the sales files.

Load an Employee dataset from another Excel file


~ 2. Basic Transformations :

Promote the first row to headers.

Rename columns to clear and meaningful names.


~ 3. Text Tools :

UPPER() - converts text to uppercase in payment_method column - Table : Append_Three_month_data

LOWER() - converts text to lowercase in column description column - Table : Product_from_web

TRIM() - removes extra spaces in id column - Table : Product_from_web

CLEAN() - clean text in Total_Amountcolumn - Table : Append_Three_month_data

DELIMATERS - extract text from website column - Table : Product_from_web


~ 4. Numeric Tools :

Round off - two decimal from price columns - Table : Product_from_web


~ 5. Date & Time Tools :

Work with Order Date column extract : Day , Month , Year , Quarter - Table : Append_Three_month_data
 
Create Fiscal Month column using : Add Column → Date → Month in - Table : Append_Three_month_data


~ 6. Conditional Columns & Indexing :

Conditional Column -> Create a Sales Category column -> by using formulas - Table : Product_from_web

Add 0 based index - Table : Append_Three_month_data


~ 7. Pivoting & Unpivoting :

It's doesn't match with my data so couldn't do it .


~ 8. Merging & Appending : 

Use Append Queries from Folder to combine the sales files.

Merge Sales data with Employee data using Region.


~ 9. Grouping & Aggregation :

Use group by with advance option ->sum of total Amount column name : Total Sales , average of total Amount column name : Average Order Value and count rows column name : Transaction Count  :- Table : Apr_Sales_data


~ 10. Data Profiling & Quality :

Column Profile , Column Distribution , Column Quality : Find missing values , Detect errors , See unique and distinct values


12. Refresh Simulation :

I also Add new file : Sales_Apr.xlsx







 