# Crowdfunding_ETL

## Project Contributors:
  Bharti Sharma
  Aisha Henderson 

## Tools used for this Project:
  VS Code
  pgAdmin 4
  QuickDBD.com

## References:
UTA Gitlab Files: https://git.bootcampcontent.com/University-of-Texas-at-Austin/UTA-VIRT-DATA-PT-04-2023-U-LOLC
Class TAs: Trisha Mallya and Nathan Darter

## Project Description:

The purpose of this mini project was to Extract data from a source (which was Excel in this instance), Transform and clean the data into DataFrames, and Load the data into a database through CSV files. This involved building an ETL pipeline using Python, and Pandas to extract and transform the data. After we transformed the data, we created four CSV files and used the CSV file data to create an ERD and a table schema. Finally, we uploaded the CSV file data into a Postgres database. 

## Project Details:

This mini project is divided into the following subsections:

Step 1: Creating Category and Subcategory DataFrames
Step 2: Creating a Campaign DataFrame
Step 3: Creating a Contacts DataFrame
Step 4: Creating a Crowdfunding Database

### Step 1
A. Extracted and transformed Excel data to create a Crowdfunding DataFrame.

B. Created Category and Subcategory columns and placed unique values in separate lists. 

C. Created 2 separate DataFrames for Category and Subcategory

D. Exported the Category DataFrame as category.csv

E. Exported the Subcategory DataFrame as subcategory.csv

<img width="953" alt="image" src="https://github.com/AishHen/Crowdfunding_ETL/assets/131278014/9c5d49cb-b255-4205-adbd-92c498f866f0">
<img width="464" alt="image" src="https://github.com/AishHen/Crowdfunding_ETL/assets/131278014/3c6141e5-e1d3-4d2e-b12a-f59ffc44ac17">
<img width="560" alt="image" src="https://github.com/AishHen/Crowdfunding_ETL/assets/131278014/be600779-9fc9-4954-a658-6056531e0238">



### Step 2
A. Extracted and transformed Excel data to create a Campaign DataFrame (campaign_df)

B. Renamed and changed the Data types for "goal" and "pledged" columns 

C. Renamed and changed the Data types to Datetime for "launched_date", and "end_date" columns 

D. Merged the Campaign DF with Category and Subcategory DataFrames

E. Dropped unwanted columns and saved the cleaned DataFrame as campaign.csv

![image](https://github.com/AishHen/Crowdfunding_ETL/assets/131278014/f1b6c424-f58c-4297-a2c4-406947dcc8b0)


### Step 3
A. Iterated through the Contacts DataFrame and converted each row to a Python dictionary

B. Appended the keys and list values to a list named dict_values, and printed the dict_values list

C. Created a DataFrame from the dict_values list

D. Re-ordered the columns and saved it as Contacts.csv

![image](https://github.com/AishHen/Crowdfunding_ETL/assets/131278014/c3b6307b-dd9d-481d-a725-238abfc19edd)


### Step 4
A. Used QuickDBD to create an ERD diagram for the 4 CSV files that were saved in the previous steps.

B. Imported file to Postgres and ran queries to create each table

C. Inserted values to each table by importing each CSV file

D. Saved tables and data as SQL file
  
<img width="953" alt="image" src="https://github.com/AishHen/Crowdfunding_ETL/assets/131278014/2a4be4b1-b642-4956-98be-7ab2986f50bb">
