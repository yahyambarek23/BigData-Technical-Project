# Data Preparation Pipeline

This notebook contains the first stage of the project and prepares the foundation for all later steps.

## What is done here
- Data ingestion from the original CSV dataset
- Exploratory Data Analysis (missing values, duplicates, distributions)
- Data cleaning and validation
- Date standardization
- Privacy-related column removal
- Feature engineering (shipping, RFM, financial, discount, segmentation)

## Input
Raw Kaggle e-commerce dataset.

## Output
Clean and feature-enriched dataset used by:
- storage phase
- data augmentation
- SQL analytics
- machine learning
