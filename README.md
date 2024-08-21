# Leveraging-the-Factory-Pattern-and-Data-Lake-Integration-by-SPARK-on-Databricks
This repository showcases an advanced data engineering project using Apache Spark on Databricks. The project focuses on implementing the Factory pattern for building a modular and scalable ETL pipeline. It also demonstrates best practices for integrating and optimizing data workflows within a Data Lake environment. Through this project, we explore Spark's capabilities to process, transform, and analyze large datasets, providing actionable insights into customer behaviors, specifically within the context of Apple product sales.


### File List  

### apple_analysis.ipynb:
- Implements an ETL pipeline to analyze customer behavior, focusing on those who bought AirPods shortly after purchasing an iPhone. 

### loader_factory.ipynb:
- Defines an abstract class DataSink and its implementation LoadToDBFS for loading data into storage systems like DBFS.
### extractor.ipynb:
- Contains the Extractor class and AirpodsAfterIphoneExtractor for extracting transaction data from sources like CSV files.
###loader.ipynb:
- Defines loaders (AbstractLoader, AirPodsAfterIphoneLoader) for saving transformed data, particularly related to AirPods and iPhones, into a target storage location.
### reader_factory.ipynb:
- Implements data source readers (CSVDataSource, ORCDataSource, DeltaDataSource) for ingesting data in different formats into Spark DataFrames.
### transform.ipynb:
- Provides transformation logic (AirpodsAfterIphoneTransformer, OnlyAirpodsAndIphone) to filter and analyze transaction data, focusing on customers who bought AirPods after purchasing an iPhone.
