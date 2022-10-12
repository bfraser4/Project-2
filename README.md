# Project 2 ETL

## Group Members: 
- Jeff Brown
- Brittanie Fraser
- Andreas Heger
- Xilonem Montoya 
- Vandan Patel 

## Data Sources: 
    1) https://www.kaggle.com/datasets/shivamb/netflix-shows
    2) https://www.kaggle.com/datasets/ramjasmaurya/top-250s-in-imdb

## Proposal 

We will analyz data from Netflix streaming services and IMDB data set. We will join the data set by the title, Movie Rating, votes, date added, and rating. Lastly, we will analyze and complete the extract, transform and load (ETL) process on the data set.


Extract: Extracting Disney+ and Netflix CSV file from data from Kaggle.com 

Transform: Cleaning data, filtering, joining, aggregating 

Load: PgAdmin

Responsibilities: 

- Extract, data discovery: All team
- Transform, Pandas: Andreas + team
- Load, PostgreSQL: Jeff + team
- Data Mapping: Brittanie + Xilonem
- Git Hub repository set up & maintenance: Brittanie 

## ETL Process:

- Extract: indicates the original data sources and how the data were formatted at a professional level

We imported each CSV file into pandas as a DataFrame. Then, within pandas, the "title" column was aggregated into upper case format, and the "rating" column was formatted to lower case in the final DataFrame.   

- Transform: explains what data clearing or transformation was required at a professional level.

As a team, we removed data that we felt were unnecessary to the data set. In cleaning the data set, we identified multiple columns that can be deleted. Once the data was removed, we began to merge each table. Ultimately we joined all two tables into one. Once all the tables were integrated into a final DataFrame, a Postgres connection was created and added to PgAdmin.

- Load: explains the final database, tables/collections, and why the topic was chosen at a professional level

The Netflix DataFrame was created with the following columns: title, date_added, and rating. In addition, the IMDB DataFrame contained the Movie Name, Movie Rating, and Votes columns. Our final table had both Netflix and IMBD and included the following columns: title, Movie Rating, votes, date_added, and rating. We actively chose this topic as we felt finding movie datasets would be readily available. 

