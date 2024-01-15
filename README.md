This SQL script addresses diverse aspects of database management, performance optimization, and analytical reporting for a hardware company. 
Below is a breakdown of key sections:

### Problem Statement and Pre-Invoice Discount Report
- Detailed reports on sales data with pre-invoice deductions.
- Two versions: specific to a customer and fiscal year, and inclusive of all customers for a given fiscal year.

### Performance Improvement #1
- Creates 'dim_date' table for enhanced query efficiency.
- Elimination of 'get_fiscal_year()' function to reduce query execution time.

### Performance Improvement #2
- Addition of the fiscal year directly to 'fact_sales_monthly' table for optimized query performance.

### Database Views: Introduction
- Introduction of database views.
- Generation of 'net_invoice_sales' amount using CTEs.
- Creation of 'sales_preinv_discount' view to store data as a virtual table.

### Database Views: Post Invoice Discount, Net Sales
- Creation of 'sales_postinv_discount' view with post-invoice deductions.
- Establishment of 'net_sales' view utilizing previous views for ultimate net sales figures.

### Top Markets and Customers
- Queries to identify top markets and customers by net sales.
- Introduction of stored procedures for dynamic retrieval of top markets and customers.

### Window Functions: OVER Clause
- Window functions with 'OVER' clause for percentage calculations and per-category distributions.
- Demonstration of window functions in generating cumulative expenses.

### Window Functions: Using it In a Task
- Window functions to determine customer-wise net sales percentage contributions for a specific fiscal year.

### Exercise: Window Functions: OVER Clause
- Exercise to find customer-wise net sales distribution per region for a given fiscal year.

### Window Functions: ROW_NUMBER, RANK, DENSE_RANK
- Examples of using 'ROW_NUMBER', 'RANK', and 'DENSE_RANK' to extract top expenses and rank student marks.
- Query to identify top products from each division based on total quantity sold.

This script provides a comprehensive approach to database management and analytics using SQL, offering insights into performance optimization techniques and the utilization of window functions. Feel free to incorporate and customize these SQL queries based on your specific requirements.
