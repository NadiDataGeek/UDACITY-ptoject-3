# (Ford GoBike System Dataset)
## by (Naod Mergiya)


## Dataset

> This dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. Only data for the month of Feburary, 2019 was provided in the classroom, however, I went ahead to obtain links to monthly datasets from January to December, 2019 from this lnk: https://s3.amazonaws.com/baywheels-data/index.html

Variables in the Dataset Include: 1. duration_sec 2. start_time 3. end_time 4. start_station_id 5. start_station_name 6. start_station_latitude 7. start_station_longitude 8. end_station_id 9. end_station_name 10. end_station_latitude 11. end_station_longitude 12. bike_id 13. user_type 14. bike_share_for_all_trip 15. rental_access_method

For my data wrangling process, I converted dtype of 'start_time' to datetime object, then split start_time into date and time columns. Afterwards, I extracted day and month from start_time column, extracted hour from start_time column, converted 'hour' column into int dtype, dropped irrelevant columns, drop rows containing missing values, and obtained trip distance in km from latitude and longitude columns


## Summary of Findings

> 10.8% of bike rides were taken by customers, while 89.2% were taken by subscribers 2. For both subscribers and customers, number of trips peaked at 8am and 5pm 3. Subscribers took the most trips in March, while customers took the most trips in December 4. Customers spent more time on trips and also covered longer distance compared to subscribers 5. Most bike trips were taken on weekdays, however, the longest bike trips in terms of duration, were taken on weekends.


## Key Insights for Presentation

> It is interesting to see that eventhough most bike trips were taken on weekdays, longest bike trips in terms of duration were actually taken on weekends. 2. Eventhough subscribers take more rides than customers, it is interesting to see that customers travel for longer distance and longer periods. 3. The longer the trip duration and trip distance, the lower the number of trips