## How is Airbnb really being used in and affecting the neighbourhoods of your city?

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

My first static map is of median rents in New york city to have a better idea about how rents are divided around NYC.


Here is my sample web map

<iframe src= "Airbnb_chloropeth_map.png" height= "900" width= "95%"></iframe>

