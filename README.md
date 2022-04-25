# Movies-ETL(Extract Transform Load)

## Overview 
This project is for Amazing Prime which creates an automated pipeline that takes in new data, performs the appropriate transformations, and load the data into existing tables. It refactor the code from the module to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data—and performs the ETL process by adding the data to a PostgreSQL database.This project extracts a large data set from Kaggle, then transforms the data into a usable dataset for a "hacking competition." Once the data is transformed and usable for the hack-a-thon, the DataFrames are loaded into PostgresSQL.

## Process Involved
1. Create an ETL pipeline from raw data to a SQL database.
2. Extract data from disparate sources using Python.
3. Clean and transform data using Pandas.
4. Use regular expressions (Regex) to parse data and to transform text into numbers.
5. Load data with PostgreSQL and verify in PgAdmin.

## Data Extraction 
- Using your knowledge of Python, Pandas, the ETL process, and code refactoring, function is created that reads in the three data files Wikipedia JSON file,Kaggle metadata and MovieLens ratings data and creates three separate  DataFrames in ETL_function_test.ipynb as displayed below. <br>
 1. The wiki_movies_df DataFrame <br>
   ![WikiMovieDF](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/WikiMovieDF.PNG)<br><br>
 2. The kaggle_metadata DataFrame <br>
   ![Kaggle_metadataDF](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/kaggle_metadataDF.PNG)<br><br>
 3. The ratings DataFrame <br>
 4. ![Ratings](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/ratings.PNG)<br><br>



 
