# Patient Readmission Dashboard with Databricks

![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

A comprehensive analytics project for analyzing diabetic patient readmission patterns using Databricks.

## Overview

This project provides data analysis and visualization tools to understand factors influencing hospital readmission rates for diabetic patients. The insights help healthcare providers identify high-risk patients and implement targeted intervention strategies.

## Medallion Architecture

This project follows the **Medallion Architecture** pattern, a best practice for organizing data in a lakehouse:

### 🥉 Bronze Layer (Raw Data)
* Ingests raw healthcare data from source systems (EHR, hospital management systems)
* Preserves original data format and structure
* Includes patient demographics, admission records, diagnosis codes, and medication history
* Provides data lineage and audit trail for compliance

### 🥈 Silver Layer (Cleaned & Validated)
* Cleanses and standardizes data from the Bronze layer
* Handles missing values, outliers, and data quality issues
* Enriches patient records with derived features (age groups, comorbidity scores, length of stay calculations)
* Applies business rules and validation logic
* Creates fact and dimension tables for analytics

### 🥇 Gold Layer (Business-Level Aggregates)
* Produces curated datasets optimized for analytics and reporting
* Aggregates readmission metrics by patient cohorts, departments, and time periods
* Powers the Lakeview dashboard with pre-calculated KPIs
* Supports machine learning feature stores for predictive models
* Enables self-service analytics for healthcare stakeholders

### Benefits for Healthcare Analytics
* **Data Quality**: Progressive refinement ensures high-quality analytics
* **Scalability**: Handles growing patient data volumes efficiently
* **Governance**: Clear data lineage from source to insights
* **Performance**: Optimized Gold layer tables enable fast dashboard queries
* **Flexibility**: Analysts can query any layer based on their needs

## Contents

* **Diabetic Patient Readmission Analysis.ipynb** - Jupyter notebook containing data exploration, feature engineering, and predictive modeling for patient readmission analysis
* **Diabetic Patient Readmission Analysis Dashboard.lvdash.json** - Interactive Lakeview dashboard visualizing key metrics and trends in patient readmissions

## Key Features

* Patient demographic analysis
* Readmission rate trends and patterns
* Risk factor identification
* Predictive analytics for readmission likelihood
* Interactive visualizations for stakeholder reporting

## Getting Started

1. Open the notebook to explore the data analysis and modeling approach
2. View the dashboard for executive-level insights and KPIs
3. Customize queries and visualizations based on your healthcare data

## Technology Stack

* **Databricks** - Unified analytics platform
* **Apache Spark** - Distributed data processing
* **Python** - Data analysis and modeling
* **SQL** - Data querying and transformation
* **Lakeview Dashboards** - Interactive visualization

## Use Cases

* Healthcare quality improvement initiatives
* Population health management
* Care coordination optimization
* Resource allocation planning
* Compliance reporting

## Contributing

To contribute to this project:
1. Create a feature branch
2. Make your changes
3. Test thoroughly
4. Submit a pull request with a detailed description


