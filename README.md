## Data Modeling with Apache Cassandra


#### Introduction
Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. Their analytics team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data resides in a directory of CSV files on user activity on the app. The goal is to create a database for this analysis.


#### Project Description
In this project, I have created a database in Apache Cassandra and modeled tables optimized to run queries on song play data to answer the questions. I have also written an ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.


#### Datasets

###### Event Data
In this project, we have event data in a directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:\
event_data/2018-11-08-events.csv\
event_data/2018-11-09-events.csv

And below is an example of what event data looks like:
![alt text](https://github.com/rumijha/data-modeling-with-apache-cassandra/blob/main/image_event_datafile_new.jpg)


#### Project Files
The project includes one Jupyter Notebook file, which:
* processes the event_datafile_new.csv dataset to create a denormalized dataset
* models the data tables keeping in mind the queries needed to run (queries have been provided that are needed to model the data tables)
* loads the data into tables in Apache Cassandra and runs the provided queries
