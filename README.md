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
- What month of the year does an accident occur the most?
- What is the percentage of total casualties with respect to the Accident Severity?
- What is the percentage of total casualties with respect to Vehicle Type?
- What is the maximum Casualties by Road Type?
- What is the distribution of Total Casualties by Road Surface?
- What is the relation between Casualties and Light Conditions (DAY/NIGHT)?
- What is the relation between Casualties and Area/Location

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

### Data Analysis

Using Pivot Tables, the following analysis was being done;
1. Sum of number_of_casualties to calculate the total casualties.
2. Sum of number_of_casualties grouped by the accident_severity to calculate the percentage of each accident severity of the total.
3. Sum of number_of_casualties grouped by the vehicle_type to calculate the casualties by each vehicle types.
   - This is done  by using the "Calculated Items" option in the pivot table to combine some vehicle types that fall within the same category.
   - After combining similar vehicles, we are then left with 6 vehicle types (Agricultural Vehicle, Car, Vans, Bike, Bus and Others).
4. Number_of_casualties grouped by the each months and filetered by each year. This was done to access the casualties in each month and create a combo chart of monthly trend for each year.
5. Sum of number_of_casualties grouped by the Road_type to calculate the casualties by each Road type, as well as format the values into thousands (K) to make it look concise for the dashboard.
6. Sum of number_of_casualties grouped by the Road_Surface_Conditions to calculate the casualties by Road surfaces.
   - This is done  by using the "Calculated Items" option in the pivot table to combine some Road surface conditions that fall within the same category.
   - After combining similar Road surface conditions, we are then left with 3 Road condition types (Dry, Wet, and Snow/Ice).
7. Sum of number_of_casualties grouped by the Are/Location to calculate the casualties by either the Urban or Rural Area, as well as format the values into thousands (K) to make it look concise for the dashboard.
8. Sum of number_of_casualties grouped by the Light conditions to calculate the casualties by either night or day, as well as format the values into thousands (K) to make it look concise for the dashboard. I also made use of the "Calculated Items" option in the pivot table to combine some Light conditions that fall within the same category.
9. We then created a Timeline using the Accident date and connecting it to all other pivot table created except that of the monthly trends.
10. A slicer was also created using the Urban/Rural Area and connecting it to all other pivot table created.

### Results/Findings

The analysis results are summarised as follows;
- Cars are involved in the most accidents, with cars constituting almost 80% of all casualties in the previous and current years.
