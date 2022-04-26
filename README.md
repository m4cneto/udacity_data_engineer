# Data Modeling Project with Postgres Udacity - Data Engineer

The objective of the project was to create a whole data pipeline, from extraction, etl and ingestion of data into tables using sql and python in jupyter notebook.

5 tables, 1 fact and 4 dimensions were created, namely:

Fact table:

songplay 
(songplay_id, start_time, user_id, level, song_id, artist_id, session_id, location, user_agent)

Dimension tables: 

users
(user_id, first_name, last_name, gender, level)

song
(song_id, title, artist_id, year, duration)

artist
(artist_id, name, location, latitude, longitude)

time
(start_time, hour, day, week, month, year, weekday)


The project workspace consists of 6 files:
• create_tables.py: Used to DROP AND CREATE tables, it is executed every time the ETL script is executed.
• etl.ipynb: Reading and processing a single song_data and log_data file, and loading the data into the tables, this file has detailed ETL instructions for each table.
• etl.py: Reads and loads the song_data and log_data files and loads the tables. It is populated based on the etl.ipynb block.
• READMY.md: Contains project details.
• sql_queries.py: Contains all SQL queries and is important for create_tables.py, etl.ipynb and etl.py files.
• test.ipynb: Display the first rows of each table to check how the database is doing.


## How to run the script?

• Open a terminal in Jupyter, run your Python scripts in the terminal like you would in your local terminal.
• Execute etl.ipynb for detailed ETL process. 
• Execute test.ipynb where applicable and do remember to restart kernel as per instruction in test.ipynb notebook.
• Execute etl.py for ingest the data from log and song on tables.