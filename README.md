# Ford Go Bike data Exploration
## by Scholastica Wambui Muigai 


## Dataset

This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area
The data set has been stored as a pandas dataframe, It has 16 columns and 183412 rows. 
In this dataset I look onto three main features; trip information, station and member information

### Data Wrangling Process
Data wrangling process:
* fix multiple fields that are not in the correct dtype, i.e. start_time, end_time should be datetime type, user_type and member_gender should be categorical data type, etc
* add new columns for trip duration in minute, trip start date in yyyy-mm-dd format, trip start hour of the day, day of week and month
* add a new column calculating riders' age from 'member_birth_year'
* filter out outlier ages from visual examination of the member age distribution and statistical percentile
* cast 'member_birth_year' and 'member_age' to integer instead of float type
* cast 'start_dayofweek' to category dtype
* cast 'start_month' to category dtype for easy plotting
* filter out outlier trip records where the duration was very long

The Goal of this presentation is to explore the main features of bike-sharing in the greater San Francisco Bay area. The main goal here is to specify the main determinants of trip duration by looking at the relationship between trip duration and other explanatory variables in the dataset. We try to answer the following questions:

1. What does the distribution of trip duration look like?
2. Which days have the highest demand on trips?
3. Which hours during the day have the highest demand on trips?
4. How trip duration differs by user age, hour, day, and user type?

## Summary of Findings
When exploring the data,I came up with the following findings;
1. Most of the users are subscribed in this system (the number of subscribers are more than 9 times greater then those of customers)
2. The number of rides decreases greatly during the weekends (saterday and sunday) compared to the number of rides during the rest of days in the week.
3. The average trip duration during weekends (saturday and sunday) is longer than that during the rest of week the male users have the least trip duration in general , the average trip duration for all genders increased at hte weekend (saterday and sunday) which can be explained that the trips during the weekends are for entertainment where no need to hurry.
4. The subscribers users have the least trip duration in general , the average trip duration for both subscribers and customers increased at the weekend (saterday and sunday) especially the customers which can be explained that the trips during the weekends are for entertainment where no need to hurry
5. More than 90% of the trips are below 20 minutes.
I also observed that the interactions between features are all supplementing each other and quite make sense when looked at combined. 


## Key Insights for Presentation

Used different visualizations to convey the distribution of age against duration and type of user against gender.