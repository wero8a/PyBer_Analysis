# PyBer Analysis Report

## Overview
  The purpose of this report is to analyze Pyber's ride share data and create a summary DataFrame  to inform the CEO, V. Isualize, with the best analysis possible. We will use this DataFrame to create a graph that demonstrates how the data differs by city type and how these differences will affect V. Isualize's decision making on PyBer moving forward.
  
## Resources
- Python 3.7.13
- conda 4.14
- jupyter_client 6.1.12
## Results
The image below demonstrates the summary DataFrame for our analysis. 

![image](https://user-images.githubusercontent.com/110706169/190729821-e2ec3838-9365-465a-ad2a-183d236b0907.png)

From this summary we can depict that:
- Urban cities have the most total fares, drivers, and rides.
- Rural cities have the least total fares, drivers, and rides.
- Suburban cities are in between.
- The average fares in rural cities is considerably higher than the rest 
- The average fares in urban cities is considerably lower  than the rest

To get these values we used the *groupby()* function to set the index as city types and return all the data we need. For instance, to calculate the total rides for our summary DataFrame we used:

![image](https://user-images.githubusercontent.com/110706169/190734592-6d9143b0-037d-45b8-ad73-3532f9c6b820.png)

We did the same to find the total drivers and total fares. To get the averages we simply divide Total Fares by Total Rides and Total Fares by Total Drivers.

![image](https://user-images.githubusercontent.com/110706169/190749341-8757f387-e9ad-49f3-8c33-7f52e2409376.png)

![image](https://user-images.githubusercontent.com/110706169/190749841-615be79a-da70-4dfc-b3aa-09cac25090b7.png)

The image below demonstrates the differences in **Total Fares** by city type in **Urban, Suburban, and Rural cities** across 5 months(Jan - May) in 2019.

![image](https://user-images.githubusercontent.com/110706169/190732100-dd59cca8-704f-46f6-ba45-3aa2d42f3f09.png)

From this graph we can depict that:
- Urban cities **Total Fares** min was around $1,700 in early January
- Urban cities **Total Fares** max reached close to $2,500 in February and March.
- Suburban cities **Total Fares** min was around $700 in early January.
- Suburban cities **Total Fares** max was around $1,400 in February.
- Rural cities **Total Fares** min was around $100 in January and February.
- Rural cities **Total Fares** max was around $500 starting April.

## Summary
Over these 5 months the trend seems to stay consistent; in order to improve Pyber usage in rural areas, changes must be made.
1. Prices per ride are much greater in rural areas and they also have the least amount of drivers.

![image](https://user-images.githubusercontent.com/110706169/190774468-7569034b-3d83-4ca2-9253-8ec05b7efe27.png)

The image above shows the average rides per driver in all 3 city types. If profits from Urban **Total Fares** can be funneled into driver compensation for Rural Drivers then they can charge less per ride while not affecting their current income. This should increase Pyber popularity over time in rural cities.

2. Usually, people from urban cities have access to better salaries. We should set a minimum price for rides to increase the **Average Fare per Ride**. People might not care too much to pay a little extra. This can facilitate our first recommendation.

3. Decrease price per mile un rural areas. It is extremely inconvinient to catch a ride in a rural area when a small trip can cost you $35. Locals might prefer to ride a bike around instead.
