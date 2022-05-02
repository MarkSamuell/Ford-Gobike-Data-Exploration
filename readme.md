# Ford Gobike Data Exploration and Visualization <br />
### by Mark Samuel

## Dataset:
###### This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. 
<br>

## The structure of the dataset 
<br>
- The data after wrangling contains 174952 individual trip records with 20 variables collected. The variables can be divided into 4 major categories:<br>

#### 1- trip duration info: <br>
(duration_sec, duration_mins) <br>
<br>
#### 2- station info: <br>
(start_station_id, start_station_name, start_station_latitude, start_station_longitude, end_station_id, end_station_name, end_station_latitude, end_station_longitude) <br>
<br>
#### 3- time info: <br>
(start_time, start_hour, start_day, end_time) <br>
<br>
#### 4- user info: <br>
(bike_id, user_type, member_birth_year, member_gender, bike_share_for_all_trip, member_age)
<br>
<br>
##### Variables are drived to 11 numerical variables, and others are 4 datetime, 4 object 'string' type and 1 is boolean type.


### What is/are the main feature(s) of interest in the dataset?
<br>
- in my opinion the main feature to the company will be the trip duration and how it changes by the influence of other fea
tures.
<br>
<br>
- also, how trip duration may influnece other features.
<br>
<br>
- some important other features are (start and end station, start hour, start day, gender and age)

### What features in the dataset will help support the investigation into feature(s) of interest?
<br>
- the start station and end station will affect duration owing to the distance between them.
<br>
- user type, member gender and member age will also affect the duration of the trip.
<br>
- Also 'bike_share_for_all_trip' may affect the duration of the trip.

## Data Wrangling:
##### -remove nans 
##### -change dates to datetime
##### -divide "start_time" colum to two columns(start_hour, start_day)
##### -change the data type for "bike_share_for_all_trip to" be bool
##### -convert "duration_sec" to duration by minutes 
##### -add "member_age" column
##### - make new column that divide member age to three categories ['young', 'middle aged', 'old']


### Findings:
<br>
1.  not many trips exceed one hour duration and most trips are between 3 to 30 minutes.
<br>
2- about 75% of our users are young people between 20's and 40's
<br>
3. more than 90% of our users are subscribers
<br>
4. about 75% of our users are males
<br>
5. the trip count is decreased by 50% during Sunday and Saturday
<br>
6. that most of trips are occur between 7 a.m and 8 p.m, and it reachs to the peak at 8 a.m and 5 p.m
<br>
7. the popular start stations are almost the popular end stations too.
<br>
8. Sunday and Saturday have the highest duration average
<br>
9. Customers have higher average duration than Subscribers, however Subscribers have the higher number of trips
<br>
10. Bike share for all trip works only with trips that have lower duration.
<br>
11. age group doesn't affect the duration of the trip that much.
<br>
12. females have higher average duration trips, while men have higher trip number.
<br>
13. the average duartion of trips is almost the same eiher bike share all trip or not, except on sunday and monday
<br>
14. Customers never use bike share for all trip, while Subscribers do.
