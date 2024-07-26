# Crowdfunding_ETL
Project Overview
This mini project involves extracting, transforming, and loading data from Excel files into a PostgreSQL database. The project is divided into several key tasks:

Create the Category and Subcategory DataFrames
Create the Campaign DataFrame
Create the Contacts DataFrame
Create the Crowdfunding Database
Instructions
1. Create the Category and Subcategory DataFrames
Category DataFrame
Objective: Extract and transform data from crowdfunding.xlsx to create a category DataFrame.
Columns:
category_id: Sequential entries from cat1 to catn.
category: Titles of the categories.
Export: Save the DataFrame as category.csv.
Subcategory DataFrame
Objective: Extract and transform data from crowdfunding.xlsx to create a subcategory DataFrame.
Columns:
subcategory_id: Sequential entries from subcat1 to subcatn.
subcategory: Titles of the subcategories.
Export: Save the DataFrame as subcategory.csv.
2. Create the Campaign DataFrame
Objective: Extract and transform data from crowdfunding.xlsx to create a campaign DataFrame.
Columns:
cf_id
contact_id
company_name
description (formerly blurb)
goal: Converted to float
pledged: Converted to float
outcome
backers_count
country
currency
launch_date: Renamed from launched_at and converted to datetime format
end_date: Renamed from deadline and converted to datetime format
category_id: Match category_id in the Category DataFrame
subcategory_id: Match subcategory_id in the Subcategory DataFrame
Export: Save the DataFrame as campaign.csv.
3. Create the Contacts DataFrame
Choose one of the following options:

Option 1: Using Python Dictionary Methods
Import contacts.xlsx into a DataFrame.
Convert each row to a dictionary and extract values using list comprehension.
Create a new DataFrame and split the name column into first_name and last_name.
Export the DataFrame as contacts.csv.
Option 2: Using Regular Expressions
Import contacts.xlsx into a DataFrame.
Use regular expressions to extract contact_id, name, and email.
Create a new DataFrame and split the name column into first_name and last_name.
Export the DataFrame as contacts.csv.
4. Create the Crowdfunding Database
Sketch an ERD: Inspect the CSV files and create an Entity-Relationship Diagram (ERD) using QuickDBD.
Create Table Schema: Define schemas for each table in the crowdfunding_db_schema.sql file.
Create Database: Create a new PostgreSQL database named crowdfunding_db.
Create Tables: Use the schema to create tables with proper primary and foreign keys.
Import Data: Load each CSV file into its respective table.
Verify Data: Run SELECT * statements to ensure data is correctly imported.
