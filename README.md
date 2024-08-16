# Temperature and Corn Yield: Insights from Historical Data in the United States

## Overview
This project involves analyzing corn yield data from the United States in relation to average temperature data. The goal was to explore the relationship between temperature and corn yield and assess whether temperature alone could be used to predict corn yield. This analysis uses data spanning several decades and covers various states in the U.S.

## Data Description

### Corn Yield Data
- **Source**: U.S. Department of Agriculture (USDA)
- **Columns**:
  - **Year**: The year of the record.
  - **State**: The state where the data was recorded.
  - **State ANSI**: An identifier for the state.
  - **Value**: The corn yield, measured in bushels per acre (or another unit).

### Temperature Data
- **Source**: National Oceanic and Atmospheric Administration (NOAA)
- **Columns**:
  - **Year**: The year of the record.
  - **State**: The state where the data was recorded.
  - **average_temp**: Average monthly temperature in Fahrenheit.
  - **centroid_lon**: Longitude of the state's centroid.
  - **centroid_lat**: Latitude of the state's centroid.

## Data Preparation

### Data Import
Data was imported and merged based on common columns (Year and State), resulting in a unified dataset containing both corn yield and temperature data.

### Data Cleaning
- **Missing Values**: Handled by identifying and removing rows with missing values.
- **Column Selection**: Focused on relevant columns from both datasets for analysis.

### Merged Data
The final merged dataset includes:
- Year
- State
- State ANSI
- Value (Corn Yield)
- average_temp (Average Temperature)

## Exploratory Data Analysis (EDA)

### Summary Statistics
Key statistics for corn yield by state include:
- **Mean**: Varies by state, with states like California having higher average yields.
- **Standard Deviation**: Indicates variability in corn yield within each state.
- **Min/Max**: Provides insight into the range of corn yields.

### Correlation Analysis
- **Correlation Coefficient**: The correlation between corn yield and average temperature is -0.072905, indicating a very weak negative linear relationship.

## Visualization
- **Corn Yield Over Time**: Visualizations showed trends in corn yield across different states over time.
- **Average Temperature Over Time**: Graphs illustrated changes in average temperature over time across various states.
- **Temperature vs Corn Yield**: Scatter plots demonstrated the weak relationship between average temperature and corn yield.

## Conclusions
- **Temperature as a Predictor**: The analysis shows that average temperature alone is not a strong predictor of corn yield. The correlation coefficient of -0.072905 suggests that temperature does not significantly influence corn yield in a linear fashion.
- **Further Analysis**: To improve predictions, additional factors such as soil quality, precipitation, and farming practices should be considered. Advanced machine learning techniques might also be necessary to capture non-linear relationships.

## Future Work
- **Incorporate Additional Features**: Including other variables such as soil moisture, precipitation, and crop management practices.
- **Advanced Modeling**: Employing machine learning models like Random Forests or Gradient Boosting to capture complex relationships and improve prediction accuracy.

