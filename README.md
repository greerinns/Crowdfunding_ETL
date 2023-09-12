# Crowdfunding_ETL

## Project Overview
Crowdfunding_ETL involves the Extraction, Transformation, and Loading (ETL) of data from Excel files into a PostgreSQL database.

## Subsection 1: Category and Subcategory DataFrames

In the initial subsection, we focus on creating the Category and Subcategory DataFrames. We extract and transform data from the "crowdfunding.xlsx" Excel file to construct a Category DataFrame. This DataFrame contains two critical columns: "category_id" and "category," where "category_id" represents unique category identifiers ("cat1" to "catn") and "category" denotes the corresponding category titles. A similar process is applied to construct the Subcategory DataFrame, which contains "subcategory_id" and "subcategory" columns. Both DataFrames are thoughtfully structured and are subsequently exported as CSV files.

![Category DataFrame](https://github.com/estellesantini/Crowdfunding_ETL/assets/47437697/f1b6c09a-4fc2-4d69-baf2-4ce1a7453720)

![Subcategory DataFrame](https://github.com/estellesantini/Crowdfunding_ETL/assets/47437697/ee46ca91-89f6-4a86-9c03-289f1f3e70d4)

## Subsection 2: Campaign DataFrame

The subsequent task revolves around the creation of the Campaign DataFrame. We extract and transform data from the "crowdfunding.xlsx" file to construct this comprehensive DataFrame. It encompasses multiple columns, including "cf_id," "contact_id," "company_name," "description," "goal," "pledged," "outcome," "backers_count," "country," "currency," "launch_date," "end_date," "category_id," and "subcategory_id." Several data type conversions and renaming operations are conducted to ensure the data's integrity and consistency. Additionally, the "launch_date" and "end_date" columns are transformed into datetime format. The Campaign DataFrame is meticulously organized and is subsequently exported as a CSV file, readily available in the GitHub repository.

![Campaign DataFrame](https://github.com/estellesantini/Crowdfunding_ETL/assets/47437697/e8b248f3-4967-4535-a86a-c482d743d1c5)

![Campaign DataFrame](https://github.com/estellesantini/Crowdfunding_ETL/assets/47437697/3c2efa71-c375-41ce-b8af-ef9033b1a3ea)

## Subsection 3: Contacts DataFrame

In this subsection, our focus shifts towards the creation of the Contacts DataFrame. We present two options for extracting and transforming data from the "contacts.xlsx" Excel file. The chosen method involves converting each row into a dictionary, thereby facilitating data manipulation. We import the "contacts.xlsx" file into a DataFrame, extract the row data into dictionaries, and subsequently consolidate these dictionaries into a new DataFrame. The "name" column is thoughtfully split into separate columns for first and last names. The resultant Contacts DataFrame is thoroughly cleaned and exported as a CSV file, readily accessible in the GitHub repository.

![Contacts DataFrame](https://github.com/estellesantini/Crowdfunding_ETL/assets/47437697/fd54c824-a1d4-43d1-9470-f8be5bfd134a)

## Subsection 4: Crowdfunding Database

The final subsection centers around the creation of the Crowdfunding Database. We commence by meticulously examining the provided CSV files and the Entity-Relationship Diagram (ERD). Subsequently, we sketch the table schemas for each CSV file based on the ERD using QuickDBD. The resulting database schema, which includes data types, primary keys, foreign keys, and other constraints, is saved as a PostgreSQL file named "crowdfunding_db_schema.sql" and is stored within the GitHub repository. Following this, we create a new PostgreSQL database named "crowdfunding_db" and construct the tables in accordance with the database schema's foreign key relationships. We validate the table creation by executing SELECT statements for each table, ensuring data integrity. Finally, we import the CSV files into their respective SQL tables and employ SELECT statements to verify the presence of the correct data in each table.

## Conclusion

Crowdfunding_ETL represents a meticulous and systematic effort to extract, transform, and load data from Excel files into a PostgreSQL database. This project reflects the skillful application of data engineering techniques, enabling the seamless transformation of raw data into structured, accessible, and informative datasets.
