## Data Modelling with Cassandra

### Project Overview

This project builds a data model using Apache Cassandra for Sparkify, a music streaming startup, to support analytical queries on song play activity.

Sparkify collects user activity and song data in a directory of CSV files, but the data is not structured in a way that supports efficient analysis. The goal of this project is to design a NoSQL data model and build an ETL pipeline in Python that transforms raw event data into query-optimized tables in Apache Cassandra.

Using Apache Cassandra’s query-first design approach, this project models data based on specific business questions provided by Sparkify’s analytics team, including:

- What songs were played during a given session?
- What song did a specific user listen to during a session?
- Who listened to a particular song?

### Objectives

This project focuses on:

- Designing Apache Cassandra tables around query patterns
- Creating an ETL pipeline in Python to process event data
- Loading transformed data into Cassandra tables
- Running analytical queries against the modeled data
- Applying partition key and primary key design principles for efficient retrieval


### Technologies Used

- Python
- Apache Cassandra
- CQL (Cassandra Query Language)
- CSV
- Jupyter Notebook


### ETL Pipeline Workflow

The pipeline performs the following steps:

1. Reads raw event CSV files from a directory  
2. Combines them into a consolidated event dataset  
3. Creates query-specific Cassandra tables  
4. Inserts records into Cassandra  
5. Executes analytical queries to validate results
