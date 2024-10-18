# Data Analysis on Sales Data project

## Perfrom Data analysis on sales data using MySQL, PowerBI



- [Setup MySQl database and PowerBI desktop on local ](#-STEP-1-:-Setup-MySql-database-and-PowerBI-destop-on-local)
- [Create database and tables in MySql ](#-STEP2:Create-database-and-tables-in-MySql)
- [EXTRACT data in PowerBI from MySQL server.](#-STEP3:EXTRACT-data-in-PowerBI-from-MySQL-server)
    - [connect SQL from PowerBI ](#:connection-details)
    - [local connection details](#:connection-details)
    - [extract the data](#:extract-data)
- [Data Modeling ](#STEP-4:-data-modeling)
- [TRANSFORM data in PowerBI ](#STEP5:-transform)
- [LOAD the data](#STEP-6:-Load-the-data-by-applying-transfromation)
- [Data Visualization](#STEP-7:-Data-Visualization-start-building-the-dashboard.)
- [Gather the Insights from dashboard](#STEP-8:-Gather-the-Insights.)


  

## STEP 1: Setup MySql database and PowerBI destop on local
    1. Download free version of Mysql server installation from below link 
    
   [MySql community Download](https://dev.mysql.com/downloads/file/?id=534319)

    2. Download MySql workbench to interact with database from below link

   [MySql workbench](https://dev.mysql.com/downloads/workbench/)

   3. Download free version of Power BI desktop from below link
      
   [PowerBI desktop download](https://www.microsoft.com/en-us/download/details.aspx?id=58494)

## STEP 2 :  Create database and tables in MySql

  Download and import database_prep_dump.sql file to database in MySQL workbench which will create required sales database along with tables

## STEP 3 :  EXTRACT data in PowerBI from MySQL server.

![Screenshot of step on how to connect sql from powerBI.](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/get_data_from_mySql_db.jpg)


 Connection details

 ![Connection details](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/connection_details.jpg)

 Load the data 
 ![Load the data](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Load_data.jpg)

 ## STEP-4:-data modeling

 Power will automatically establish releation between few tables and we can analyse and establish relationship on missing links as per requirement.
 In this case, we cna try to form STAR schema.

 ![Data modeling](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Data_modeling.jpg)

 ## STEP 5: Transform the data

 Data cleaning including removing unwanted rows and columns and normalise values. IN this example, converting values in same currency for all data as couple of entries in USD currency and rest of data in INR currency.
 

 ![Click on Transform data](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Transform_data_1.jpg)

Next, we can start transfromation. in this example, removing data where sales amount is less than on equal to 0 and convert USD amount into INR equivalent.

Additing new column as per given screenshot

![Add new transformed column](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/transformed_column.jpg)

applying formula
![apply formula](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/formula_transform_column.jpg)

we can filter rows where value is null or blank which is not required in this case.



## STEP 6 - Load the data by applying transfromation.

Click on close and apply button.

## STEP 7- Data Visualization - start building the dashboard.

1. creating base measaure table.
![create BaseMeasure table](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/base_mesaure.jpg)
Add new measaues Revenuew ande Sales Qty to this table by clicking three dots on right hands side of BaseMeasure - > New Measure

a. Revenue - sum(sales_amount)

b. Sales Qty- sum(sales_qty)

![New measures](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/new_measures.jpg)

2. Create charts.

   a. create Revenue and Sales qty cards by drag and drop these two from BaseMeasure to plot area.
![CARD chart](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Card_plot.jpg)

   as per above screenshot, repeate same step for Sales Qty.

   b. Horizant stack chart to show top 5 revenues by market.

![Horizontal stack chart](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Horizontal_stack_chart_2.jpg)

   c. SLicer for  year
![ Slicer](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/slicer_by_year.jpg)

Similarly, we can create slicer for month.
   
   d. Line chart to show revenue over time.
   ![Line chart](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Line_chart.jpg)

   We can re-arrange charts on dashboard as per requirement and Dashboard is ready now to be published.

   ![Dashboard](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/Dashboard.jpg)

## STEP8: Gather the insights

We can see from charts that revenue is declining ove year also we can see which market code or which region performing as per expectation or below expectation. Additionally, we cna see pain point area where focus is needed to overcome downside.

We cna Publish this dashboard if we have work email address. We cna set the frequency of publish or frequency of data retreival or alerts on any particular value in dahsboard.

We can also create mobile layover for this dashboard and publish accoridngly for stakeholders who want to refer in their mobile.

   

   





 



        
       



