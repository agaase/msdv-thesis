
## Wasted Time : Travel in Delhi

Analyse the time being wasted in Delhi in terms of road transport within the city. “Wasted” is used here to signify the excess time people spend while travelling from one place to another due to traffic or congestion. The project visualizes the same; both, at a macro level understanding patterns across the city and micro level for a particular area.

This topic is more of a personal interest to me. I have been myself frustrated by the traffic congestion in Delhi and wanted to analyse what is happening. At some point acknowledging the facts and making people aware about it is important. With this project I want to do the same and also at the same time develop a research tool to assess and analyse the situation.

There are different variables on which this project can further be studied upon like the day of the week, time of the day, different types of areas through which one can filter and get a filtered perspective.  As such there are many important questions that I aim to address such as - 
- Which areas take more time to travel in the city and hence more critical?
- For different distances what is the excess time ?
- Is there an extreme variation in travel time based on time of the day or day of the week?
- How does the situation looks like for different areas like schools, hospitals, commercial areas?
- What does the situation look like for a particular area?

But, what is the value of this type of analysis? There are several important real life problems that can be addressed by this visualization.
- Criticality - We are identifying areas which face excess time and also how much of it which gives an indication as to how critical is that area to receive attention.
- Field of movement - urban traffic is more than just the share of people coming in and out during their office hours. Analysis of areas which take more time to travel could give an indicaton to the type of travel happening.
- Bottleneck  - When we do analysis at a micro level, trying to understand if there's an extreme variation at different distances we could identify bottlenecks.

Iam working with different types of data collection and manipulation tools for this project. 
- OSM data provides the GIS mapping of different types of landuses. 
- Google Directions API provides for travel time between two points on a map
- QGIS allows for bounds calculation and identify and fix any missing GIS pieces.
- turfjs allows for geo spatial analysis
