![Header](/pics/header.png)

#### Table of Contents

[Project Overview](#project-overview)  
[Resources](#resources)  
[Objectives](#objectives)  
[Summary](#summary)   
[Challenge Overview](#challenge-overview)  
[Challenge Summary](#challenge-summary)   

## Project Overview
In this module, we used the Leaflet.js Application Programming Interface (API) to populate a geographical map with GeoJSON earthquake data from a URL. Each earthquake was visually represented by a circle and color, where a higher magnitude has a larger diameter and is darker in color. In addition, each earthquake has a popup marker that, when clicked, shows the magnitude of the earthquake and the location of the earthquake. 

## Resources
We used the Leaflet library to plot the data on a [Mapbox map](https://www.mapbox.com) through an API request and created interactivity for the earthquake data. We added the USGS URL for earthquake data by navigating to the USGS Hazards Program, clicking the Earthquakes link to open the Real-time Data Feeds link and scrolled down to "GeoJSON Summary" Feed. There, we clicked the [All Earthquakes](https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_week.geojson) link under the “Past 7 Days” heading

- **Data Source:** [majorAirports.json](/majorAirports.json), [torontoRoutes.json](/torontoRoutes.json), [torontoNeighborhoods.json](/torontoNeighborhoods.json)
- **Software:** JS, D3, Leaflet  

## Objectives 
- Create a branch from the master branch on GitHub.
- Add, commit, and push data to a GitHub branch.
- Merge a branch with the master branch on GitHub.
- Retrieve data from a GeoJSON file.
- Make API requests to a server to host geographical maps.
- Populate geographical maps with GeoJSON data using JavaScript and the Data-Driven Documents (D3) library.
- Add multiple map layers to geographical maps using Leaflet control plugins to add user interface controls.
- Use JavaScript ES6 functions to add GeoJSON data, features, and interactivity to maps.
- Render maps on a local server.

## Summary  
### logicStep1.js
[logicStep1.js](/Earthquakes_past7days/static/js/logicStep1.js) maps all recorded earthquakes in the past seven days.  
<img align="left" width="550" src="/pics/step1.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
### logicStep2.js  
As a first step in making the earthquake data more visually appealing, we added some styling to the earthquake data in [logicStep2.js](/Earthquakes_past7days/static/js/logicStep2.js) and varied the radius of each earthquake based on the magnitude.  
<img align="left" width="550" src="/pics/step2.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
### logicStep3.js  
Although, the size of the earthquake data based on magnitude looks great, it’s hard to tell the difference between earthquakes within the same area. We come up with the idea to color-code the earthquakes based on magnitude. We, also, added the magnitude and location as a popup for each earthquake in [logicStep3.js](/Earthquakes_past7days/static/js/logicStep3.js).  
<img align="left" width="550" src="/pics/step3.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
### logicStep4.js
[logicStep4.js](/Earthquakes_past7days/static/js/logicStep4.js) has the earthquake data as an overlay on both the Streets and Satellite tile layers, so users can turn the data on and off.  
<img align="left" width="550" src="/pics/step4.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
### logicStep5.js  
The final piece we added to the map is in [logicStep5.js](/Earthquakes_past7days/static/js/logicStep5.js): a legend for the color range of the earthquakes. A legend provides information needed for the colors of the earthquakes to make sense to the viewer without having to click on each marker.
<img align="left" width="550" src="/pics/step5.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
## Challenge Overview  
In this challenge, we added a third map style as an additional tile layer. We ,also, added tectonic plate GeoJSON data to the map to illustrate the relationship between the location and frequency of seismic activity and tectonic plates.To illustrate the severity of the earthquakes in relation to the tectonic plates, we logged in to GitHub and accessed the tectonic plate data from this [GitHub repository](https://github.com/fraxen/tectonicplates). We, also, made an API call to the tectonic plate data using d3.json(), and then added the data as an overlay to the map using the L.geoJSON() layer. In addition to the streets and satelliteStreets maps, we added a third map style of our choosing. All map styles were added to the base layer so that they showed up on the map to allow the user to change which layers are visible.

## Objectives
- Use d3.json() to get tectonic plate data and add the data using the L.geoJSON() layer.
- Style the tectonic plate LineString data to stand out on the map.
- Add the tectonic plate data as an overlay with the earthquake data.
- Add a third map style to allow the user to select from three different maps.

## Challenge Summary
<img align="left" width="290" src="/pics/street.png"><img align="left" width="290" src="/pics/satellite.png"><img align="left" width="290" src="/pics/dark.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<img align="left" width="290" src="/pics/quakes.png"><img align="left" width="290" src="/pics/plates.png"><img align="left" width="290" src="/pics/none.png">
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">
  <img width="900" src="/pics/street.png">
</p>
  


