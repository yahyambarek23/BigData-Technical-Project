# 01_Spark_Data_Cleaning.ipynb

## Overview
This notebook implements a comprehensive data cleaning and preprocessing pipeline using Apache Spark for an e-commerce supply chain dataset from Kaggle. It serves as the first stage in a big data analytics pipeline, transforming raw data into a clean, analysis-ready format optimized for downstream machine learning and analytics tasks.

## Purpose
The notebook performs end-to-end data preparation including ingestion, quality assessment, cleaning, and feature engineering on supply chain data to enable delivery risk analytics and operational insights.

## Key Features

### 1. **Environment Setup**
- PySpark 3.4.1 installation and configuration
- Spark session initialization with optimized memory settings (4GB driver/executor memory)
- Adaptive query execution enabled for performance optimization
- 200 shuffle partitions for distributed processing

### 2. **Data Ingestion**
- Interactive file upload widget for Google Colab
- Automatic schema inference
- Support for CSV data format
- Initial data structure exploration and profiling

### 3. **Exploratory Data Analysis (EDA)**
- Comprehensive dataset statistics and summary metrics
- Missing value detection and quantification
- Data type validation
- Duplicate record identification
- Distribution analysis for numerical and categorical features
- Visualization support using Matplotlib and Seaborn

### 4. **Data Cleaning Operations**
- **Duplicate Removal**: Identifies and eliminates duplicate records
- **Date Standardization**: Converts string dates to proper date/timestamp formats
- **Missing Value Handling**: Implements strategies for null value treatment
- **Data Type Corrections**: Ensures proper schema alignment
- **Text Normalization**: Standardizes string fields (trimming, case conversion)
- **Data Quality Validation**: Post-cleaning verification checks

### 5. **Feature Engineering**
- Temporal feature extraction (year, month, day, day of week)
- Date difference calculations
- Aggregation features (counts, statistics by customer/product)
- Categorical encoding preparations
- Derived business metrics

### 6. **Output & Persistence**
- **Parquet Format**: Columnar storage optimized for Spark operations
- **CSV Format**: Single-file export for compatibility
- **Google Drive Integration**: Automated backup to cloud storage
- Data verification and quality checks on saved outputs

## Technical Stack
- **Apache Spark 3.4.1**: Distributed data processing engine
- **PySpark**: Python API for Spark
- **pandas**: Supplementary data manipulation
- **Matplotlib & Seaborn**: Data visualization
- **Google Colab**: Development environment

## Spark Configuration
```python
- Driver Memory: 4GB
- Executor Memory: 4GB
- Shuffle Partitions: 200
- Adaptive Query Execution: Enabled
- Coalesce Partitions: Enabled
- Execution Mode: Local[*] (all available cores)
```

## Output Files
- `cleaned_data.parquet` - Optimized columnar format for Spark
- `cleaned_data.csv` - Single CSV file for broad compatibility
- Automatic backup to Google Drive at `/MyDrive/BigDataProject/`
  ### Note: (You can access this drive folder through the link available in the file Dataset details.md in the repo)

## Data Quality Metrics Tracked
- Row count before/after cleaning
- Missing value percentages per column
- Duplicate record counts
- Data type consistency
- Date field validity
- Statistical distributions

## Next Steps in Pipeline
This cleaned dataset serves as input for:
- Storage phase
- Data augmentationMachine learning model training
- SQL analytics and reporting
- Dashboard and visualization tools

## Dependencies
```
pyspark==3.4.1
matplotlib
seaborn
pandas

