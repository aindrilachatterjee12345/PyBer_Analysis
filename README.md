# PyBer_Analysis
  Pyber Analysis
    
## The notebook generates a summary DataFrame that contains 
  Total Rides,
  Total Drivers,
  Total Fares,
  Average Fare per Ride,
  Average Fare per Driver.
## The notebook generates a summary DataFrame, where all of the following are completed:
  All 15 values in the rows are correct according to the solution,
  the index name is deleted after creating the summary DataFrame and
  all of the columns that need formatting are formatted
## Line chart matches the line chart provided in the homework solution
  There is one graph like the solution containing all three city types over the time period specified,the data graphed from the DataFrame created using
  .resample(‘W’).sum().The line chart has the axes labels and chart title are properly annotated, the “fivethirtyeight” graph style is used.

  # PyBer Analysis Report

## Background and Purpose
The purpose is creating a summary DataFrame of the key metrics for the ride-sharing data by city type; creating a multiple-line graph that shows the total fares for each week by each city type; and submitting a written report on the results of the new analysis, challenges encountered and overcame, and any future recommendations for analysis.

### Technical Analysis
Loaded the files - city_data_to_load and ride_data_to_load.Read the city data file by using pd.read_csv(city_data_to_load) and store it in a pandas DataFrame.Read the ride data file pd.read_csv(ride_data_to_load) and store it in a pandas DataFrame.Combined the data into a single dataset by using pd.merge(ride_data_df, city_data_df, how="left", on=["city", "city"]).
### Results

### Summary

## Challenges Encountered and Overcome

### Challenges and Difficulties Encountered

* Programming

* Data analysis

* Graphing, etc

### Technical Analyses Used

## Recommendations and Next Steps

### Recommendations for Future Analysis

### Additional Analysis 1

* Description of Approach

* Technical Steps

### Additional Analysis 2

* Description of Approach

* Technical Steps
