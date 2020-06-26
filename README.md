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
Calculated total rides for each city types,total drivers for each city types,the total fares for each city types,the average fare per ride for each city types,the average fare per driver for each city types.To create the summary DataFrame, from the merged DataFrame got the total rides, total drivers, and total fares for each city type using the groupby() function on the city type.Calculated the average fare per ride and the average fare per driver for each city type.Deleted the index name pyber_ride summary_df.index.name.
Created the summary DataFrame with the appropriate columns- Total fare,Average Fare per Ride,Average Fare per Driver formatted with currency dollar and rounded t 2 decimal place.

The Total fare is shown by City Type. Rural,Subarban and Urban.The fare in Urban cities seems to be more than the rural and subarban is in the mid of the two. The trend seem to remain identical irrespective of the city.Sometimes between February and March sees the peak of the fare. 

![Fare](Challenge_fare_summary.png)


## Challenges Encountered and Overcome

### Challenges and Difficulties Encountered

   ### Programming:
    Some rows will contain NaNs
   ### Data analysis:
    Did not help in the analysis as there was no data showing up 
   ### Graphing:
    The plotting was difficult because of NaNs. I could not draw any inference from the graph.
### Technical Analyses Used
Created a new df and used resample by week and got sum of the fares for each week
weekly_fares_df = fare_Jan_April.resample("W").sum()
## Recommendations and Next Steps


### Recommendations for Future Analysis

### Additional analysis I

* I will probably do a deep dive on Urban. Introduce some incentives such as earning reward point.That will increase the turnover in Urban areas 
* Technical Steps
I will introduce a dataset rewards. add a filter to the cities and filter Urban to see the increase in the fare.

### Additional Analysis II

* I will dig deep into weekly analysis involving categories of riders. If we see the rides mainly to the downtown area during weekends or maybe at one particular time the riders are to a particular location where there is college I can come up with offers for those frequent riders. 

The frequent riders can earn points and utilize that to purchase other stuff.
