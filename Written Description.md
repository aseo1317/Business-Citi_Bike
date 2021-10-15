# Project Tour de France
Andrew Seo

## Abstract
Citi Bike has seen explosive growth in ridership in the last few years that was further accelerated due to the COVID-19 pandemic. I myself, after 7 years in NYC, took my first Citi Bike ride in the summer of 2020 due to fear of taking public transport. Since I started, I have barely taken any other forms of transporation. I'm not the only one as the system has already surpassed all of last year's record breaking total and daily rides are over 100,000. NYC Department of Transportation and Lyft (owners of Citi Bike) have announced many expansion plans over the last year but the rising demand seems to be outpacing them. I attempted to find some insights and make recommendations by taking a deep dive into the monthly ride data provided by Lyft. I used pandas in Python and Excel for EDA and Excel and Tableau to visualize my findings. 

## Design
I will be addressing the NYC Department of Transportation as I have identified the Citi Bike as needing improvement. Specifically, my first hand experience has led me to the business problem of insuffiencet dock space or bike availability at certain stations. These situations lead to inefficiency for each individual and potentially in the long run, users abandoning the system. I believe by identifying the most trafficked stations, I can make informed recommendations of adding docks/bikes to specific stations at specific times either through moving docks from stations that need them less but preferably through overall capacity increases. This would increase efficiency for the department as these stations would likely be the ones requiring the most maintenance. The end result would be a safer and more satisfied userbase and greater usage, which is in line with the city's goal to reduce car traffic. The way I would frame this pitch is that while I recognize DoT and Lyft are making some efforts, resources needed to be better directed or just more resources are needed in general 

## Data
The original dataset came from the Citi Bike website, where I downloaded all of September's ride data. Because each row represented a single ride, the dataset was over 3 million rows and contained the start and end station, time, and geographical latitude/longitude coorindates. I also used Geopy to find the boroughs, neighborhoods, and zipcodes of the start and end stations. This was too large a dataset to analyze in Excel so I took the top 10 stations from where rides were started and analyzed this subset.

## Algorithms

_Data Acqusition and EDA in pandas_
1. Loaded in csv file and looked at dataframe, types of columns, and dealt with null rows (removed them in this case)
2. Used geopy and coordinates given to gain further information about the stations. 
3. Merged neighborhood, borough, and zip code info into main dataframe
4. Made further adjustments to neighborhood names by mapping zip code to neighborhood. 
5. Grouped by top ten stations where rides started
6. Used these stations and created a mask to download ride data on only these ten stations

_Tableau_

Most of the EDA and visualization done in Tableau and Excel is straightforward except for the map overlay in Tableau
1. Drag latitude (generated) and longitude (generated) in rows and columns
2. Copy latitude (generated) again to show two identical maps next to one another
3. To the bottom graph, add Zip Code into Detail pill and count of rows to color pill.
4. Change latitude (generated) associated with botom graph to dual axis

## Tools
- Citi Bike website for initial dataset and factoids about the system
- Pandas for further data acquisition and initial EDA 
- Excel for further EDA and some visualizations
- Tableau for more visualization

## Communication
Presentation of findings attached to this written description. This includes visualizations and conclusions.
Python notebook, Excel notebook, Tableau worksheet also attached for further insights that didn't make it into presentation. 
