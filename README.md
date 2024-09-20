# Data integration project using AWS Glue and Pyspark
This a data integration project to consolidate user, order, and product information from multiple JSON files into a single merged JSON file. The tasks involves several steps, including schema inference, data transformation, and writing results to a data catalog table. Identify the difference in schema and final dataframe and generate the output. 
Requirements:

# Schema Inference:

There a CSV file named schema.csv that describes the schema of the final DataFrame. The CSV file is stored in an S3 bucket at s3://your-bucket/schema.csv. Using AWS Glue Crawler, infer the schema from the schema.csv file and create a table in the Glue Data Catalog.

# Data Transformation:

There are three JSON files stored in S3: users.json (located at s3://your-bucket/users.json) orders.json (located at s3://your-bucket/orders.json) products.json (located at s3://your-bucket/products.json) These JSON files contain user, order, and product information respectively.

# The goal is to:

Flatten the JSON structures. Join the data based on appropriate keys. Produce a single merged JSON file.

# Write to Glue Table:

Write the resulting merged JSON data to a table in the Glue Data Catalog. The table should be named merged_data_table and should be stored in the S3 location s3://your-bucket/merged_data/.

