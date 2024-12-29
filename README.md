# Hardware Company Sales Analytics SQL Project

## Overview
Advanced SQL implementation for analyzing and optimizing sales data for a hardware company, featuring performance-tuned queries, stored procedures, and analytical views for business intelligence reporting.

## Database Structure
- 10 interconnected tables
- 2M+ records
- Key tables include:
  - fact_sales_monthly
  - fact_gross_price
  - fact_pre_invoice_deductions
  - fact_post_invoice_deductions
  - dim_product
  - dim_customer
  - dim_date

## Technical Implementation

### Performance Optimization
1. Query Performance Improvements:
   - Implemented dimensional modeling using date dimension table
   - Added fiscal year column to fact tables reducing function calls
   - Optimized JOIN operations for faster data retrieval

### Advanced SQL Features Implemented
1. Common Table Expressions (CTEs):
   - Net sales calculations
   - Customer-wise sales distribution
   - Regional performance analysis

2. Window Functions:
   - ROW_NUMBER, RANK, DENSE_RANK for sales analysis
   - OVER clause with PARTITION BY for market share calculations
   - Running totals and percentages

3. Views:
   - sales_preinv_discount
   - sales_postinv_discount
   - net_sales

4. Stored Procedures:
   - get_top_n_markets_by_net_sales
   - get_top_n_customers_by_net_sales
   - get_top_n_products_per_division_by_qty_sold

### Key Features
- Pre and post-invoice discount analysis
- Market and customer segmentation
- Product division performance tracking
- Fiscal year-based reporting
- Customer net sales distribution

## Business Impact
- Automated sales performance reporting
- Enhanced data retrieval efficiency
- Streamlined analytical processes
- Improved decision-making capabilities

## Skills Demonstrated
- Complex SQL query optimization
- Database performance tuning
- ETL process design
- Business intelligence reporting
- Data modeling

## Future Enhancements
- Additional performance optimization
- Enhanced reporting capabilities
- Automated ETL processes
- Advanced analytics integration
