# Datalake-real-time-streaming-pipeline-in-AWS

![Final Project](https://user-images.githubusercontent.com/88790752/160277457-9128def6-4994-4b9c-9ada-9fc69db3b1eb.jpeg)

Streaming ETL pipeline project is based on Toronto Transit Committion Bus API vehicle tracking data. The pipeline is a real time event based data streaming process including on fly data transformation using a set of current AWS services.

-- Data ingestion and dataframe is done in Apache Nifi project
-- Ingested dataframe is collected in MySQL server and bridged with Kafka Debezium spinned in Docker container
-- Kafka(MSK) preconfigured topics are used for a data transition to Spark
-- Spark Streaming job SBT project in the .jar file is responsible for data transformation into parquet format using Hudi
-- Generated parquet data is stored in S3 bucket
-- TTC Bus real time data analysis is done in Superset

_________________________________________________________________________________________________________________________________________________________________

Live chart examples

![Chart 1](https://user-images.githubusercontent.com/88790752/160277510-3357d164-034e-444a-8299-4598f8ade00e.jpg)

![Chart 2](https://user-images.githubusercontent.com/88790752/160277517-d28ec00d-2aea-4918-b227-55959bbf7b69.jpg)
