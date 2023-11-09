# Home_Sales

In this challenge, you'll use your knowledge of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

**Instructions**

1. Rename the Home_Sales_starter_code.ipynb file as Home_Sales.ipynb.

2. Import the necessary PySpark SQL functions for this assignment.

3. Read the home_sales_revised.csv data in the starter code into a Spark DataFrame.

4. Create a temporary table called home_sales.

5. Answer the following questions using SparkSQL:

    What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

    ![image](https://github.com/amccollough1/Home_Sales/assets/133404805/f8161593-c5d2-405f-9314-ec0a15901efa)



    What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

   ![image](https://github.com/amccollough1/Home_Sales/assets/133404805/f6e8c061-36ea-4f37-8397-db9571872fd2)



    What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

    ![image](https://github.com/amccollough1/Home_Sales/assets/133404805/a5dfadca-7fbe-4e2f-b7d7-14e7e6798c9b)


    What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

![image](https://github.com/amccollough1/Home_Sales/assets/133404805/84962fed-f9f0-4d0b-b810-20a7e080c679)


6. Cache your temporary table home_sales.
  
 ![image](https://github.com/amccollough1/Home_Sales/assets/133404805/b0477707-55b7-4f15-a802-23369ad37616)


7. Check if your temporary table is cached.

   ![image](https://github.com/amccollough1/Home_Sales/assets/133404805/baee7d7b-2475-43d4-a7ea-e7c9615d0309)


8. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

   ![image](https://github.com/amccollough1/Home_Sales/assets/133404805/16deb5e9-c6d9-4204-8751-b4c473f5adbe)

     Using the cached data we see that the runtime is slightly faster than the uncached runtime. 


9. Partition by the "date_built" field on the formatted parquet home sales data.

10. Create a temporary table for the parquet data.

11. Run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime.

![image](https://github.com/amccollough1/Home_Sales/assets/133404805/3cfbfeb7-f957-495a-b429-e99731e8fc88)

    From this query we show that the runtime takes longer than the uncached runtime. 


12. Uncache the home_sales temporary table.

![image](https://github.com/amccollough1/Home_Sales/assets/133404805/69add2df-5e04-4a8b-a435-102aa4563277)

13. Verify that the home_sales temporary table is uncached using PySpark.

![image](https://github.com/amccollough1/Home_Sales/assets/133404805/8861a899-028c-47b9-bf62-bcd7e179193f)

14. Download your Home_Sales.ipynb file and upload it into your "Home_Sales" GitHub repository.
