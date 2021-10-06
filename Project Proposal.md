# Citi Bike Resource Deployment

## Question
Citi Bike is a public bicycle sharing system in NYC serving Manhattan, Brooklyn, the Bronx, Queens, and Jersey City and Hoboken in New Jersey. During the pandemic, the city has seen an unprecedented rise in ridership as the COVID-19 pandemic has convinced many to turn to alternative means of transport. With this rise, however, comes increased maintenance costs as well as greater demand. This demand issue is what I will be looking to solve. Specifically, I will be looking to balance the number of bike docks there are in a given station based on volume and traffic patterns. The recommendations in the most basic form would be to add docks to some stations while removing some from others. In some cases, the data may indicate an entirely new station is necessary. This project would most directly benefit riders, who would less often be faced with a full dock when attempting to dock their bikes.  

## Data
I will be looking at ridership data which Citi Bike publicly provides in csv format online. Each file shows every ride taken over the course of a month. Each line shows the time and location of the start and end of a single ride as well as whether the rider was a member or one-off user. One piece of information this file doesn't provide is how many docks there are per station. If it is obtainable, this would be added to the larger dataset. I initially aim to explore which stations are most and least popular and then take a deeper dive into figuring out a way to determine when docks are full. This should be easier if the number of docks is available but possibly approximated based on timestamps as well. In addition to determining when a dock is full, I may want to get a sense of how many bikes are being used at different times of the day. With more time, it may be interesting to look at residency and work population data and cross-reference with dock locations to see how many people live/work within a certain block radius of a station.   

## Tools
I intend to mostly use Excel for EDA but may have to go to SQL if the data ends up being too cumbersome. I will use Tableau for visualization. I don't anticipate needing other tools (besides SQL possibly) at this time.  

## MVP Goal:
My MVP should have the most popular stations, potentially parsed by day of week or time of day. It may or may not have a framework to determine when/how often docks are full.  
