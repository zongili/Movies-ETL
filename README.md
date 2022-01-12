# Extract - Transform - Load (ETL) Movies
## Purpose :
Extract data from Wikipedia and Kaggle, transform and merge using python, pandas, ETL processes, and save them into a PostgreSQL database so that the hackathon participants have a nice, clean dataset to use.

## Analysis: 
 For this project  gathered wikipedia_movies.json from wikipedia site,  movies_metada.csv and ratings.csv from Kaggle.com site. Using Python, Pandas, the ETL process, and code refactoring, written a function that reads in the three data files and creates three separate DataFrames. While extracting the IMDb_IDs using a regular expression string and dropping duplicates, used a try-except block to catch errors. Kaggle metadata and MovieLens rating data, then convert the transformed data into separate DataFrames. Wikipedia data is merged it with the Kaggle metadata to create the movies_df DataFrame. Finally rating data merged with the movies_df DataFrame to create the movies_with_ratings_df. 
Print Elapsed Time is a recommend optional step to do when running a long process. The image below shows the result of the print on the total amount of time elapsed at every step which is useful to estimate how long the process is going to take.

![This image shows the result of the titles vs count ](Resources/ratings_elapsed_time.png)
 
 ## Results:  
Final step in the project is to save the movies and ratings dataframes into SQL database and count the number of rows as shown in the following images. 6052 records for the movies and 26024289 for the ratings table.

![This image shows the result of the titles vs count ](Resources/movies_query.png)

![This image shows the result of the titles vs count ](Resources/ratings_query.png)
