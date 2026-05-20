# E-Commerce Product Analysis Project



# Step 1: Start Spark Session

## Objective:
The first step of the project is to initialize and start the Apache Spark session using PySpark. This session creates the connection between the Jupyter Notebook environment and the Spark engine, allowing big data processing operations to be performed.

## Purpose of This Step:
This step is important because it:
- Starts the Spark environment for big data processing
- Establishes communication with the PySpark engine
- Prepares the system for loading and analyzing e-commerce datasets
- Verifies that Spark is configured correctly in Jupyter Notebook

## Output:
The successful output confirms that the Spark session has been initialized correctly and the environment is ready for further data analysis tasks.

---

# Step 2: Load Product Dataset:

## Objective:
The second step of the project is to load the e-commerce product dataset into a Spark DataFrame. This allows the raw CSV file to be transformed into a structured format for big data analysis and processing.

## Purpose of This Step:
This step is important because it:
- Loads the e-commerce product dataset into Spark
- Converts raw CSV data into a structured DataFrame
- Prepares the dataset for analysis and transformation
- Confirms successful data loading by displaying sample records

## Expected Output:
After executing the code, Spark displays the first five rows of the dataset in tabular form.
The output contains columns such as:
- product_id
- product_category_name
- product_photos_qty
- product_weight_g
- product_length_cm
- product_height_cm
- product_width_cm

This output confirms that the dataset has been successfully imported into the Spark environment and is ready for further analysis.

---

# Step 3: Load Order Items Dataset:

## Objective:
The third step of the project is to load the order items dataset into a Spark DataFrame.

This dataset contains important information about product prices, seller details, and freight charges, which are required for product price analysis and identifying the most expensive products.

## Purpose of This Step:
This step is important because it:
- Loads the order items dataset into Spark
- Provides product pricing information for analysis
- Includes seller and freight details related to orders
- Helps identify the most expensive products in the e-commerce dataset
- Verifies correct data loading by displaying sample records

## Expected Output:
After running the code, Spark displays the first five rows of the dataset in table format.
The output includes columns such as:
- order_id
- product_id
- price
- freight_value
- seller_id

This confirms that the order items dataset has been successfully imported and is ready for further analysis in the project.

---

# Step 4: Find the Most Expensive Product:

## Objective:
The fourth step of the project is to identify the most expensive product in the e-commerce dataset. Since the product details and price information are stored in separate datasets, both datasets must be joined before performing the analysis.

## Purpose of This Step:
This step is important because it:
- Combines product information with pricing data
- Allows analysis using data from multiple datasets
- Identifies the most expensive product in the dataset
- Demonstrates how joins are performed in PySpark
- Uses sorting operations for analytical queries

## Expected Output:
After executing the code, Spark displays one row containing the most expensive product.
The output includes:
- product_id
- product_category_name
- price (highest value in the dataset)

This confirms that the datasets were successfully joined and the highest-priced product was identified correctly.

---

# Step 5: Group Products by Category:

## Objective:
The fifth step of the project is to analyze how products are distributed across different categories by grouping the dataset based on the product category and counting the number of products in each category.

## Purpose of This Step:
This step is important because it:
- Groups products according to their category
- Calculates the total number of products in each category
- Helps in understanding category-wise distribution of products
- Provides insights into which categories are more populated
- Demonstrates the use of groupBy() and aggregation functions in PySpark

## Expected Output:
After executing the code, Spark displays a table containing product categories along with the number of products in each category.
The output includes:
- product_category_name
- count (number of products in each category)

Result Interpretation:
This output confirms that the dataset has been successfully grouped by category, and the count of products in each category has been calculated correctly. It helps in analyzing product distribution and identifying high-volume categories in the dataset.

---

# Step 6: Count Products per Category:

## Objective:
The sixth and final step of the project is to calculate the number of products in each category and present the results in a sorted format to identify the most populated categories.

## Purpose of This Step:
This step is important because it:
- Groups products based on their category
- Counts the total number of products in each category
- Sorts the categories in descending order of product count
- Provides a clear ranking of categories based on size
- Improves readability and supports better data analysis
- Demonstrates the use of groupBy(), count(), and orderBy() functions in PySpark

## Expected Output:
After executing the code, Spark displays a table showing product categories sorted by the number of products in descending order.
The output includes:
- product_category_name
- count (number of products in each category, sorted highest to lowest)

Result Interpretation:
This output confirms that the dataset has been successfully grouped, counted, and sorted.
It helps identify the most and least common product categories in the dataset, making it useful for business insights such as demand analysis and inventory planning.

---

This step groups products by category and counts the number of products in each category. The results are sorted in descending order to identify the most frequent product categories in the dataset.
