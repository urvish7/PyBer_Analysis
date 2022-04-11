# PyBer_Analysis
## Overview of the Analysis

  This assignment is given by the V. Isualize for using our Python skills and knowledge of Pandas. In this Analysis we are generating a summary Dataframe of the ride-sharing data by the city type. The results is done in the visualization of the multiple-line graph that shows the total weekly fares for each city type. After calculating the data we have to use it for decision making at PyBer.
  
## A ride-sharing summary DataFrame by city type
  In this Analysis part we going to summarize the data to Total Rides, Total Drivers, Total Fares, Average Fare per Ride and, Average Fare per Driver section. 
  We are going to use the groupby() function to fetch the Total Rides, Total Drivers and Total Fares from the given csv file data. after that we will calculate the average fare per ride by city and average fare per driver. 
  After the calculation, the data summary table looks like: 

![Pyber Summary](https://github.com/urvish7/PyBer_Analysis/blob/main/Extra%20Pics/pybersummary_final.png)
 
 ## A multiple-line chart of total fares for each city type 
   In this Analysis we going to use the pivot() and resample() function to create multiple-line graph that shows the total fares for each week by city type.
   From the step-1 we create the Dataframe with multiple indices by using the groupby() function on the type and date columns then, filter with the sum amounts of the fares in the column. In step-2 we use the pivot() function to index the dates and create a data frame looks like: 
 ![pivot function use](https://github.com/urvish7/PyBer_Analysis/blob/main/Extra%20Pics/Pivotfunction.png)

 In the further steps another new Dataframe is formed by using the loc method from the date range 2019-01-01 through 2019-04-28. Also we use the resample() method.Then we check the data type for the dates through the info() function and gives the table like:
 
![info fucntion for date](https://github.com/urvish7/PyBer_Analysis/blob/main/Extra%20Pics/date_info.png)
 
 
In the following step we used the resample() and sum() method to get the total fares for each week in respect to Urban, Suburban and Rural sections.

![the resample function table](https://github.com/urvish7/PyBer_Analysis/blob/main/Extra%20Pics/resample.png) 
 
  
### Results: 
  Overall when it comes to the Total rides, Total Drivers  and, Total Fares Urban leads the numbers to maximum compare to Suburban,while Rural standing at bottom. However, talking about the Average Fare per Ride and per Driver the Urban has the cheapest price compare to Suburban and Rural has the costliest. 
![graphical view](https://github.com/urvish7/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

### Summary
 - Urban fare is growing in the beginning months of the year, it fluctuates more in around March and April however keeps its numbers after May there is a sudden decline in numbers. 
 - Suburban fare leaps in the begining month of the year, however reaches maximum at the end of the February and does a sudden fall till March beginning. remains around $1000 between Mar and April after that takes a jump at the end of the April month and after May it collapes.
 - Rural does change a lot. The fare remains between $0-$500 thoughout the year. 
 - Recommendation: All in all keep the drivers data up to date and focus on the business more in the beginning of the year. the months till may are good earning phase for the business. we have keep the stabily after may as it shows the decline in the fares so keep less drivers on the road which helps in keeping stability in business.
