# <center>FordGo Bicycle Sharing System</center>
### <center>by</center>
## <center>Shedrack David</center>

## Dataset
FordGo is a regional public bicycle sharing system in California's San Francisco Bay Area. It is operated by Motivate in a partnership with the Metropolitan Transportation Commission and the Bay Area Air Quality Management District. Bay Wheels is 'the first regional and large-scale bicycle sharing system deployed in California and on the West Coast of the United States. It was established as Bay Area Bike Share in August 2013. the system was officially re-launched as Ford GoBike in a partnership with Ford Motor Company. After Motivate's acquisition by Lyft, the system was renamed to Bay Wheels on June 11, 2019. This investigation explores a dataset containing FordGo's trip data for each month in the year 2019.

A part of this dataset was gotten from Udacity's project 3 Data Analytics projects and the remainder of th data was gotten from  <a href="https://www.kaggle.com/datasets/moamenabdelkawy/bay-wheels-trip-data-full-august-2021">kaggle</a> 
This data set includes 2,390,220 information about individual rides made in the bike-sharing system covering the greater San Francisco Bay area for the year of 2019

In the wranling phase, i merged the entire dataset for the year 2019 into one csv file, then converted the time stamps to datetime format, dropped all unnecessary columns i wasn't going to use, feature engineered a new column which held a category data for time of day, also feature engineered another column which held months of the year by names, dropped all NaN values and duplicates, changed trip durations from seconds to minutes, Finally, to make my analysis easier, I converted a categorical variable of user type to a dummy variable; and since duration had extreme outliers, I cut it at the 99𝑡ℎ percentile and day at 0 to remove ngative days..

The wrangled dataset contains 2,371,857 entries in the dataset with 9 columns.
- duration
- start_time
- end_time
- is_weekend
- user_is_subscriber
- trip_time_of_day
- start_month 
- time_diff
- start_station_name
- end_station_name

## Summary of Findings
- Most users of Bay Wheels are subscribers (80.7% of all users)
- Popular start and end stations are entirely different.
- Customers tend to have more duration for their trips, their distribution also have more spread compared to subscribers.
- Significant drop in Subscribers demand for bikes on weekends while Customers demand remained smooth accross the week
- Customers tend to have more duration for their trips, their distribution also have more spread compared to subscribers.
- the most busy day appears to be 11th and 12th day of the month with the most trips, but drops significantly on the 15th, 16th and 27th day.
-  most trips are taken at late hour of the day between the hours of 4-6pm and at early hours of the day between the hours of 7-9am.
-  most trips are taken during weekdays rather than weekends. thursdays and teusdays seem to be the most prefered days to take a trip.
- The median trip duration for customers is higher than subscribers on all weekdays.
- Customers' trip durations distribution have higher spread on all weekdays compared to subscribers.
-  Subscribers demand for bikes really peaked in the month on march and april but drastically drops in the month of december even below that of Customer
- On an hourly basis, both user groups have the same peak and off-peak hours; but "Subscribers" demand was more volatile.

## Key Insights for Presentation


- FordGo or Bay Wheels differentiate between two user groups; "Subscribers" who are members of an annual or a monthly plan, and "Customers" who pay for each single trip. During the investigation period, 80.7% of users were "Subscribers", while 19.3% were "Customers".

- A question of interest for this analysis is to know when when most trips taken in terms of time of day or month of the year, From investigating the dataset

most trips are taken at late hour of the day

most trips are taken during weekdays rather than weekends. thursdays and tuesdays are the most prefered days to take a trip.

on average, trips on weekends tend to be slightly longer than on weekdays and has less outliers and more spread distribution

- Most trips were taken in the month of March and April but drastically drops in the month of December.

changes in monthly trips count tended to be similar for both user groups; this pattern persists till November and in the month of December, the number of "Customers" became, higher than this of "Subscribers".

- for both users, trips peak around the hours of 8-9am and 5-6pm but drops around 10am - 3pm. though it seems to drop more significantly for subscribers

customer's trips tends to peak on the 12th, 13th and 19th day but seems to drop significantly on the 14th and 15th day, while for subscribers, it peaks on the 11th and 12th day but drops on the 15th and 27th day

subscribers trips peaks mostly on weekdays but significantly drops on weekends while customers demand seem consistent accross the entire week, we could assume that most subscribers use bikes to and from their works based on our findings for trips per hour

- Trip durations in the dataset ranges from 1minute to about 90minutes. The distribution is right-skewed on a linear scale but when plotted on a logarithmic scale, the distribution of trip durations gets closer to normal but with a rough shape.


- Customers tend to have more duration in their trips than Subscribers and their distribution also have more spread compared to Subscribers. In other words, Customers tend to vary their trip durations, while Subscribers mostly use the service for short trips.

Duration distribution has more spread on weekends for both user types but is more apparent for Customers, and the meadian trip duration for Customers has more spread which means Customers tend, on average, to take longer trips, and their trips' durations vary more compared to Subscribers.

## Useful Feedback
I increased the size of the piechart for clearer visuals

## Resources

-  <a href="https://en.wikipedia.org/wiki/Bay_Wheels ">Wikipedia page on FordGo/Bay Wheels</a> 
-  <a href="https://stackoverflow.com/">stackoverflow</a>
-   <a href="https://www.geeksforgeeks.org/grouping-and-aggregating-with-pandas/ ">geekforgeeks</a>

## Notes

- the dataset used for my exploratory analysis was uploaded to kaggle(download it  <a href="https://www.kaggle.com/datasets/shedrackdavid/bay-wheels-data-set-for-the-year-2019">here</a> )
-  the datasets for each month of the year 2019 was also uploaded to kaggle(download it  <a href="https://www.kaggle.com/datasets/shedrackdavid/bay-wheels-dataset-for-each-month-in-the-year-2019 ">here</a> )


```python

```
