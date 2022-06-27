# Citibike Bikeshare Data Trends
### Project Overview: Analyze Citibike data and develop visualizations to demonstrate usage patterns, and convince investors that a bike-sharing program in Des Moines is a solid business proposal.
</br>

We analyzed 2,344,224 New York Citibike customer rides, and developed visualizations via Tableau based on the following analyses:
- Peak Hours for Citibike usage
- Amount of time the bikes were checked out for by ride
- Amount of time the bikes were checked out for, broken down by gender
- Concentration of bike rides by hour of day and days of week
- Concentration of bike rides by hour of day and days of week, further broken down by gender
- Concentration of bike rides by days of week, broken down by customer type and gender
- Top bike ride starting locations
</br>

## Results
[Link to Tableau Visualizations & Story](https://public.tableau.com/app/profile/alexandra.curtis/viz/BikesharingChallenge_16562246503820/BikeshareDataTrends?publish=yes)
</br>
</br>

## Summary
Our analysis and visualizations show the most substantial amount of business occurs between 5PM and 6PM.  The least amount between 3AM and 4AM.  Repairs would best occur between 3AM and 4AM, so as not to interfere with peak business hours.  Close to zero customers utilized the bikes for longer than one hour.  Most customers used the bikes around 10 minutes.  This exemplifies a utilitarian point A to point B type of usage, rather than utilizing the bikes for joy rides.

When we look at bike checkout times by gender, usage trends stay about the same (around 10 minutes) for both males and females, but males utilize the bikes much more than females.  Those whose gender is "unknown" appear to have slightly longer bike rides on average.  We think this is because customers that do not subscribe to the rideshare as a regular service generally do not provide their gender to the system.  Since the non-subscribers are not using it regularly, for things such as transit to work, they are using it for longer -- joy ride type usage.  This is further exemplified in the breakdown for regular customers versus subscribers.  While most customers are subscribers, and where males still turnout to be the most prominent users, there were no subscribers with "unknown" gender, and significantly more "unknown" gender non-subscribers than male or female non-subscribers. 

The concentration of hourly usage by day of week shows the number of trips is the greatest between 6AM and 9AM on weekdays, and again between 5PM and 7PM.  There is a large gap of time during the weekdays when usage subsides.  The time of usage is less concentrated and more spread out, between about 9AM to 6PM or 7PM, on the weekends.  The bikes appear to be utilized more often on Sundays than Saturdays.  Top bike ride starting locations are worth noting, so the company can conisider where to place majority of the bikes for optimal business.  Most trips begin around a centralized location, likely a downtown area.  It should be noted that this data is for New York City.  Des Moines will need to asses for their most centralized locations.
</br>
</br>

### Instructions to Download the CSVs
**Original Data Source:** Go to the [Citi Bike System Data Page](https://ride.citibikenyc.com/system-data). In the "Citi Bike Trip Histories" section, click the link that says "downloadable files of Citi Bike trip data." This link will take you to an index of trip data. Scroll down the list to 201908-citibike-tripdata.csv.zip.  This zip file contains all the August 2019 data. We used data from August, because there was likely more traffic during the summer months.
</br>
</br>
**Coverted Tripduration File:** We converted the "tripduration" column from an integer to a datetime datatype to get the time in hours and minutes, to be used for further analysis in Tableau.  Please open the NYC_CitiBike_Challenge.ipynb notebook in this repository, and print to_csv to get the updated csv.

