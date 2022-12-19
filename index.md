## How is Airbnb affecting Rental Market in New York City?

# Marziya Farooq- Command Line GIS
# Final Project

# Introduction
Airbnb claims to be part of the "sharing economy" and disrupting the hotel industry. 
However, data shows that the majority of Airbnb listings in most cities are entire homes, many of which are rented all year round - disrupting housing and communities. 
Community groups and housing advocates in cities across the world have begun to sound the alarm about Airbnb’s impact on affordable housing in their communities, citing
concerns about housing supply lost, racialized gentrification, and impact on residents’ quality of life.

DATA CONCERNS
For the project, I tried to understand that how airbnbs disrupts the rental market and if they have any connection to evictions and rental market.
I found airbnb data for 2019 using inside Airbnb, a website that tracts Airbnb data all over the world to understand and inform about Airbnb's impact on residential communities.
I found eviction data for new york from NYC open data. I used census tract data from IPUMS which provides census and survey data from around the world integrated across time and space
I used IPUMS because it allowed me to get clipped census tract so I didn't have to clip it myself. The eviction data was updata in 2021 but i used 2019 so I could collaborate it better with airbnb
I also used census tract data for total housing and median rents in New York from census data (2016-2020 ACS survey). I also Black population data from ACS census survey (2019-2020) from Census data

Most of the data was in CSV format except the census tract files which were in shape format. for census data, I joined it normally. 
For eviciton and airbnb, I joined it used spatial join and aggregation and I created centroids of it. 
I had to clean quite abit of the data because there were null value and infinite values and some low-relaiability values.

My first static map is of the density of airbnb around NYC. I normalised airbnb data with total number of housing to get a better and more accurate version or airbnb density. My second static map is of median rents in New york city to have a better idea about how rents are divided around NYC. the two maps side by side do a good job of showing how airbnb density and rents correlate with each. increase rents are in areas where the airbnb density is high.


## Static Maps:
<div style="display: flex;">
  <img src="Median Rents in NYC (1).png" style="width: 50%; height: auto;">
  <img src="Arbnb Chloropleth map.png" style="width: 50%; height: auto;">
</div>


I also an interactive plotly map to show how airbnb is distrbuted using the price per night. this can be seen in junction to the rents and it is easy to see that in areas where rents are, airbnbs prices are also high. mostly because it is manhattan where living costs are extremely high.This shows the how the airbnb in newyork city are distrbuted with price, with the cheapest being 20 per night and the most expensive being 10,000 dollars per night.


## AIRBNB PRICE

<iframe src= "map.html" height= "855" width= "95%"></iframe>



Finally, I wish to show my interactive webmap which shows 3 layers. the first is the chloropleth layer than i also created a static map. I wanted to use that in my folium so that I could show how my map looks on folium. I overlaid the map with eviction data using proportional symbols to have a better idea of the relationship between evictions and airbnb density. Finally I created a cluster map of airbnb data
I used only manhattan because the folium kept crashing when i tried to map the point data for the whole of new york as it was too many points (more than 40,000).

## AIRBNB AND EVICTIONS


<iframe src= "Airbnb_Data.html" height= "855" width= "95%"></iframe>
