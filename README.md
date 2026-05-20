# E-Commerce Product Analysis Project

# Step 1: Start Spark Session

## Objective
The first step of the project is to initialize and start the Apache Spark session using PySpark. This session connects the Jupyter Notebook environment with the Spark engine.

## Purpose of This Step
- Starts the Spark environment for big data processing  
- Establishes communication with PySpark engine  
- Prepares system for loading and analyzing datasets  
- Verifies Spark configuration in Jupyter Notebook  

## Output
The successful output confirms that Spark session has started and the environment is ready for analysis.

---

# Step 2: Load Product Dataset

## Objective
Load the e-commerce product dataset into a Spark DataFrame for analysis.

## Purpose of This Step
- Load dataset into Spark  
- Convert CSV into structured DataFrame  
- Prepare data for processing  
- Display sample records  

## Expected Output
Columns include:
- product_id  
- product_category_name  
- product_photos_qty  
- product_weight_g  
- product_length_cm  
- product_height_cm  
- product_width_cm  

---

# Step 3: Load Order Items Dataset

## Objective
Load order items dataset containing pricing and seller information.

## Purpose of This Step
- Load dataset into Spark  
- Provide product price information  
- Include seller and freight details  
- Support price analysis  

## Expected Output
Columns include:
- order_id  
- product_id  
- price  
- freight_value  
- seller_id  

---

# Step 4: Find Most Expensive Product

## Objective
Identify the most expensive product using joined datasets.

## Purpose of This Step
- Combine product + price data  
- Perform dataset joins  
- Identify highest priced product  
- Apply sorting operations  

## Expected Output
- product_id  
- product_category_name  
- highest price value  

---

# Step 5: Group Products by Category

## Objective
Analyze product distribution by category.

## Purpose of This Step
- Group products by category  
- Count products per category  
- Analyze category distribution  
- Use groupBy and aggregation  

## Expected Output
- product_category_name  
- count of products  

---

# Step 6: Count Products per Category

## Objective
Count and sort products per category.

## Purpose of This Step
- Group data by category  
- Count total products  
- Sort in descending order  
- Identify most common categories  

## Expected Output
- product_category_name  
- product count (sorted)

---

# 📊 Conclusion

This project demonstrates big data processing using PySpark. It helps analyze e-commerce product data, pricing trends, and category distribution efficiently using Apache Spark in Jupyter Notebook.
