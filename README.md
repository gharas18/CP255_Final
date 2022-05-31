# Transit Oriented Development: Accessibility & Health Vulnerability

**Authors:** Gregory Harasym, JP Zeigler

## Problem Statement
I will be exploring the potential long-term health impacts of transit-oriented development being situated adjacent to freeways in the Bay Area. TOD is a means to increase density and reduce our carbon-footprint through the encouragement away from auto-centric mobility and towards public transit. Due to the nature of BART being directly parallel to a large portion of highway infrastructure, a portion of TOD projects in the Bay will essentially be subsidizing market rate and low-income people to live adjecent to freeways, which have higher concentrations of particulate matter exposure and can lead to asthma and other respiratory complications.

Specifically, I will be concentrating on the distribution of PM2.5 data in the Bay Area. Research has shown that short-term exposures (up to 24-hours duration) of PM2.5 have been associated with premature mortality, increased hospital admissions for heart or lung causes, acute and chronic bronchitis, asthma attacks, emergency room visits, respiratory symptoms, and restricted activity days. This pollutant will be the primary evaluating factor I will be focusing on to determine the ideal eucledian distance for TOD's from freeway adjacent BART stations.

![Screen Shot 2022-05-05 at 9 19 02 PM](https://user-images.githubusercontent.com/82476483/167476249-f703a9f7-dacf-4017-ad8f-4b42b07a45a4.png)

### Goal
A goal of this project is spatially analyzing various sources of health, pollution, and transit data. I will explore the ideal euclidian distance of housing from freeways (and BART stops) that limits health impacts and maximizes mobility and accessibility. BART TOD grants currently incentivize placement of residential complexes within 1/2 mile radius from BART stop locations; however, it is common practice to develop TOD's directly adjacent to the station. A major component of TOD's is to increase accessibility, which will hopefully discourage individual car use and thus reduce pollution effects. I will be using walkshed time and distances to evaluate the proximity of three TOD locations (Balboa Park, MacArthur Commons, & Antioch) to both freeways and their relative proximity to PM2.5 concentration. I will be using 300', 500', 1000' walkshed distances from each TOD location because California has established those distance thresholds as being the most to least vulnerable in terms of exposure to PM2.5 near freeways. California currently has laws in place that restrict development of new schools within 300' of highways, but no such laws exist for housing, community centers, or day care centers.

## Bay Area Pollution PM2.5 Concentration

From the figure below, it appears that Oakland has the highest concentration of PM2.5 in the Bay Area. The PM2.5 data is aggregated on a census block level, which can misrepresent the actual concentrations of "hot zones". I attempted to normalize the data by square area of the census block polygons, but there was little variation among PM2.5 concentration which created a uniform choropleth map. For that reason, my PM2.5 data below will not be normalized by area. Areas in the South Bay appear to have the lowest levels of concentration of PM2.5 and Oakland appears to have the highest concentrations.

<img width="904" alt="Screen Shot 2022-05-08 at 5 17 39 PM" src="https://user-images.githubusercontent.com/82476483/167321810-3b7d8e94-8215-4f32-9f4f-8cdcb5005efc.png">

### Spatial PM2.5 Distribution Curve

The figure below shows the kernel density plot for the 5 county distribution of PM2.5 levels. Contrary to the spatial choropleth map, San Francisco appears to have the highest concentration from a normal distribution perspective. 

<img width="1011" alt="Screen Shot 2022-05-09 at 4 23 12 PM" src="https://user-images.githubusercontent.com/82476483/167514139-611cdd53-6594-4699-80f2-9b04ed7d397f.png">


### Map of Study Area
The map below shows our study area and highlights the three TOD sites, along with the parallel BART lines. The coordinate reference system was projected to ESPG:3310 and the TOD locations were geocoded using the code below. 

<img width="1014" alt="Screen Shot 2022-05-09 at 4 26 29 PM" src="https://user-images.githubusercontent.com/82476483/167514442-7ba07140-8e31-41f4-aa09-5280f4abf1f9.png">

<img width="1047" alt="Screen Shot 2022-05-09 at 4 27 03 PM" src="https://user-images.githubusercontent.com/82476483/167514486-0b709e1a-8116-48be-b090-2bdcc367413a.png">

## Balboa Park Site Analysis (San Francisco)
In this section, I will be exploring various walksheds time and distances and contrasting them with existing TOD site locations, PM2.5 concentrations, and freeways.

### Baboa Park Walkshed distances from centroid of TOD location - 5, 10, 15, 20 Minute Intervals
<img width="1126" alt="Screen Shot 2022-05-09 at 4 55 18 PM" src="https://user-images.githubusercontent.com/82476483/167516974-be83ba73-6b27-483d-83f8-20225d56bb3d.png">

### 300' Walkshed Distance from Balboa Park TOD - Normalized by sq area
<img width="1042" alt="Screen Shot 2022-05-09 at 5 00 04 PM" src="https://user-images.githubusercontent.com/82476483/167517141-061c2ee6-31cb-40dd-b794-aa6a6557e0b8.png">

### 500' Walkshed Distance from Balboa Park TOD - Normalized by sq area
<img width="1019" alt="Screen Shot 2022-05-09 at 5 05 16 PM" src="https://user-images.githubusercontent.com/82476483/167517533-f1672c6e-c70e-4d27-8f7c-c942a233b3a3.png">

### 1000' Walkshed Distance from Balboa Park TOD - Normalized by sq area
<img width="1033" alt="Screen Shot 2022-05-09 at 5 06 03 PM" src="https://user-images.githubusercontent.com/82476483/167517585-a83cd749-bd50-46cc-97f8-80725aee065b.png">

## MacArthur Commons Site Analysis (Oakland)
In this section, I will be exploring various walksheds time and distances and contrasting them with existing TOD site locations, PM2.5 concentrations, and freeways.

### MacArthur Commons Walkshed distances from centroid of TOD location - 5, 10, 15, 20 Minute Intervals
<img width="954" alt="Screen Shot 2022-05-09 at 5 33 34 PM" src="https://user-images.githubusercontent.com/82476483/167519822-09a6e49d-a704-4a1a-bd48-a7ac0939ef6a.png">

### 300' Walkshed Distance from MacArthur Commons TOD - Normalized by sq area
<img width="1049" alt="Screen Shot 2022-05-09 at 5 34 07 PM" src="https://user-images.githubusercontent.com/82476483/167519864-fe57df4b-c212-45b9-8746-78c16954b4f5.png">

### 500' Walkshed Distance from MacArthur Commons TOD - Normalized by sq area
<img width="1050" alt="Screen Shot 2022-05-09 at 5 34 34 PM" src="https://user-images.githubusercontent.com/82476483/167519907-b81c8005-faca-47e6-9aff-63298efbd29b.png">

### 1000' Walkshed Distance from MacArthur Commons TOD - Normalized by sq area
<img width="1041" alt="Screen Shot 2022-05-09 at 5 35 29 PM" src="https://user-images.githubusercontent.com/82476483/167519972-b0158908-9246-471f-bbd2-3c9f82e23fb0.png">

## Antioch Site Analysis
Obtaining data on Antioch was a bit more difficult than the other site analysis. Specifically, I could not locate a highway network geojson file for Antioch. Additionally, the Antioch TOD location is more spatially distant from the highway and BART location, which reduces the effectiveness of creating a 300, 500, and 1000' walkshed distance from the TOD centroid location. For those reasons, I am only reporting the below results that show the concentration of PM2.5 in the city of Antioch (normalized by sq. mile) and the 5-20 minute walk intervals. 

### PM2.5 Concentrations Antioch
<img width="881" alt="Screen Shot 2022-05-09 at 5 37 18 PM" src="https://user-images.githubusercontent.com/82476483/167520127-0ac8c9fc-aeaf-4085-b746-cc66c9d07d7f.png">

### Antioch Walkshed distances from centroid of TOD location - 5, 10, 15, 20 Minute Intervals
<img width="1083" alt="Screen Shot 2022-05-09 at 5 42 17 PM" src="https://user-images.githubusercontent.com/82476483/167520493-252091ba-3022-4fc3-8b5d-aa3bdb61ba36.png">


## Additional Implications
New developments in California are required to dedicate a percentage of new units to be "affordable". People applying for affordable housing enter a lottery system and are chosen based on priority preference, but are subject to availability. MacArthur Commons and Antioch have approximately 30% of units dedicated as affordable housing units, and Balboa is intended to be 100% affordable. Research has shown that people who are placed at TOD locations utilize BART less frequently than market-rate units who buy into the building. Lower-income residents often have differing transportation needs that require non-linear modes of rail transit. BART is a primary commuter rail system that does not service all areas of the Bay that people may need to commute and travel to. For health and mobility reasons, it is important to think of the implications of obligating lower-income residents to freeway adjacent TOD locations. 

## Conclusion
Based on existing literature, TOD site locations should be at a least 500' from adjacent freeways. California faces an unprecedented housing crisis, but special attention should be placed on where desity is being relegated to. BART increases accessibility for select Central Business District commuters, but with the increase in telework procedures, commute and travel patterns may be changing. Densifying neighborhoods where multi-modal transportation alternatives exist, rather than focusing on BART proximity, may produce more sustainable and healthy outcomes for residents.

## Future Considerations
Future work may include looking into a comparison of prior planning decisions that led to in-equitable health outcomes to lower-income and minority populations. Additionally, I may consider analyzing the level of pollution based on permissable freight routes on highways to see if there is any correlation or areas of concern that are adjecent to proposed BART TOD sites. I will attempt to attain PM2.5 data on a more granular level because the aggregated census block data can be missleading. Also, I will attempt to build a more robust transit accessibility network to better assess which locations may be better suited to serve lower-income residents.




