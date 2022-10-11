# Data Sources: 
    1) https://www.kaggle.com/datasets/shivamb/disney-movies-and-tv-shows
    2) https://www.kaggle.com/datasets/shivamb/netflix-shows
    3) https://www.kaggle.com/datasets/ramjasmaurya/top-250s-in-imdb
    
√ Extract: indicates the original data sources and how the data were formatted at a professional level

We imported each CSV file into pandas as a DataFrame. Then, within pandas, the "title" column was aggregated into upper case format, and the "rating" column was formatted to lower case in the final DataFrame.   

√ Transform: explains what data clearing or transformation was required at a professional level.

As a team, we removed data that we felt were unnecessary to the data set. In cleaning the data set, we identified multiple columns that can be deleted. Once the data was removed, we began to merge each table. Ultimately we joined all three tables into one. Once all the tables were integrated into a final DataFrame, a Postgres connection was created and added to PgAdmin.

√ Load: explains the final database, tables/collections, and why the topic was chosen at a professional level

From the Netflix and Disney+ data set, DataFrames were created with the following columns: title, date_added, and rating. In addition, the IMDB DataFrame contained the Movie Name, Movie Rating, and Votes columns. Our final table had all three DataFrames and included the following columns: title, Movie Rating, votes, date_added, and rating. We actively choose this topic to analyze the top titles of movies/tv shows for Disney+ and Netflix streaming services. 

