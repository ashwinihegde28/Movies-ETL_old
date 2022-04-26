# Movies-ETL(Extract Transform Load)

## Overview 
This project is for Amazing Prime which creates an automated pipeline that takes in new data, performs the appropriate transformations, and load the data into existing tables. It refactors the code from the module to create a function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data and performs the ETL process by adding the data to a PostgreSQL database.This project extracts a large data set from Kaggle, then transforms the data into a usable dataset for a "hacking competition." Once the data is transformed and usable for the hack-a-thon, the DataFrames are loaded into PostgresSQL.

## Process Involved
1. Create an ETL pipeline from raw data to a SQL database.
2. Extract data from disparate sources using Python.
3. Clean and transform data using Pandas.
4. Use regular expressions (Regex) to parse data and to transform text into numbers.
5. Load data with PostgreSQL and verify in PgAdmin.

## ETL Function to Read Three Data Files
- Using the knowledge of Python, Pandas, the ETL process, and code refactoring, function is created that reads in the three data files Wikipedia JSON file,Kaggle metadata and MovieLens ratings data and creates three separate  DataFrames in ETL_function_test.ipynb as displayed below. <br>
 1. The wiki_movies_df DataFrame <br>
   ![WikiMovieDF](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/WikiMovieDF.PNG)<br><br>
 2. The kaggle_metadata DataFrame <br>
   ![Kaggle_metadataDF](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/kaggle_metadataDF.PNG)<br><br>
 3. The ratings DataFrame <br>
   ![Ratings](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/ratings.PNG)<br><br>

## Extraction and Transforming Wiki movie data
- Using the knowledge of Python, Pandas, the ETL process, and code refactoring, extracting and transforming the Wikipedia data and merge it with the Kaggle metadata.  While extracting the IMDb IDs using a regular expression string and dropping duplicates, used a try-except block to catch errors and parsed the data.The cleaned Wikipedia data is converted to a Pandas DataFrame, and the DataFrame is displayed in the ETL_clean_wiki_movies.ipynb file. <br>
1. Clean wiki_movies_df <br>
   ![WikiMovieDF](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/cleanWikiDF.PNG)<br><br>
   
2. Clean wiki_movies_df columns <br>
   ![WikiMovieDF columns](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/cleanWikiColumnList.PNG)<br><br> 
   
## Extract and Transform the Kaggle Data
- Using the knowledge of Python, Pandas, the ETL process, and code refactoring, extracting and transforming the Kaggle metadata and MovieLens rating data, then converting the transformed data into separate DataFrames. Next merging the Kaggle metadata DataFrame with the Wikipedia movies DataFrame to create the movies_df DataFrame. Finally, merging the MovieLens rating data DataFrame with the movies_df DataFrame to create the movies_with_ratings_df as displayed below. <br>
1. Movies_with_ratings_df DataFrame. <br>
  ![Movie With Ratings](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/movieWithRatings.PNG)<br><br>
2. movies_df DataFrame <br>
 ![MovieDF](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/Deliverable2.PNG)<br><br>
 
 ## Create the Movie Database
 - Added the movies_df DataFrame and MovieLens rating CSV data to a SQL database. Please find the images below. <br>
 1. movies_query.png <br>
   ![movies_query.png](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/movies_query.png)<br><br>
 2. ratings_query.png <br>
   ![Ratings](https://github.com/ashwinihegde28/Movies-ETL/blob/main/Resources/ratings_query.PNG)<br><br>
   
   
 ## Summary
 The ETL Extract, Transform, Load) function created collects and cleans movie data from different sources (Wikipedia JSON and Kaggle and ratings CSV files). It transforms and merges the data and loads it into two updatable PostgreSQL dataset tables ready to be used by the hackathon participants for their analysis.
 

   




 
