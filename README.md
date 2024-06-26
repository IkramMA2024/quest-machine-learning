# NYPD Complaint Data Analysis and Classification Project

## Introduction
This project aims to utilize the NYPD Complaint Data Historic dataset to develop a machine learning model for predicting the profile of a suspect based on various features such as location, date, time, type of offense, and more. The primary objective is to clean, explore, and preprocess the data to prepare it for a supervised machine learning classification task.

## Data Collection
### Path to the File
The dataset was loaded from a specified file path with selected columns that are pertinent to the analysis.

### Columns to Keep
The columns retained for analysis include:
- Date and time of the complaint (`CMPLNT_FR_DT`, `CMPLNT_FR_TM`)
- Offense codes and descriptions (`KY_CD`, `PD_CD`, `PD_DESC`, `OFNS_DESC`)
- Crime completion status (`CRM_ATPT_CPTD_CD`)
- Law category code (`LAW_CAT_CD`)
- Location details (`PREM_TYP_DESC`, `Latitude`, `Longitude`, `LOC_OF_OCCUR_DESC`)
- Suspect information (`SUSP_AGE_GROUP`, `SUSP_RACE`, `SUSP_SEX`)
- Victim information (`VIC_AGE_GROUP`, `VIC_RACE`, `VIC_SEX`)

## Data Analysis
### Null Values Analysis
An analysis was performed to identify the number and percentage of missing values for each column. This step helps to understand the extent of missing data and plan for appropriate data cleaning strategies.

### Data Types Analysis
The data types of each column were checked to ensure they are appropriate for the type of data they hold. This step is crucial for further data manipulation and analysis.

### Categorical Columns Analysis
The unique values and their proportions were calculated for categorical columns to understand the distribution and frequency of different categories within the dataset.

## Data cleaning

### Date & Time Analysis and Cleaning
Convert and Clean Date & Time Data
- **Conversion**: Date and time columns were converted to appropriate datetime formats.
- **Missing Values Removal**: Rows with missing or null values in the date and time columns were removed.
- **Filtering by Year**: Data was filtered to include only records from the year 2006 onwards.

### Summary of Date and Time Analysis
- **Date Range**: The range of dates in the dataset was identified after filtering.
- **Time Range**: The range of times in the dataset was identified.
- **Values Per Year**: The number of records per year was calculated to understand the distribution of data over time.

### Analysis of Numerical Columns
Latitude and Longitude
Basic statistics were calculated for the latitude and longitude columns, and boxplots were created to identify any outliers.

### Suspect and Victim Age Groups
Basic statistics were calculated for the suspect and victim age groups, and boxplots were created to visualize the distribution and identify any outliers.

## Summary
This project involved several steps to clean, preprocess, and analyze the NYPD Complaint Data Historic dataset in preparation for building a machine learning classification model to predict the profile of suspects based on various features. The steps included:

1. **Data Collection**: Loading the dataset and selecting relevant columns.
2. **Initial Analysis**: Performing null value analysis and data type verification.
3. **Categorical Columns Analysis**: Analyzing value counts and percentages for categorical columns.
4. **Date & Time Analysis and Cleaning**: Converting date and time columns, filtering data, and calculating the percentage of rows removed.
5. **Numerical Columns Analysis**: Analyzing latitude, longitude, suspect age, and victim age with descriptive statistics and visualizations.

This thorough data preparation is crucial for developing a reliable and accurate machine learning model for the classification task.
