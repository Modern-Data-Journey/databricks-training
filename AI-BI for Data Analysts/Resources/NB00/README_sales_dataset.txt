Synthetic sales dataset for Databricks training

Grain:
- ca_orders: one row per order line (fact table)
- ca_customers: one row per customer
- ca_products: one row per product
- ca_sales_reps: one row per sales representative
- ca_sales_targets: one row per year and sales representative
- ca_opportunities: one row per sales opportunity

Relationships:
- ca_orders.customer_id -> ca_customers.customer_id
- ca_orders.product_id -> ca_products.product_id
- ca_orders.salesrep_id -> ca_sales_reps.salesrep_id
- ca_sales_targets.salesrep_id -> ca_sales_reps.salesrep_id
- ca_opportunities.customer_id -> ca_customers.customer_id
- ca_opportunities.product_id -> ca_products.product_id
- ca_opportunities.salesrep_id -> ca_sales_reps.salesrep_id

All values are synthetic and do not represent real persons or companies. Currency is EUR. Dates use ISO 8601 YYYY-MM-DD.
