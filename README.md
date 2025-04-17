# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal of this project is to see if there is a relationship between bike availability at stations and the surrounding area. I chose to explore if there was a relationship between bike stations and restaurants as well as transit stations (bikes, trains).

## Process
### Step 1: 
Pull live data from CityBikesAPI from London. I made a dataframe and exported to a csv for the station name, location, and number of bikes at each station.
### Step 2:
Pull data from Foursquare and Yelp APIs to gather information about points of interest around those stations specifically restaurants and transit hubs. I explored the data to see which source was more useful for this exercise.

### Step 3:
Join the bike station data with the foursquare and yelp data and store it in a SQLite database. Perform EDA on the joined dataset using visualizations to start understand relationships and distributions of the data.

## Step 4:
Make a regression model to explore how different points of interest could predict the number of bikes available or being used at a station. 

## Results
Yelp returns more points of interest in London and provided more data per location (review counts, ratings). Foursquare covers a wider range of categories and responds more quickly when called. 

## Challenges 
I found working with APIs a bit challenging, particularly with Foursquare. I wasn't able to save my authentication keys in my local environment and then call them in the Jupyter notebook so will need to troubleshoot that in the future. I had no issues with the Citi bikes API every day I worked on it until today and then was unable to even connect to the website so I believe there's an issue with this API. At different points in the project I was able to get the information I needed from both Foursquare and Yelp but only at particular times and was not able to consistently call information. I also found it challenging to find what variable might be helpful to predict. I thought I was onto something by looking at transit stations (buses, trains) near bike stations, but that also yielded no useful relationship. 

## Future Goals
I'd first find out how to store my authentication key in my local environment. I think I'd keep trying different points of interest until I found a meaningful relationship and then would try to see if this relationship help across different cities. 





