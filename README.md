# ELT Pipeline with dbt, Snowflake, and Airflow

## Overview
This project demonstrates an **ELT (Extract, Load, Transform) pipeline** using **dbt (Data Build Tool), Snowflake (Cloud Data Warehouse), and Apache Airflow (Workflow Orchestration)**. The pipeline extracts data from a source, loads it into Snowflake, and transforms it using dbt.

## Features
- **Data Extraction**: Extracts data from a raw source.
- **Loading into Snowflake**: Uses Snowflake as the cloud data warehouse.
- **Data Transformation**: Utilizes dbt for transformations.
- **Orchestration with Airflow**: Automates and schedules the pipeline.
- **Modular and Scalable**: Easily adaptable for different datasets and transformations.

## Technologies Used
- **Snowflake**: Cloud-based data warehouse.
- **dbt**: Transformation framework for analytics.
- **Apache Airflow**: Workflow automation and orchestration.
- **Python**: Scripting and automation.
- **Docker** (optional): Containerization for deployment.

## Architecture
```mermaid
graph TD;
    A[Extract Data] -->|Raw Data| B[Load into Snowflake];
    B -->|Transform with dbt| C[Transformed Data];
    C -->|Orchestrate with Airflow| D[Final Processed Data];
