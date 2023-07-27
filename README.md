# Home_Sales
# Introduction

I Used SparkSQL to determine key metrics about home sales data. Then use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.
finding

   -  What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places. The average price for four-bedroom houses sold fluctuates slightly from year to year. In 2019, the average price was $300,263.70, which decreased slightly to $298,353.78 in 2020. However, but we can see that the average price in 2020 was higher ($301,819.44), to decrease again in 20222 to ($296,363.88).

    - What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places. We can observe that the average price of homes with 3 bedrooms and 3 bathrooms does not show a consistent increasing or decreasing trend based solely on the year the home was built. The average prices fluctuate without a clear pattern or linear progression from year to year

    - What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places. according to the result we can see that depending on ther year that house was built is s not affecting the price of the house. The average prices fluctuate without a clear pattern or linear progression from year to year.

    - What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places. Based on the runtime results, it's evident that both the cached data and the Parquet formatted data have faster runtimes compared to the original data. This can be attributed to the optimizations and benefits offered by caching and using the Parquet data format. Parquet formatted data demonstrates the best runtime among the three options. By utilizing Parquet, you can achieve faster query performance, reduced storage requirements, and improved overall data processing efficiency.

# Conclusion

In conclusion, it's important to consider that the average price for homes is influenced by various factors. The provided data doesn't show a direct relationship between the year of construction and the average house price. Based on the runtime of the original data, cached data and parquet formatted data, parquet formatted data demonstrates the best runtime among the three options. The Parquet data format is indeed optimised for efficient processing and can provide better performance compared to other file formats like CSV or JSON, especially when dealing with large datasets. However, the runtime of a query can be influenced by various factors, including the size of the dataset, the complexity of the query, the available system resources, and the specific operations being performed. Additionally, runtime performance can vary depending on the specific dataset, hardware configuration, and the execution environment.
