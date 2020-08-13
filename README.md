
## Purpose of the database in the context of Sparkify 
This database will make it easier to understand information regarding what songs are being played the most, who is playing them, where they are 
being played from and so on. This information can help the company know their end user and their likes and dislikes more. 

## Database schema design and ETL pipeline 
We have used a star schema optimized for queires on song play analysis. 
Data is extracted from json files containing song and app_events data.
Songplay events are filtered, and loaded into songplays table with relevant song and artist information. 
The event json files are read in chronological order so that the user's latest level (paid/free) is always updated in db. 

## How to run 
1. Run the create_tables.py script
2. Run the etl.py script

## Files 
data folder : has json song and event data
create_tables.py : creates database, and initiailizes new DB creation
etl.py : extraction of data from json files, transformation into desired structure, loading into database
sql_queries.py : All the sql commands for create, drop, insertion, selection and deletion of data. 



