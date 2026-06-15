## relational-sql-bike-analytics
A structured, purely relational SQL analytics project optimizing multi-table JOINs and aggregate functions to evaluate retail performance, customer distributions, and zero-stock inventory metrics for a bicycle retail chain.

## 🗄️ Database Schema & File Structure
The project utilizes 9 structured CSV datasets representing a typical retail and production ecosystem:

* [cite_start]**`stores.csv`**: Contains store details including `store_id` and `store_name`[cite: 4, 18].
* [cite_start]**`customers.csv`**: Holds customer profile data mapped by `customer_id`[cite: 6].
* [cite_start]**`orders.csv`**: Core transaction ledger connecting `order_id`, `customer_id`, `store_id`, and `order_date`[cite: 6, 18].
* [cite_start]**`order_items.csv`**: Line-item details containing `order_id`, `product_id`, `quantity`, `list_price`, and `discount`[cite: 18].
* [cite_start]**`products.csv`**: Master catalog mapping `product_id`, `product_name`, `brand_id`, and `category_id`[cite: 5, 7].
* **`brands.csv`**: Contains manufacturer names mapped by `brand_id`[cite: 7].
* **`categories.csv`**: Structural categorization for inventory classes.
* **`stocks.csv`**: Real-time warehouse balance tracking matching `store_id`, `product_id`, and `quantity`[cite: 8].
* **`staffs.csv`**: Employee operational assignments across branches.

## 🔗 Data Source
The relational tables utilized in this analysis were extracted from the **[Bike Store Sample Database on Kaggle](https://www.kaggle.com/datasets/dillonmyrick/bike-store-sample-database)** (originally sourced from standard relational database sample collections).
