# Project Tour de France

In my project proposal, I identified the demand issue in Citi Bikes. In this MVP, I attempt to more concretely define the issue at hand and some potential solutions.

## Business Problem:

Citi Bike has seen explosive growth in ridership in the last few years that was further accelerated due to the COVID-19 pandemic. Due to this rising demand, I have seen many instances where stations often don't have bikes to take out or inversely don't have docks to park the bikes. These instances cause delays in people's lives as they have to involuntarily find a further than ideal station to use, which would reduce overall efficiency for each person's life. In the long run, repeated frustrations with this issue could result in more people losing faith in the system and resorting to some sort of vehicle transportation, which the city has been forthright about trying to reduce.      

## Impact Hypothesis:

I believe I can identify the stations that need more (or fewer) docks or in extreme cases, areas that need more stations. This would result in a more efficient use of the city's resources as the busiest stations would also require the most maintenance so the the city could proportionally manage its time. Users would clearly benefit not only from more seamless day to day use but also safety as well as maintenance is directed more accurately. 

## Data:

I downloaded the entire set of ride data of September 2021 from Citi Bike's website. I used pandas to gather more meaningful information about each station's location such as neighborhood, borough, and zip code. Unfortunately due to its size, I was only able to take a 5% sample to import into Excel. An assumption I must make is that this random sample is representative of the entire dataset.   

## Solution Paths:

An immediate issue I see from the dataset is that there is no information on how full or empty the dock is when a bike is used. Thus I have to figure out the classification issues of full/not full when attempting to dock and empty/not empty when attempting to use bikes. A less data science solution path would be to assume the trends of increased ridership continue and add incrementally more docks and bocks to every station.  

## Visuals:
![image](https://user-images.githubusercontent.com/89528655/137046155-93a637ac-417c-4173-be95-1f913ccdcdfa.png)

I've taken an initial stab to see which neighborhoods are most popular to start rides at. I attempted a bar chart on a station level but there were far too many columns. Unfortunately, my data acquisition wasn't perfect as some neighborhood names are missing. After mapping these names more descriptively, I think analyzing these trends with those of most popular neighborhoods to end rides is my best bet to make meaningful recommendations to Lyft/City of New York. 

## Next Steps/Concerns:
- I need to better map neighborhood names as stated previously. I'm a bit concerned however that since neighborhoods are not officially designated this could present quite a challenge. 
- How can I define success in terms of a clear, quantifiable goal?
- I've identified the classification issue but that is not something I'm currently equipped to handle. 
- What exactly is my stopping point? Having trouble delineating between Results and Conclusions.  
