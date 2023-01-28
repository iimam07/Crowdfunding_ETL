# Crowdfunding_ETL

Creates an ETL pipeline using Python, Pandas, Python dictionary methods  to extract and transform the data. Afterwards, four CSV files were created and used  to create an ERD and a table schema. Finally,  the CSV file data was uploaded into a Postgres database.

The Four Subsections
1. Category and Subcategory DataFrames

We extracted and transformed the crowdfunding.xlsx Excel data to create a category DataFrame, which have the followings columns: "category_id", "category"
Export the category DataFrame as category.csv

We extracted and transformed the crowdfunding.xlsx Excel data to create a subcategory DataFrame that has the following columns: "subcategory_id", "subcategory"


2. Campaign DataFrame

We created a copy of the crowdfunding_info_df DataFrame name campaign_df. Then we renamed the blurb column to description, the launched_at column to launch_date, and the deadline column to end_date.

Next, we converted the pledged columns to a float data type. Then we formatted the launch and end date columns to datetime formats. Next, we merged the campaign_df with the category_df on the "category" column and the subcategory_df on the "subcategory" column and used .tail(10) to view the last 10 rows.

Exported the campaign DataFrame as campaign.csv


3. Contacts DataFrame

Used Python dictionary methods for extracting and transforming the data from the contacts.xlsx Excel data

With the DataFrame, convert each row to a dictionary, and add values for each row to a new list

Split each "name" column value into a first and last name, and place each in a new column.

Clean and export the DataFrame as contacts.csv

Note: Both ETL_Mini_Project_Starters are the same, but we ran into some issues viewing one, so ETL_Mini_Project_Starter_Code might work better.

4. Crowdfunding Database

Inspect the four CSV files, and then sketch an ERD

Create a table schema for each CSV file

Create the tables in the correct order to handle the foreign keys

Verify the table creation by running a SELECT statement for each table

Import each CSV file into its corresponding SQL table

Verify that each table has the correct data by running a SELECT statement for each


Note: All the CSVs and ERD will be in the resources folder

