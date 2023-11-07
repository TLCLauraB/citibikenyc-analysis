<img src="https://github.com/TLCLauraB/citibikenyc-analysis/blob/main/images/CitiBike-Logo.png" width="200" align="center">

CitiBikeNYC Through the Pandemic: Looking at August 2019, 2020 & 2021<br/>
Presented by Laura Bishop (TLCLauraB)<br/>
Tableau-Public Link: [Module 18: Citi Bike Data Analysis](https://public.tableau.com/views/Module18_CitiBikeDataAnalysis-Final/StoryMod19CitiBikeNYCAnalysis?:language=en-US&:display_count=n&:origin=viz_share_link)<br/>

# Introduction:

<img src="https://github.com/TLCLauraB/citibikenyc-analysis/blob/main/images/CitiBike-1.png" width="300" align="left">

In August of 2019, little did we know that a global health crisis was only eight months away, poised to alter the course of our lives in profound ways. Our daily routines, from commuting to work to enjoying leisurely bike rides, were soon to be dramatically affected. The world was on the brink of an unforeseen challenge that would force us to adapt, innovate, and come together as a global community in the face of the COVID-19 pandemic, forever changing how we live and interact with our surroundings.

Using the information provided by [CitiBikeNYC](https://citibikenyc.com/homepage), I analyzed data from August of 2019, 2020 and 2021. I set out to address several questions:

  * How many trips were recorded in Aug 2019, Aug 2020 and Aug 2021?
  * By what percentage did ridership grow (if at all) from Aug 2019 to Aug 2020 to Aug 2021?
  * What is the average distance in miles for a bike trip in Aug 2019, Aug 2020 and Aug 2021?
  * Did the proportion of "annual subscribers" change from Aug 2019 to Aug 2020 to Aug 2021?

## Data Clean Up:
Between August of 2020 and August of 2021, several data formats were updated to better suit CitiBikeNYC's needs. To incorporate both sets into my analysis, I had to convert several text entries to 0=Customer, 1=Subscriber before reunifiying them, as well as normalizing Station Lat/Long to work with individual Station Latitude and Longitude geo-measurements. 

<ins>Data Format for August of 2019 and 2020:</ins>
* Trip Duration (seconds)
* Start Time and Date
* Stop Time and Date
* Start Station Name
* End Station Name
* Station ID
* Station Lat/Long
* Bike ID
* User Type (Customer = 24-hour pass or 3-day pass user; Subscriber = Annual Member)
* Gender (Zero=unknown; 1=male; 2=female)
* Year of Birth

<ins>Data Format for August of 2021:</ins>
* Ride ID
* Rideable type
* Started at
* Ended at
* Start station name
* Start station ID
* End station name
* End station ID
* Start latitude
* Start longitude
* End latitude
* End Longitude
* Member or casual ride


## Analysis: Maps & Station Trends:

While trip count remained almost the same from August of 2019 (pre-pandemic) to August of 2020 (6 months into the pandemic), we can see a significant jump in ridership from August of 2020 to August of 2021 (6 months after the initial outbreak, 9 months after the first vaccines were announced). Focus seemed to shift from Upper Manhattan to central-and-lower, including Hell's Kitchen, the High Line, Greenwich Village, and Soho/Lower Manhattan.

## Analysis: Casual Customer to Service Subscriber:

While there was a rough 10% drop in service subscribers to casual customers between August of 2019 and August of 2021, the overall total of ridership for the CitiBikeNYC service increased by almost 500,000 individual trips. Also, while the average trip distance in August of 2019 was under 1 mile, by August of 2021, the average had risen to 2 miles.

## Resources:
[CitiBikeNYC - Index of bucket "tripdata"](https://s3.amazonaws.com/tripdata/index.html)
  * 201908-citibike-tripdata.csv
  * 202008-citibike-tripdata.csv
  * 202108-citibike-tripdata.csv
