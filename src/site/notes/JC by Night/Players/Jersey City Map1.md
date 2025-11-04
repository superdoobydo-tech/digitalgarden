---
{"dg-publish":true,"permalink":"/jc-by-night/players/jersey-city-map1/"}
---


> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`



```leaflet  
id: JersyCityMapplayer ### Must be unique with no spaces  
image: [[Jersey City Map1.png]] ### Link to the map image file. Do not add a ! in front of the image  
bounds: [[0,0], [2159, 2692]] ### Size of the map in px Height_y, Width_x. Ignore 0,0  
height: 850px ### Size of the leaflet embed in px on your screen  
width: 95% ### Size of the leaflet embed in your note  
lat: 1079.5 ### To center the map, make this half of the map height.  
long: 1346 ### To center the map, make this half of the map width.  
minZoom: -2 ### Controls how far away from the map you can zoom out. Hover over the target icon to see the current level.  
maxZoom: 1 ### Controls how far towards the map you can zoom in. Hover over the target icon to see the current level.  
defaultZoom: -1.5 ### Sets the default zoom level when the map loads. Hover over the target icon to see the current level.  
zoomDelta: 0.2 ### Adjust how much the zoom changes when you zoom in or out.  
unit: mi ### The value displayed when measuring so you know what type of unit is being measure.  
scale: 0.09328358208955223 ### Real units/px (resolution) of your map  
recenter: false  
darkmode: false ### markermarker: default,1254.641940511094,1439.8933879887836,s 3,hellooo,,

```