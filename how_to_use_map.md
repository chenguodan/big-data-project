##How to use the Interactive map.

The final presentation of our analysis in the form of a website is hosted on Amazon Web Services at http://big-data-project-env-nwg6zhjxp8.elasticbeanstalk.com/. You may also find the source code for both the website and data analysis procedure at our Github repository.

There are two pages in the website, the overview page and visualization page. The first pages summarizes facts we found in taxi data with simple graphs and charts as presented in previous sections of this report. The visualization page is an interactive map with clickable region for each of the neighborhoods identifiable from the Zillow shape file. 

In default, when demo is off, user can choose weather, day of week and time of day, after which when a region is clicked, a histogram will show up representing distribution of trip counts for this region under the chosen conditions. For each such histogram, x-axis represents the counts of pick-ups and drop-offs combined, and y-axis represents how frequency of the counts historically under given conditions.

When demo is on, we use data for the last week of 2013 to show how we can detect regions with unusually high density of trips given day of week and time of day. For the chosen options, regions where trip densities are unusually high based on historical data of the same region with the same weather, day of week and time of day are plotted in blue. Button for choosing weather is disabled in this mode because once we have fixed the time period to be in the last week of 2013, weather is automatically determined based on time and location. 

Although the demo is for the last week of 2013 only, we could potentially use this functionality to detect regions with unusually high density of trips for any given time. This could be useful in finding usual events that cause people to gather in certain regions.
