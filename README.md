# Citi_Bike

## Overview
This project includes a Tableau data story analyzing a dataset of user data collected by the bike ridesharing company "CitiBike" from its userbase in Manhattan island, NYC.  To prepare it for analysis, the dataset was first loaded into Python 3 using Pandas so that a datetime format could be applied, and then imported into Tableau, where a series of visualizations were generated, arranged into Dashboards, and then annotated with brief anlyses as part of a [Data Story](https://public.tableau.com/views/CitiBike_Analysis_DataStory/CitiBikeDataStory?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link).

### Purpose
The purpose of this project is to provide a hypothetical investor considering helping CitiBike to expand their operations in another city with useful and engaging insights into the existing userbase in Manhattan.  

## Results 
The first visualizations produced were two interactive maps using MapBox 2023 geospatial data.  These maps display green and red dots of varying sizes over the street locations where CitiBike users were recorded as having started and stopped their bike rentals, respectively.  The size of the dots correspond to the relative frequency of the recorded trips to or from those locations.  

![TopStarts](/Images/starts.png)

![TopStops](/Images/stops.png)

The second set of visualizations were created to show the number of bikes rented for various durations of time.  
![CheckoutUsers](/Images/checkoutusers.png)

Another version of this line graph was created to show how that data breaks down across gender.
![CheckoutGenders](/Images/checkoutgenders.png)

Finally, a series of heatmaps were created to observe user trends over the course of an average week.  The first of these heatmaps displayed trends for the entire userbase at hourly intervals.
![tripsweekdayhourly](/Images/tripsweekdayhourly.png)

The second version of this heatmap was filtered to separate out trends across genders.
![tripsweekdayhourlygenders](/Images/tripsweekdayhourlygenders.png)

The final heatmap broke down the userbase even further, by filtering between users who paid for each trip individually and those who subscribed to a reoccuring fee for the CitiBike service.
![tripsweekdaygendersusers](/Images/tripsweekdaygendersusers.png)


### Analysis
From these seven visualizations, three Dashboards were assembled in order to compare the data for analysis.  The first Dashboard arranged the two interactive maps side-by-side for comparison, revealing that the same locations were reported as both popular start and stop locations for bike rentals.  This pattern was hypothesized to indicate that many CitiBike users utlize the service for their regular commute.
![dash_toplocations](/Images/toplocations.png)

The second Dashboard compared the two line charts showing rental times and durations, revealing that the breakdown thereof across gender remained within an apparent normal distribution.  However, it was also observed that men are responsible for the majority of recorded user rentals.    
![dash_checkouts](/Images/dash_checkouts.png)

The third Dashboard compared the weekly useage heatmaps, corroborating the observation that men are responsible for the greatest number of recorded rentals.  Additionally, both men and women were observed to exhibit consistent use patterns during the work week where one rental trip would be recorded during the morning and another during the evening, further supporting the hypothesis that many CitiBike users utilize the service for their commute.  It was also noted that men make up the great majority of Subscriber renters.
![dash_tripsheatmaps](/Images/dash_tripsheatmaps.png)

## Summary
In conclusion, the hypothesis that male weekday commuters comprise the majority of CitiBike users appears to be supported across all of the angles from which the dataset was analyzed.  Moreover, men being the greatest portion of the reoccuring Subscriber base makes that demographic especially notable, as those users represent the most reliable source of revenue for the company.  

### Proposals for Additional Analysis
To further investigate the aforementioned hypothesis, equipping the potential investor with an even more detailed understanding of the CitiBike userbase, two additional visualizations are proposed.  First, the interactive maps might be coded in some way (introducing a third color along a spectrum, for instance) to indicate which starting and stopping locations are frequented by Customers versus Subscribers.  This could provide insights into which neighborhoods high-value Subscribers are more likely to live and work, which could be projected against exogenous geoddemographic data to extrapolate a more detailed picture of the subscriberbase than would be otherwise possibled using just the data provided in this dataset.  Second, a bar chart could be generated to show the average total of CitiBike bikes in active use for each hour of the day during the week.  It is vital for a company such CitiBike to time their employees' operations for retrieving and replacing bikes from the city so as to minimally impinge upon user rental time, requiring a detailed model of peak hours.     

