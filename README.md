# Market-Analysis-Report-for-National-Clothing-Chain

Sales have been flat for an online national clothing chain. They want to lure lost customers back. They want to advertise specific products to specific customers in specific locations. Some of the products they carry are:

*	Shirt: $25
*	Sweater: $100
*	Leather Bag: $1000

I conducted an analysis to determine the best product to advertise to each customer.

The project uses a variety of data sources, including
## US Census Bureau

* Average Income
* Location
* Population
* Industry

## Business Data

* Product Inventory
* Product Prices
* Customer Rating
* Product Return Rate

## Customer Data

* Customer ID
* Names
* Location
* Date of Birth
* Purchase History

## Additional Data

* Weather

## Data Processing

* Imported the **census data, customer list, purchase list and state list into Power BI**.
* Formatted, transformed, and cleaned the data in Power Query.
* Set up table relationships, following a star schema.
* The **purchase list** contains all sales transaction dates and corresponding transaction amounts. I unpivoted the data (flattened the data) to put it in a matrix format (all dates are in one column and all transaction amounts are in a different column).
* Additional data: Imported weather data into Power BI.
* Created a new table called **Regression Table** from the customer list to summarize the average customer sales by state. Set up calculated columns and created DAX measures to predict customer incomes (set up sales as x and used y = mx + b to predict customer income).

## Data Analysis | Visualization

Created visualizations to make sense of the data.

* Created a scatterplot with **r²** value to show a positive relationship between **average incomes** and **average sales by state**.
* Created a calculated column in the **customer list** table for **predicted customer incomes**.
* Categorized the predicted customer incomes into ranges using DAX to determine the best product fit for each customer (histogram on **Customer Insights** tab).
* Visualized household income distribution across the U.S. using a heatmap.
* Created a scatter plot with **r²** value to show a negative relationship between **customer rating** and **product return rate**.

## Summary

* There is a **strong positive linear relationship** between **average sales** and **average income**.

![Average Sales vs. Average Income image]()
















