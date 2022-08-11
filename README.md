# Surfs Up: Weather Analysis with SQLite and SQLAlchemy
Provided with SQLite database containing weather information for the island of Oahu in Hawaii a weather analysis was conducted using the SQLite query editor SQLAlchemy to reveal temperature trends.

## Overview
Data retrieval was conducted to obtain summary statistics about temparture data for the months of June and December in Oahu. These summary statistics were obtained in order to determine the sustainability of keeping a surf and ice cream shop business open year-round. The database used for this analysis is found in the hawaii.sqlite file. The code for data retrieval and summary statistics can be found in the SurfsUp_Challenge.ipynb file. 

## Results 
Temperature data for June and December were plotted and displayed in histogram graphs. A summary dataframe of the summary statistics for each month was also created to show a side by side comparison
- June Temperature Histogram
The data was sorted into 20 bins. The graph follows a bell curve and a more normal distribution around the mean compared to the December Temperature Histogram.  

![Screen Shot 2022-08-11 at 7 08 52 PM](https://user-images.githubusercontent.com/104794100/184257167-8027e2da-f933-40db-8d19-d3e0c4cf8660.png)

- December Temperature Histogram 
The data was sorted into 20 bins. The graph has a less normal distribution around the mean compared to the June Temperature Histogram and there is a larger range in recorded temperatures in December compared to June. 
![Screen Shot 2022-08-11 at 7 09 35 PM](https://user-images.githubusercontent.com/104794100/184257228-ae750bef-dd41-45a0-aed9-dfca3f6d0b90.png)

- Summary DataFrame
The average temperature in June (~75 degrees F) is almost 4 degrees F higher than the average temperature in December (~71 degrees F). The minimum temeprature in December (56 degrees F) is 8 degrees F lower than the minimum temoperature in June (64 degrees F), but the maximum temperature in December (83 degrees F) is only 2 degrees F lower than the maximum temeperature in June (85 degrees F). The recorded temperatures in December are much more variable the recorded temperature in June. 

![Screen Shot 2022-08-11 at 7 02 12 PM](https://user-images.githubusercontent.com/104794100/184256858-a223a7bf-8762-4578-b73b-ab33d04ca032.png)

## Summary of Findings
June and December average temperatures on the island of Oahu are similar. Although the histogram for December temperatures shows that the temperature is much more varible compared to the recorded temperatures for June, this should not be a reason to dismiss the idea of keeping the surf and ice cream shopopen year round. Attention should be turned to the median of the December temperature graph. The median of the December graph is about 72 degrees F and this temperature is recorded during the month of December at a frequency more than double the frequency of the next two most frequently recorded temperatures. This means that even though the temperature in December is much more variable compared to the temperature in June, it is still very consistently 72 degrees F. 
Before making the final decision about keeping the surf and ice cream shop open year round, additonal queries should be conducted using the weather data. -- Precipitation should be considered along with temperature. A query should be conducted to retrieve summary statistics about the precipitation levels during these two months.
- The stations at which these temperatures are recroded should also be considered. Summary statistics for each month should be compared by station. The frequency of records per station and the variance in temperatures per stations can be compared to locate where the least temperature variance occurs 
