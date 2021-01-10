# Sparkify a Case Study of Data Modeling with Postgres

## Summary

This is project is intended to help Sparkify music startup to build a database in postgres to query their data. Until now their dataresides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

The code in this repo are ETLs to load songplays, users, songs, artists and time tables into a database in Postgres.

## Instructions

1. Load the song and log data into each of the folders in data.
2. Run `creates_tables.py` to drop all existing tables in the sparkify database, and create new ones.
3. Run `etl.py` to extract, transform and load into sparkify database the songplays, users, songs, artists and time tables from song and log json files.
4. Run `test.ipynb` to verify that etl ran successfully.

## Repo structure

* `data`: Contains the song data and log data, which are json files. 
* `creates_tables.py`: Drops and creates tables in Postgre sparkify databse.
* `etl.ipynb`: Notebook with all the prototype code to build the ETL process.
* `etl.py`: Runs the ETLs to load data into sparkify databse. It creates the following tables:
    - songplays
    - users
    - songs
    - artists
    - time
* `sql_queries.py`: Script with all the drop, create and insert SQL commands.
* `test.ipynb`: Script that tests the existence and content of each of the tables in the database.
