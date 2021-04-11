# FordGo-Bike-Analysis

**FORDGO BIKE: RIDE ANALYSIS**

* Introduction:

    * Bay Wheels, known as FordGo bikes for a brief period, is a regional public bicycle sharing system in California’s San Francisco Bay area. It was established in August 2013.
    * In September 2016, Ford announced that its sponsorship with Bay wheels and on June 28, 2017, they renamed the company to Ford GoBike. In June 2019, after its acquisition by Lyft the system was rebranded to Bay Wheels and they dropped the Ford naming.
    * As of January 2018, the Bay Wheels system had about 10,000 annual subscribers, over 2,600 bicycles in 262 stations across San Francisco, East Bay and San Jose.
The data analyzed below is of February 2019. 
    * The source of the data is udacity.The dataset has 16 columns and 1,83,412 rows, which means approximately 1,83,000 rides were made during that month.
    * The original columns of the data set are as follows:

        * duration_sec: duration for which bike is rented in seconds
        * start_time: Date and time on which the bike was rented
        * end_time: Date and time on which the bike was dropped
        * start_station_id: Station ID from where the bike was rented
        * start_station_name: Station name from where the bike was rented
        * start_station_latitude: Latitude of the station from where the bike was rented
        * start_station_longitude: Longitude of the station from where the bike was rented
        * end_station_id: Station ID where the bike was dropped
        * end_station_name: Station name where the bike was dropped
        * end_station_latitude: Latitude of the station where the bike was dropped
        * end_station_longitude: Longitude of the station where the bike was dropped
        * bike_id: ID of the bike rented
        * user_type: Customer or subscriber
        * member_birth_year: Birth year of the rider
        * member_gender: Gender of the rider
        * bike_share_for_all_trip: yes/no

**Questions analyzed are as follows:**

* Which are the most popular pick up and drop off stations?
* At what time of the week, the demand for the bike is at the peak? For how much time do they ride the bike on an average?
* At what time of the day there are maximum number of riders? For how much time do they ride the bike on an average?
* How much percentage of the riders are subscribers and how much percentage of them are customers? Note: riders can either be subscribers on they can rent it on adhoc basis

**Limitations:**

* The data analyzed is only for one month. Demand for bike is largely impacted by the weather mainly rain, heat and cold. Rain is the most adverse weather for riding bikes. Hence, it might be a good idea to have the weather data along with this.

**Data Extraction:**

* Downloaded from Udacity

**Data Cleaning/Feature Engineering:**
* Removed nulls
* Updating Data Types

**Exploratory Data Analysis:**
* Reviewed the dataset
* Flitered records and null values review
* Data Visualization for final findings
* Created maps, barcharts and pie charts to answer various questions

**Code and Dataset Details**
* Python Version: 3.6.3

* Packages: pandas, numpy, folium, matplotlib, datetime

**Main Findings:**

* Market Street at 10th St., San Francisco caltrain station2, Berry Street at 4th Street are few of the most popular pick up stations in San Francisco, where the bikes picked up are more than 3000 per month. These stations are located in the heart of the city and they are well connected to other parts of the city through trains, buses or freeways.
San Francisco Caltrain station2, Market Street at 10th St., Montgomery Street BART Station are few of the most popular drop-off stations in San Francisco with drop off more than 3500 per month. These stations are located in the heart of the city and they are well connected to other parts of the city through trains,buses or freeways.
* The demand for the bikes is highest on Thursday totalling to approximately 35,000 per month.
The bike is rented for higher minutes in weekend as compare to weekdays. On an average bikes are rented for 15 minutes on weekend.
* -The demand for the bike is highest between 8 and 9 AM and between 5 and 6 PM. The average duration of the bike rented during this time is 11 and 12 minutes respectively. It seems that these bikes would be rented mainly for commuting purposes.  The bike is rented for maximum amount of time which is almost 25 minutes between 3 AM and 4 PM. It might be a good idea to look at the data in the detail and consider whether this is one of the events or it's a routine thing.
* Almost 89% of the renters are subscribers. It seems that they would be using bike regularly.
