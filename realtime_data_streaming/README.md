# Realtime streaming data project | end-to-end-data-engineering-project

## Table of contents
- [Introduction](#introduction)
- [System Architecture](#system-architecture)
- [What You'll Learn](#what-youll-learn)
- [Technologies](#technologies)
- [Getting Started](#getting-started)
- [Watch the Video Tutorial](#watch-the-video-tutorial)

## Introduction

This project servers as a comprehensive guide to building an end-to-end data engneering pipeline. It covers each stage from ingestion to processing and finally to storage, utilizing a robust tech stack that includes Apache Airfow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. Everything is containerized using docker for ease of deployment and scalability.

## System Architecture 

![System Architecture](Data engineering architecture.png)

The project is designed with the following components:

- **Data Source**: We use `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgresSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgresSQL to the processing engine.
- **Control Center and Schema Resgistry**: Helps in monitoring and schema management of out Kafka streams.
- **Apache Spark**: For data processing with its master and worker nodes.
- **Cassandra**: Where the processed data will be stored.


## What you'll learn

- Setting up a data pipeline with Apache Airflow
- Real-time data streaming with Apache kafka
- Distributed synchronization with Apache Zookeeper
- Data processing techniques with Apache Spark
- Data storage solutions with Cassandra and PostgreSQL
- Containerizing your entire data engineering setup with Docker

## Technologies

- Apache Airflow
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker
- Python

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/julianNgo/end-to-end-data-engineering-project.git
    ```

2. Navigate to the project directory:
    ```bash
    cd Realtime Data Streaming
    ```

3. Run Docker Compose to spin up the services:
    ```bash
    docker-compose up
    ```