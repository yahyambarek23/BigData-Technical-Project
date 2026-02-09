# Big Data Pipeline for Customer Segmentation and Supply Chain Analytics in E-Commerce 

Big Data Analytics project developed at Tunis Business School (2025/2026).

## Objective
Build an end-to-end big data pipeline to clean, transform, augment and analyze e-commerce transactions, and apply machine learning to discover customer segments and delivery risks.

## Architecture
Raw Data → Cleaning → Feature Engineering → Augmentation (10M+) → Spark SQL Analytics → ML Clustering → Power BI Dashboard.

## Technologies Used
- Apache Spark (PySpark)
- Spark SQL
- Spark MLlib (K-Means, PCA)
- Google Colab
- Google Drive
- Power BI

## Dataset
- Source: Kaggle e-commerce dataset
- Original size: 108K records
- After augmentation: 10M+ records
- Storage format: Parquet

## Repository Structure
- ingestion → data loading
- eda → exploration & quality analysis
- cleaning → preparation & validation
- feature_engineering → derived business metrics
- augmentation → big data simulation
- analytics_sql → SQL insights
- ml → clustering & PCA
- dashboards → BI results
- performance → partitioning & caching tests

## How to Reproduce
Install libraries:
pip install -r requirements.txt

Run pipeline in this order:
1. ingestion
2. cleaning
3. feature engineering
4. augmentation
5. analytics / ML

## Authors
- Ibtihel Jlassi  
- Nouha Hajji  
- Yahya Mbarek

Instructor: Dr. Manel Abdelkader
