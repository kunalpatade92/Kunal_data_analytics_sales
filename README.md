# Data Analysis to get Sales insights

- [Setup MySQl database and PowerBI desktop on local ](#-STEP-1-:-Setup-MySql-database-and-PowerBI-destop-on-local)
- [Create database and tables in MySql ](#-STEP2:Create-database-and-tables-in-MySql)
- [EXTRACT data in PowerBI from MySQL server.](#-STEP3:EXTRACT-data-in-PowerBI-from-MySQL-server)
    - [connect SQL from PowerBI ](#:connection-details)
    - [local connection details](#:connection-details)
    - [extract the data](#:extract-data)
- [Data Modeling ](#STEP-4:-data-modeling)
- [TRANSFORM data in PowerBI ](#STEP5:-transform)
  

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

creating base measaure table.
![create BaseMeasure table](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/base_mesaure.jpg)
Add new measaues Revenuew ande Sales Qty to this table by clicking three dots on right hands side of BaseMeasure - > New Measure

a. Revenue - sum(sales_amount)

b. Sales Qty- sum(sales_qty)

![New measures](https://github.com/kunalpatade92/Kunal_data_analytics_sales/blob/main/src/new_measures.jpg)



 



        
       



