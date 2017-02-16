# Spatio Temporal Visualization of Traffic Congestion in Delhi


[![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mindmap.png)](https://mm.tt/839687015?t=jSvOCBwlvc)

## Research Question
I want to carry out spatio-temporal visualisation of traffic flow in Delhi because I want to find out the extent of congestion being faced by different types of roads and areas in order to help the users analyse traffic congestion based on different parameters.


## Why are we talking about congestion?
- What, Why?
- Economic cost
- Traffic flow theory - An understanding in traffic flow theory is a necessity to understand and analyze traffic congestion.

##### References
 - The Hidden Cost of Gridlock on our Roads (link)
 - Traffic Congestion and Reliability: (link)
 - Traffic Flow Theory, Sven Maerivoet∗ and Bart De Moor (link)

## Congestion in Delhi
##### References
 - Why Delhi's decongestion plan will only increase congestion? (link)
 - Why Delhi's decongestion plan will only increase congestion? (link)
 - Growing congestion on Delhi roads likely to reduce speeds to 5kmph (link)
 - Decongestion Plan for Delhi (link)
 - Transport and land-use policies in Delhi (link)

## Spatial Representation: Why?
- Significance of spatial visualization - What spatial representation helps in? Why do we need it?
- Traffic congestion and spatial representation
- Existing research & Visualization

##### References
 - Visual Exploration of Spatial-Temporal Traffic Congestion Patterns Using Floating Car Data (link)
 - TIME: An open platform for capturing, processing and delivering transport-related data (link)
 - Congestion patterns of traffic studied on Nanjing city dual graph (link)
 - Mastering the Information Age Solving Problems with Visual Analytics (link)


## Congestion Analysis
#### Variables

##### Temporal
 - Day of the week
 - Time of day
 - Any special day/public holiday/ city level event

##### Spatial - Different type of land uses
 - School
 - Hospital
 - Residential
 - Commercial/Retail
 - Industrial

#### Analysis
  1. For different days, a timeline of congestion will be shown from which a particular day can be selected
  2. For a single day, another timeline is shown along with the ability to play that timeline using a slider. User can thus analyse where its getting more congested or less 
  3. The map showing the congestion for a particular timespan can be analysed further for
	1. Which parts are more congested?
	2. Bottlenecks can be highlighted automatically and can be studied
	3. Zooming in will show a congested area in detail which can be analysed for - 
		1. Different type of land uses at that place
		2. What all types of roads converge 
		3. For a particular area, the timeline of congestion at different times.
    
    
## Research/Visualization methodology
#### Data Sources
 - [OpenMapTiles](https://openmaptiles.org/schema/) - Provides high resolution vector tile set with different features.

 - [Google Map Directions API](https://developers.google.com/maps/documentation/directions/intro) - Service that calculates directions between locations using an HTTP request.

#### Data Collection
##### Fetch
Based on different road data that OSM provide, fetch travel time for each as per below logic
 1. Each day is divided into different hours.
 2. For each timespan one query is sent that returns travel time on basis of historical data and live traffic.
 3. the travel time along with information, like distance is stored

##### Manipulate
 - Once the data is collected over 3-4 weeks, calculate averages for days of week based on different values
 - Any outliers should be investigated (public holiday, any special city level event?)

##### Store
OSM Data to be combined with the traffic data

#### Data Visualization
 - Setup map to visualize for a particular timespan within a day.
 - Color scheme for different congestion levels.
 - Color scheme for different land uses.
 - Quantify congestion levels for a single timespan that can be displayed for a single day.


## Mocks
![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mocks/1.jpg)
![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mocks/2.jpg)
![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mocks/3.jpg)
![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mocks/4.jpg)
![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mocks/5.jpg)


## POC
[![PREVIEW](https://raw.githubusercontent.com/agaase/msdv-thesis/master/writing/mocks/POC.png)](https://www.mapbox.com/studio/styles/agaase/ciyytgl6a00302qo96ewqf74j/edit/)
