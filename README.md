# Movies-ETL

# Background

The dataset has to updated on a daily basis. To create an automated pipeline process ETL,  that takes in new data, performs the appropriate transformations, and loads the data into existing tables to maintain its integrity. The ability to perform data analysis without the use of ETL is extremely limited.

# Overview of the project

 The Amazing Prime, a video streaming company,loves the dataset and wants to keep it updated on a daily basis. It has decided to sponsor a hackathon, where participants trying to predict which low budget movies being released will become popular. Participants of a hackathon need a performs the appropriate transformations, and loads the data into existing tables. The goal of this project is to create an ETL pipeline that can be refactored to process large datasets into a PostgreSQL database, which includes the following,

* Write an ETL Function to Read Three Data Files
* Extract and Transform the Wikipedia Data
* Extract and Transform the Kaggle data
* Create the Movie Database

# Analysis
## Write an ETL Function to Read Three Data Files
   
Read in the Kaggle metadata and MovieLens ratings CSV files as Pandas DataFrames.

Open the Wikipedia JSON file and use the json.load() function to convert the JSON data to raw data and read as a Pandas DataFrame.

## Extract and Transform the Wikipedia Data   

Transform the Wikipedia Data takes the Wiki dataframe and clean the data using functions clean_movie, subfunction change_column_name, extract_transform_load, parse_dollar. Use the list comprehensions, lambda functions and RegEx in the process.

## Extract and Transform the Kaggle data
Reads in the three data files and creates the kaggle metadata and ratings DataFrames.

Take the kaggle dataframe as input and transform the data. 
    
Merge the wiki movies dataFrame and the kaggle metadata dataFrames with ratings data.

##  Create the Movie Database
    
A connection to the database was established in the Python environment using sqlalchemy library and to_sql method and the final dataset was loaded into two SQL tables, 
* movies
* ratings

 # Results 

**movies** table query and the output is as below,

   ![Movies Query](Resources/movies_query.png?raw=true)   

**ratings** table query and the output is as below,

   ![Ratings Query](Resources/ratings_query.png?raw=true)   
    