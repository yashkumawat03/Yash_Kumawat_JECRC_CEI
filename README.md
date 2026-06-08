# Country Segmentation using Unsupervised Machine Learning

## Project Overview

This project focuses on segmenting countries based on socio-economic and health indicators using Unsupervised Machine Learning techniques. The objective is to help HELP International identify countries that require the most financial aid by grouping countries with similar characteristics into clusters.

## Dataset

The dataset contains socio-economic and health-related information for 167 countries, including:

* Country Name
* Child Mortality Rate
* Exports (% of GDP)
* Health Spending (% of GDP)
* Imports (% of GDP)
* Income per Person
* Inflation Rate
* Life Expectancy
* Total Fertility Rate
* GDP per Capita

## Project Workflow

### 1. Data Ingestion and Validation

* Loaded the dataset into a Pandas DataFrame
* Examined dataset structure and data types
* Checked for missing values and duplicate records
* Verified data quality before analysis

### 2. Exploratory Data Analysis (EDA)

* Analyzed feature distributions using histograms
* Identified outliers using boxplots
* Performed correlation analysis using a heatmap
* Explored relationships among socio-economic indicators

### 3. Data Preprocessing

* Removed the country name column from model training
* Standardized numerical features using StandardScaler
* Prepared the data for distance-based clustering algorithms

### 4. Dimensionality Reduction

* Applied Principal Component Analysis (PCA)
* Reduced feature dimensionality while preserving 95% of data variance
* Improved clustering efficiency and visualization

### 5. Cluster Selection

* Applied the Elbow Method to determine an appropriate number of clusters
* Evaluated clustering performance using Silhouette Score
* Selected the optimal number of clusters for K-Means

### 6. K-Means Clustering

* Trained a K-Means clustering model on PCA-transformed data
* Segmented countries into distinct groups based on socio-economic characteristics
* Assigned cluster labels to each country

### 7. Cluster Analysis

* Performed cluster profiling using average feature values
* Analyzed cluster centroids
* Compared feature distributions across clusters
* Identified developed, developing, and underdeveloped country groups

### 8. Aid Prioritization

* Identified the cluster with the lowest income and GDP per capita
* Examined countries with high child mortality and lower life expectancy
* Generated a list of countries that should be prioritized for financial aid

### 9. Model Persistence

* Saved preprocessing and clustering components using Joblib
* Stored:

  * StandardScaler
  * PCA Transformer
  * K-Means Model

### 10. Inference Pipeline

* Created a reusable prediction function
* Enabled cluster prediction for new country-level data

## Evaluation Methods

The clustering solution was evaluated using:

* Elbow Method (WCSS)
* Silhouette Score
* Cluster Profiling Analysis
* PCA Visualization

## Key Findings

* Countries were successfully segmented into meaningful socio-economic groups.
* One cluster exhibited significantly higher child mortality and lower life expectancy.
* Another cluster showed high income levels and high GDP per capita, representing developed nations.
* The underdeveloped cluster contained countries requiring immediate financial assistance.
* PCA effectively reduced dimensionality while retaining most of the information.

## Conclusion

This project demonstrates a complete end-to-end Unsupervised Machine Learning pipeline, including data validation, exploratory data analysis, preprocessing, dimensionality reduction, clustering, cluster evaluation, profiling, and business recommendations.

The analysis provides valuable insights that can help HELP International allocate resources efficiently and prioritize countries most in need of aid.
