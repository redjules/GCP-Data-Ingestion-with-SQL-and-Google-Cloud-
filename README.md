# GCP Data Ingestion with SQL using Google Cloud Dataflow

# Project Description
The agenda of the project involves Data ingestion and processing pipeline on Google cloud platform with real-time streaming and batch loads. Yelp dataset, which is used for academics and research purposes is used. We first create a service account on GCP followed by downloading Google Cloud SDK(Software developer kit). Then, Python software and all other dependencies are downloaded and connected to the GCP account for further processes. Then, the Yelp dataset is downloaded in JSON format, is connected to Cloud SDK following connections to Cloud storage which is then connected with Cloud Composer and Yelp dataset JSON stream is published to PubSub topic. Cloud composer and PubSub outputs are Apache Beam and connecting to Google Dataflow. Google BigQuery receives the structured data from workers. Finally, the data is passed to Google Data studio for visualization.

# Usage of Dataset:

Here we are going to use Yelp data in JSON format in the following ways:

- Yelp dataset File: In Yelp dataset File, JSON file is connected to Cloud storage Fuse or Cloud SDK to the Google cloud storage which stores the incoming raw data followed by connections to Google Cloud Composer or Airflow to the Google cloud storage for scheduling and orchestration to batch workloads.

- Yelp dataset Stream: In Yelp dataset Stream, JSON Streams are published to Google PubSub topic for real-time data ingestion followed by connections to Apache beam for further processing.

# Data Analysis:

- From the given website, the Yelp dataset is downloaded in JSON format. The Yelp JSON file is connected to Google SDK or GcsFuse for transfer of data to Google cloud storage which is connected to Google Cloud composer/Airflow for scheduling and orchestration of batch workloads.

- Yelp dataset JSON streams are published to Google PubSub which is used for real-time ingestion or streaming datasets.

- Data pipeline is created by apache beam which receives the real-time data from Google PubSub and the data from Google cloud storage as inputs which are followed by creating Google dataflow stream job and batch job scaling the compute based on throughput.

- Apache beam orchestrates stream and batch jobs following the output of Google Dataflow to workers.

- Google BigQuery acts as a Data warehouse storing structured data which receives the input from workers and queries the data.

- Finally data is visualized using different graphs and table definitions in Google Data Studio.
