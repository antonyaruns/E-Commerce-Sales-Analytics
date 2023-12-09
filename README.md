
#  E-Commerce Sales Analytics


## Dashboard Link: [Power Bi Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNmI1MGNhNTYtZDMyZS00NjZlLTg1MzUtZWVmMTk3ODAzYjZkIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

The project presents a comprehensive analysis of an e-commerce business, utilizing Power BI tools. Key performance metrics and trends are analyzed and displayed using a Power BI dashboard. The insights gained from this analysis can aid in informed decision-making and drive business growth. The project also includes forecasting techniques to predict future trends and performance.
## Project Overview

A US Bassed Ecommerce Sales Company wants us to create a Sales Dashboards showing information of YTD Sales and generate insights for below scenarios: 

- Create KPI banner showing YTD Sales, Profit, Quantity sold, Profit Margin.

- Find Year-on-year (YoY) growth for each KPI and show a YTD sparkline for each measure in the KPI to understand the monthly trend for each fact.

- Find YTD Sales, Past-Year-to-Date (PYTD) Sales, and YoY Sales growth for different customer category. Add a trend icon for each category.

- Find YTD Sales performance by each state.

- Top 5 and Bottom 5 products by sales.

- YTD Sales by region to know the best and worst performing regions all over contry.

- YTD Sales by shipping type to get the best shipping type percentage.
## Tools:

- Power BI (Power Query, Dax Query)
- MS SQL Server
- Excel
  
## Steps Covered: 



 
   - Downloaded dataset from Kaggle, consisting of `ecommerce_data.csv` and `us_state_long_lat_codes.csv`.

   - Imported data into MS SQL Server for efficient storage.

 
   - Established a connection between MS SQL Server and Power BI.


   - Connected `ecommerce_data` and `us_state_long_lat_codes` using the `customer_state` and `name` fields.

 - Created a new table using DAX queries:

    Calendar: `CALENDAR(MIN(ecommerce_data[order_date]), TODAY())`

    Year: `YEAR('Calendar'[date])`
    
    Month: `FORMAT('Calendar'[date], "mmmm")`

 
   - Linked `ecommerce_data` to the `Calendar` table based on the `order_date` and `Date` fields.


   - Added a background image to visualizations.
   
   - Created visualizations for:
      - YTD sales, YTD profit, YTD quantity, YTD profit margin.
      - Sales by category, sales by state.
      - Top 5 products YTD sales, bottom 5 products YTD sales.
      - YTD sales by region, YTD sales by shipping type.

 
   - Added three segments: consumer, corporate, home office.

## Dashboard Preview: 

![E-Commerce Sales Analytics](https://github.com/antonyaruns/E-Commerce-Sales-Analytics/assets/125898266/2e330206-e584-4c13-be7d-a1c21ba61ecd)

## Conclusion: 

This project has been successfully completed as part of a learning portfolio project aimed at practicing the creation of interactive dashboards on PowerBI as a beginner. The key learning takeaways from this project include:

- How to connect PowerBI to MS SQL server and flat files
- Data modeling with three tables
- Data cleaning in Power Query
- How to create a data table in Power BI
- Time intelligence functions (TOTALYTD, SAMEPERIODLASTYEAR, etc)
- Creating dynamic and complex KPI's
- Basic to Advanced Dax Queries
- Conditional Formatting, Adding dynamic icons in Power BI
- Creating different charts, maps and formatting them
- Generating insights from charts
- Export report
