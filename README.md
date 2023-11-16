# Home_Sales

## Background
The Home_Sales_starter_code_colab.ipynb file was provided for this challenge.  I have coded in 
Working with Big Data in this challenge, SparkSQL was used to determine key metrics about home sales data. 
Then, I used Spark to create temporary views, to partition the data and to cache + uncache a temporary table. 
The final step was to verify that the table had indeed been uncached.
________________________________________
## Instructions

1.	Renamed the *Home_Sales_starter_code_colab.ipynb* file which was provided as *Home_Sales.ipynb*.

2.	Imported the necessary PySpark SQL functions for this assignment.

3.	Read the *home_sales_revised.csv* data in the starter code into a Spark DataFrame.

4.	Created a temporary table called *home_sales*.

5.	Answered the following questions using SparkSQL:

    •	What is the average price for a four-bedroom house sold for each year?  The answer was rounded off to two decimal places.

     ![image](https://github.com/Mago281/Home_Sales/assets/131424690/c2a4d03b-3517-4349-88ec-41e379feb522)


    •	What is the average price of a home for each year it was built that has three bedrooms and three bathrooms?  The answer was rounded off to two decimal places.

     ![image](https://github.com/Mago281/Home_Sales/assets/131424690/b7b0d2e9-70d2-4662-91c7-0bcf7699071b)


    •	What is the average price of a home for each year built that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?  Rounded off the answer to two decimal places.

     ![image](https://github.com/Mago281/Home_Sales/assets/131424690/050989c8-f42d-4bb6-8423-ce85f8a14b03)


  •	What is the "view" rating for homes costing more than or equal to $350,000?  The answer was rounded off to two decimal places and the runtime was determined.  
      ![image](https://github.com/Mago281/Home_Sales/assets/131424690/f8d76388-c05d-4b75-8c45-27d0c80eddd5)

    

6.	Cached the temporary table home_sales_data.


7.	Checked if the temporary table was cached.


8.	Using the cached data, I ran a query that filtered out the view ratings with an average price of greater than or equal to $350,000 and determined the runtime.  This runtime result was then compared to the uncached runtime.

    ![image](https://github.com/Mago281/Home_Sales/assets/131424690/68b8de68-d383-4149-872e-16ab62e785ad)

  
The runtime for the cached data above was quicker at 0.6312069892883301 seconds while the uncached runtime was 0.8923213481903076 seconds.


9.	Partitioned by the "date_built" field on the formatted parquet home sales data.


10.	Created a temporary table for the parquet data.


11.	Ran the query that filtered out the view ratings with an average price of greater than or equal to $350,000 and determined the runtime and compared it to uncached runtime.

    ![image](https://github.com/Mago281/Home_Sales/assets/131424690/acb61a39-ef80-42b0-827e-e0ca7099a0f5)


The runtime for the above analysis is 1.1581673622131348 seconds while the runtime for the cached version was faster at 0.6312069892883301 seconds.

12.	Uncached the home_sales temporary table.


13.	Verified that the home_sales temporary table is uncached using PySpark.


14.	Download your Home_Sales.ipynb file has been uploaded into this GitHub repository.

