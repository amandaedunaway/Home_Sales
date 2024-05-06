# Home_Sales
Module 22 Challenge

## Outline
The purpose of this assignment was to practice using Spark and illustrate the decreased processing time that results from caching tables and using parquet data.

`Home_sales.ipynb` reads in data from an S3 bucket into a DataFrame and creates a temporary view to perform SQL queries. The queries return select information about home sales data from the years 2019 - 2022. For the final query, the runtime for a non-cached table is compared to a cached table and partitioned parquet table, with the runtime decreasing for each step.

## Resources
I determined to use the `.partitionBy()` function for Item #10 from [Stack Overflow](https://stackoverflow.com/questions/34789604/dataframe-partitionby-to-a-single-parquet-file-per-partition). 