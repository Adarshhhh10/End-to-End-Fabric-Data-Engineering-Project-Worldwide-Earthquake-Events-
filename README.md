🌍 Worldwide Earthquake Events – End-to-End Data Engineering Project (Microsoft Fabric)
📌 Project Overview

This project demonstrates an end-to-end data engineering solution built using Microsoft Fabric, following the Medallion Architecture (Bronze → Silver → Gold) to ingest, process, model, and visualize Worldwide Earthquake Events data.

The solution covers data ingestion from an external API, data transformation using notebooks, orchestration with Fabric pipelines, semantic modeling, and interactive reporting using Power BI.

This project is designed for Data Engineer / Data Engineering Intern roles.

🏗️ Architecture Overview

Tools & Technologies Used:

Microsoft Fabric

Fabric Notebooks (PySpark)

Fabric Pipelines

OneLake (Lakehouse)

Fabric Warehouse

Semantic Model

Power BI

REST API (Worldwide Earthquake Events)

Architecture Pattern:

Medallion Architecture

Bronze → Raw ingestion

Silver → Cleaned & transformed

Gold → Business-ready aggregates

📂 Project Structure
Worldwide-Earthquake-Events/
│
├── notebooks/
│   ├── 01 Worldwide Earthquake Events API - Bronze.ipynb
│   ├── 02 Worldwide Earthquake Events API - Silver.ipynb
│   └── 03 Worldwide Earthquake Events API - Gold.ipynb
│
├── pipelines/
│   ├── earthquake_data_pipeline.png
│
├── lakehouse/
│   └── Worldwide_Earthquake_Events
│
├── warehouse/
│   └── Worldwide_Earthquake_Events.sql
│
├── semantic_model/
│   └── Earthquake_Events_Semantic_Model.png
│
├── reports/
│   └── Worldwide_Earthquake_Events.pbix
│
└── README.md

🔄 Data Pipeline Flow

Source

Worldwide Earthquake Events REST API

Bronze Layer

Raw JSON data ingestion

Schema-on-read storage in Lakehouse

Silver Layer

Data cleansing and normalization

Timestamp parsing and data type corrections

Removal of invalid or null records

Gold Layer

Aggregated and analytics-ready datasets

Stored in Fabric Warehouse for reporting

📘 Notebooks Description

01 – Bronze Notebook

Fetches data from the Earthquake API

Stores raw data in Bronze layer (Lakehouse)

02 – Silver Notebook

Cleans and transforms raw data

Applies schema standardization

Writes curated data to Silver layer

03 – Gold Notebook

Creates business-ready aggregates

Optimized for reporting and analytics

🧩 Orchestration

Fabric Pipeline

Orchestrates Bronze → Silver → Gold execution

Ensures dependency-based execution

Enables scheduled and automated runs

🗄️ Storage & Modeling

Lakehouse

Central storage using OneLake

Stores Bronze and Silver datasets

Warehouse

Stores Gold layer tables

Optimized for SQL analytics

Semantic Model

Business-friendly data model

Measures and relationships defined for reporting

📊 Reporting

Power BI Report

Interactive dashboards

Visual insights on:

Earthquake frequency

Magnitude distribution

Location-based analysis

Time-based trends
