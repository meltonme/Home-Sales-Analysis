# Analysis of Home Sales using SparkSQL

### Overview:
I was able to use my knowledge of SparkSQL to determine key metrics about home sales data.

### I used Spark to create:
- Temporary Views
- Partition the Data
- Cache and Uncache a Temporary Table
- Verify that the table has been uncache

### Observations:
- Without the cache, the querry took 1.7921223640441895 seconds
- With the cache, the querry took: 2.430140495300293 seconds
- After partetioning the parquet home sales, the query took 1.6986093521118164

## Questions Answered using SparkSQL:
- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.
- What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.
- What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.
- What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

## Activities using SparkSQL:
-  Cache your temporary table home and check if the temporary table has been cached.
-  Using the cached data, run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
-  Partition by the "date_built" field on the formatted parquet home sales data and create a temporary table for the parquet data.
-  Run the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
-  Uncache the home temporary table and verify that it has been uncached using PySpark.
