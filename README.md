# Police Annual Statistical Report - Arrested and Charged Persons Dataset

## Overview
This README provides comprehensive information and documentation for the "Police Annual Statistical Report - Arrested and Charged Persons" dataset. This dataset contains information on persons who have been arrested and charged, including details such as division, neighbourhood, sex, age, crime category, and crime subtype. This README will guide you through various aspects of the dataset, including its contents, data cleaning, exploratory data analysis, machine learning modeling, and more.

## Table of Contents
1. [Dataset Description](#dataset-description)
2. [Dataset Limitations](#dataset-limitations)
3. [Data Cleaning](#data-cleaning)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Machine Learning Modeling](#machine-learning-modeling)
6. [Conclusion](#conclusion)

## Dataset Description<a name="dataset-description"></a>
- **Dataset Name:** Police Annual Statistical Report - Arrested and Charged Persons
- **Dataset Size:** 129,374 entries and 11 columns

### Columns:
1. **ARREST_YEAR**: The year in which the arrest occurred.
2. **DIVISION**: Police division code, indicating the area of arrest.
3. **HOOD_158**: Neighborhood code corresponding to the arrest location.
4. **NEIGHBOURHOOD_158**: Name of the neighborhood.
5. **SEX**: Gender of the arrested person (Female, Male, Unknown).
6. **AGE_COHORT**: Age cohort of the arrested person (e.g., '<18', '25 to 34', '65+', Unknown).
7. **AGE_GROUP**: Age group of the arrested person (Adult, Youth, Unknown).
8. **CATEGORY**: Crime category (e.g., 'Crimes Against the Person', 'Other Criminal Code Violations', etc.).
9. **SUBTYPE**: Subcategory of the crime.
10. **ARREST_COUNT**: Count of arrests for each entry.
11. **NO_SPECIFIED_ADDRESS (NSA)**: Indicates whether the arrest occurred outside the City of Toronto limits or has no verified location.

## Dataset Limitations<a name="dataset-limitations"></a>
The dataset has a few limitations:

1. **Filtered by Arrest Year:** The data is filtered by arrest year, and the dataset may not include arrests from all years.

2. **Age Calculation:** Age is calculated based on the date of occurrence, which might not be precise.

3. **No Specified Address (NSA):** The 'NSA' category includes occurrences reported outside the City of Toronto limits or those that have no verified location.

## Data Cleaning<a name="data-cleaning"></a>
The data cleaning process included the following steps:

- Checked for missing values (none found).
- Analyzed and handled 'NSA' and 'Unknown' entries in relevant columns.
- Examined and prepared the dataset for further analysis and modeling.

## Exploratory Data Analysis (EDA)<a name="exploratory-data-analysis-eda"></a>
The EDA phase involved exploring various aspects of the dataset, including:

- Yearly trends in arrests.
- Distribution of crime categories and subtypes.
- Demographic distribution (age and gender) of arrested persons.
- Geographical distribution of arrests by neighborhood and police division.
- Correlation analysis between variables.

## Machine Learning Modeling<a name="machine-learning-modeling"></a>
Machine learning modeling was performed to predict crime categories based on age, gender, and neighborhood. Key steps included:

- Data preparation, including feature encoding and splitting into training and testing sets.
- Initial modeling using a Random Forest Classifier.
- Model evaluation and analysis of performance.
- Grid search for hyperparameter tuning.
- Training and evaluation of a Gradient Boosting Classifier.

The models achieved varying levels of accuracy in predicting crime categories.

## Conclusion<a name="conclusion"></a>
This README provides an in-depth overview of the "Police Annual Statistical Report - Arrested and Charged Persons" dataset, including its contents, limitations, data cleaning process, exploratory data analysis, and machine learning modeling. It serves as a comprehensive guide for understanding and working with this dataset, which contains valuable insights into arrests and charges in Toronto. Further analysis and improvements in modeling can lead to more accurate predictions and insights into criminal activities in the region.
