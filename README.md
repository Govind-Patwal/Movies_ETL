# Movies ETL

## Project Overview
Amazing Prime Video is a platform for streaming movies and TV shows on ***Amazing Prime***, the world's largest online retailer. The Amazing Prime video team would like to develop an algorithm which would predict which low-budget movie being released would become popular, so that they can buy the streaming rights at a bargain. 

To inspire the team, have some fun and connect with the coding community, Amazing Prime has decided to sponsor a Hackathon, providing a clean dataset of movie data and asking participants to predict the popularity pictures. 

Britta, a member of the Amazin Prime video team, has been tasked with creating the datasets for the Hackathons. There are two data sources, a scrape of **wikipedia** for all moviese released since 1990, and rating data from **MovieLens** website.
She will need to extract the data from the two sources, transform into one clean dataset and finally load that data into a SQL table.

Britta needs to organize the data from Wikipedia and MovieLens in a structured format before she can send it to SQL—and she's asked me to assist with this task.

## Purpose of this Assignment

Britta and I worked together to Extract-Transform-Load the data from the 2 source to PostgreSQL.

Now, Amazing Prime wants to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. I’ll need to refactor the code that I used to create one function that takes in the three files — Wikipedia data, Kaggle metadata, and the MovieLens rating data — and performs the ETL process by adding the data to a PostgreSQL database.

## Assignment Steps

### Deliverable 1

1. In Step 1, create the function to read in the three files and give it a name.
2. In Step 2, read in the Kaggle metadata and MovieLens ratings CSV files as Pandas DataFrames.
3. In Step 3, open the Wikipedia JSON file and use the json.load() function to convert the JSON data to raw data.
4. In Step 4, read in the raw Wikipedia movie data as a Pandas DataFrame.
5. In Step 5, use the code provided to return the three DataFrames.
6. In Step 6, use the variables provided to create a path to the Wikipedia data, the Kaggle metadata, and the MovieLens rating data files.
7. In Step 7, set the three variables in Step 6 equal to the function created in Step 1.
8. In Step 8, set the DataFrames from the return statement equal to the file names in Step 6. In this step, you are reassigning the variables created in Step 6 to the variables in the return statement.
9. In Steps 9-11, check that all three files are converted to a DataFrame. 

    **Image 1 (below): wiki_movies_df**
    ![wiki_movies_df](./Resources/Deliverable1_wiki_movies_df.png)

    **Image 2 (below): kaggle_metadata**
    ![kaggle_metadata](./Resources/Deliverable1_kaggle_metadata.png)

    **Image 3 (below): ratings**
    ![ratings](./Resources/Deliverable1_ratings.png)




### Deliverable 2

**Image 4 (below): wiki_movies_df**
![wiki_movies_df](./Resources/Deliverable2_wiki_movies_df.png)


**Image 5 (below): wiki_movies_df_columns_to_list.columns.to_list()**
![wiki_movies_df_columns_to_list](./Resources/Deliverable2_wiki_movies_df_columns_to_list.png)





### Deliverable 3

**Image 6 (below): wiki_movies_df**
![wiki_movies_df](./Resources/Deliverable3_wiki_movies_df.png)

**Image 7 (below): movies_with_ratings_df**
![movies_with_ratings_df](./Resources/Deliverable3_movies_with_ratings_df.png)

**Image 8 (below): movies_df**
![movies](./Resources/Deliverable3_movies_df.png)




### Deliverable 4

**Image 9 (below): Loading ratings to PostgresSQL**

![Loading ratings to PostgresSQL](./Resources/Deliverable4_loading_ratings_to_SQL.PNG)


**Image 10 (below): movies queries**

![Loading ratings to PostgresSQL](./Resources/movies_query.png)

**Image 11 (below): ratings queries**

![Loading ratings to PostgresSQL](./Resources/ratings_query.png)