# Road Accident Data Analysis

### Project Overview

This data analysis project aims to provide insights into a Road Accident data for the years 2021 and 2022. By analysing various aspects of the Road Accident data, we seek to identify trends, make comparisons, highlight the relationships between the variables in the data, and gain a deeper understanding of the distribution of casualties.

### Data Sources

Road Accident Data: The primary dataset used for this analysis is the "Road Accident Data.xlsx", containing detailed information about each occurence of accidents in 2021 and 2022.

### Tools

Excel: The Microsoft Excel tool was used from start to finish of this project, including, data cleaning, data processing, data analysis and creating of dashboard.

### Data Cleaning/Preparation

  In the initial data preparation phase, we performed the following tasks;
  - Data loading and inspection.
  - Handling wrong and missing values, as well as typographies.
  - Data cleaning and formatting.

### Exploratory Data Analysis

EDA involved exploring the accident data to generate key questions and highlight the requirements of the project. This includes questions like;
- What is the total casualties taken place after the accident?
- What is the percentage of total casualties with respect to the accident severity?
- What is the percentage of total casualties with respect to vehicle type?
- What is the maximum casualties by road type?

### Data Processing

Based on the requirements of this project, the following processes were made;
1. A "Month" column was added by inserting a new column and using the Text function to extract the first three letters of the month from the date column.
 ``` Excel Function
   =TEXT(B2,"mmm")
   ```
2. A "Year" column was added by inserting a new column and using the Text Function to extract the year from the date column.
 ``` Excel Function
   =TEXT(B2,"yyyy")
   ```
