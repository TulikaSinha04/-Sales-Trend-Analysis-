# Sales Trend Analysis Using Aggregations

## Objective
Analyze monthly revenue and order volume from the `online_sales` dataset to understand sales trends and patterns over time.

## Dataset
**Data Name:** `online_sales_grocery.csv`  

**Columns:**
- `order_id` – Unique identifier for each order  
- `order_date` – Date when the order was placed
- `order_time` – Time when the order was placed  
- `amount` – Revenue amount for the order  
- `product_id` – Identifier for the product
- `product_name` – Identifier for the product name
- `customer_name` – Identifier for the customer name  

## Tools
- MySQL 
- SQL queries with aggregation functions  

## Methodology
1. **Extract Year and Month**  
   Use SQL `EXTRACT(YEAR FROM order_date)` and `EXTRACT(MONTH FROM order_date)` to break down order dates by year and month.

2. **Aggregate Revenue**  
   Use `SUM(amount)` to calculate total revenue per month.

3. **Count Orders**  
   Use `COUNT(DISTINCT order_id)` to calculate total orders per month.

4. **Group and Sort Data**  
   Use `GROUP BY` year and month to aggregate monthly data and `ORDER BY` to sort results chronologically.

5. **Optional Filtering**  
   Use `WHERE` to limit results to a specific time period if needed.

## SQL Query File
`online_sales_groceries_queries.sql`

## Results
`all_data.csv`
`month_year.csv`
`particular_year(2024).csv`
`last_six_month.csv`

## Detailed File (with all steps)
`Task6.pdf`
