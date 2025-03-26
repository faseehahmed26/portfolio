--- 
title: "KafkaSpark: Containerized User Data Processing Engine"
description: "Multi-container distributed system with Airflow, Kafka, Spark, and Cassandra"
dateString: "Jan 2025 - Mar 2025"
draft: false
tags: ["Data Engineering", "Apache Airflow", "Apache Kafka", "Apache Spark", "Cassandra", "Docker", "ETL", "PostgreSQL", "Python", "Distributed Systems", "Data Streaming", "Real-time Processing"]
showToc: false
weight: 90
cover:
   image: "projects/KafkaSpark/cover.png"
---


### 🔗 [GitHub](https://github.com/faseehahmed26/kafkaspark-processing-engine)

## Description

* Architected and implemented a comprehensive end-to-end data engineering pipeline that connects multiple distributed systems to ingest, process, and store data in real-time.

* Designed a containerized environment using Docker Compose to orchestrate eight different services including Apache Airflow, Apache Kafka, Apache Spark, and Cassandra, ensuring seamless communication between components.

* Developed a scheduled data extraction workflow using Apache Airflow to fetch random user data from external APIs, enabling consistent and reliable data ingestion.

* Implemented a robust streaming architecture with Apache Kafka and Zookeeper that handles the continuous flow of data between services while maintaining data integrity.

* Built a real-time processing layer using Apache Spark with master-worker architecture that transforms and enriches the streaming data before storage.

* Created a scalable and fault-tolerant data storage solution with Cassandra, structuring the database schema to optimize for the specific query patterns of the application.

* Engineered custom connectors between Kafka and Spark using the Spark Streaming API to ensure smooth data transition between the messaging system and processing engine.

* Configured a PostgreSQL backend for Apache Airflow to maintain workflow state, execution history, and configurations, enhancing the reliability of the scheduled jobs.

* Developed a modular and maintainable Python codebase that connects all components, handling errors gracefully and providing detailed logging throughout the pipeline.

* Implemented a monitoring solution for the pipeline using Kafka Control Center, enabling visual tracking of data throughput, bottlenecks, and system performance.

![](/projects/data-engineering-pipeline/architecture.png#center)

## Technical Architecture

The system consists of several key components working together:

1. **Data Ingestion Layer**: Apache Airflow DAGs schedule and execute API calls to fetch random user data
2. **Messaging Layer**: Apache Kafka and Zookeeper process and queue the ingested data
3. **Processing Layer**: Apache Spark performs transformations on the streaming data
4. **Storage Layer**: Cassandra database stores the processed data for analytical queries

All components run in isolated Docker containers, communicating through a dedicated network. This architecture enables horizontal scaling of each component independently, providing flexibility and resilience to the overall system.

## Key Learnings

Building this pipeline provided deep insights into:

* Designing distributed systems that maintain consistency across multiple components
* Handling real-time data streams with exactly-once processing guarantees
* Containerizing complex applications with proper networking and resource allocation
* Implementing fault-tolerance in each layer of the data pipeline
* Optimizing data flow to minimize latency and maximize throughput