🚚 Food Delivery Data Integration & Analysis


📌 Project Overview
This project simulates a real-world data engineering task: consolidating fragmented data from multiple sources into a single, analysis-ready dataset. The goal was to merge transactional data with user and restaurant master records to provide a comprehensive view of food delivery operations.

📂 Data Sources
The project utilizes three distinct file formats to simulate a heterogeneous data environment:

orders.csv: Transactional data containing order_id, user_id, restaurant_id, and order amounts.

users.json: User master data including names, emails, and membership tiers.

restaurants.sql: Restaurant master data containing names and cuisine types.

🛠️ Technical Workflow
Data Loading: Utilized pandas for CSV/JSON and sqlite3 for SQL database extraction.

Data Merging:

Performed a Left Join between Orders and Users using user_id.

Performed a Left Join between the result and Restaurants using restaurant_id.

Note: Left Joins were used to ensure 100% retention of transactional order data.

Final Export: Generated a consolidated file named final_food_delivery_dataset.csv.

📈 Key Insights Captured
By combining these datasets, we can now answer critical business questions such as:

Which cuisine types drive the highest revenue?

How do order frequencies differ across various membership tiers?

Which users are most active in specific restaurant categories?

🚀 How to Run
Clone this repository.

Ensure you have pandas installed: pip install pandas.

Run the Jupyter Notebook or Python script to generate the final dataset.
