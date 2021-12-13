# NYC Citibike Analysis Overview
This analysis prepares visualizations of the highly-successful NYC bike-sharing program to support a business proposal targeting potential investors for a similar bike-sharing program in Des Moines. To solidify the proposal, one of the key stakeholders would like to see a bike trip analysis.
For this analysis the following set of visualizations are created:

- Length of time that bikes are checked out for all riders and genders
- The number of bike trips for all riders and genders for each hour of each day of the week
- The number of bike trips for each type of user and gender for each day of the week.

These visualizations along with previously generated ones are used to support the creation of a final presentation and analysis to pitch to investors.

# Resources
- Data Sources: 201908-citibike-tripdata.csv, citibike_tripdata.csv (converted "tripduration" column to datetime format)
- Software: Python, Jupyter Notebook, Tableau


# Results:
Visualizations for business proposal created in Tableau:  [Link to Tableau Story](https://public.tableau.com/app/profile/scott.yoder8657/viz/NYC_CitiBike_Challenge_16383067025460/NYC_CitiBike_Analysis?publish=yes)

## Convert "tripduration" column 
The data in the "tripduration" column in the 201908-citibike-tripdata.csv file is converted into a datatime datatype using Pandas library in Jupyter Notebook and exported to citibike_tripdata.csv.

![Alt Text](https://github.com/syoder821/bikesharing/blob/main/Resources/Images/converted_tripduration_column.png)


## Trip Duration and Gender Breakdown
First two major observations are: Males are by far the largest Gender group of riders and the majority of trip durations are under 60 minutes peaking at 5 to 6 minutes.

![Alt Text](https://github.com/syoder821/bikesharing/blob/main/Resources/Images/Story1.png)


## Start and Stop Locations
Top Starting and Ending Locations.  The most active starting locations are also among the most active ending locations

![Alt Text](https://github.com/syoder821/bikesharing/blob/main/Resources/Images/Story2.png)


## Checkout Times for Users and Checkout time by Gender.
Most rides are less than 20 minutes and are similar lengths by Gender.

![Alt Text](https://github.com/syoder821/bikesharing/blob/main/Resources/Images/Story3.png)


## Trips by Weekday per Hour and Trips by Gender (Weekday per Hour)
Morning (7-9am) and evening (4-7pm) commute times show the highest trip volumes.  Pattern is independent of gender with total number of trips the greatest for males.  Wednesday shows a drop in the number of trips vs. other weekdays.  

![Alt Text](https://github.com/syoder821/bikesharing/blob/main/Resources/Images/Story4.png)


## User Trips by Gender by Weekday
User Trips by Gender by Weekday heatmap shows the following: male subscribers greatly out number female and unknown subscribers,  customer's gender is often unknown, and Wednesday is the weekday with smallest number of trips.

![Alt Text](https://github.com/syoder821/bikesharing/blob/main/Resources/Images/Story5.png)

# Summary
The results of this analysis give insight into the NYC Citibike bike-sharing program and can be used for the investor proposal for starting a similar program in Des Moines.  The analysis shows that vast majority of riders are male and the vast majority of rides are less than 20 minutes in duration with the largest number of rides in the 5 to 6 minute range.  The weekday usage is concentrated around the morning and evening commute times while the week end usage is spread more evenly throughout the day. It is also noted that the most active starting locations are also the most active ending locations.  
Additional visualizations to produce would be:
1. Compare weekend trip duration to weekday trip duration
2. For the morning and evening commute time window, look at the starting and ending locations in order to capture the flow of traffic between neighborhoods at peak ours.
3. An analysis of the ages of subscribers versus customers. 
4. Analyze the length of time that bikes are checked out per day. This would identify if and when the bikes are used for longer periods of time on weekends versus weekday commutes. This information could be used to help plan the bike maintenance schedule. 
5. The current analysis was only performed for the month of August in New York City. Analyzing the bike share useage during other months would be valuable for the Des Moines proposal by providing a clearer picture of a full year of the bike share program.
