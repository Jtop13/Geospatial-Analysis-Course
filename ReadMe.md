# Geospatial Analysis Course (Kaggle) #

https://www.kaggle.com/learn/geospatial-analysis 

** Intro **

- How to use geopandas (gpd)
- Ploting a map with geopandas


** Coordinate Reference Systems (CRS) **

- Create a GeoDataFrame
- GeoDataFrame uses EPSG 32630, Coordinate reference systems are referenced by European Petroleum Survey Group (EPSG) codes.
- To convert it to a GeoDataFrame, we use gpd.GeoDataFrame().
- The gpd.points_from_xy() function creates Point objects from the latitude and longitude columns.
- to_crs() method changes the CRS of the facilities GeoDataFrame to match the CRS of regions before plotting it.

- Plotting bird migration with start, middle and end points on the americas map


** Interactive Maps **

- Heat and Bubble maps to assess earthquake activity and depth
- Choropleth maps to understand prefectures of population density in Japan
- Used Python library folium to create maps


** Manipulating Geospatial Data **

Investigate the demographics of various counties in the state of California, to determine potentially suitable locations
to find the next store into a Starbucks Reserve Roastery.

- Geocoding: converting the name of a place or an address to a location on a map
- Used Nominatim() (from geopy.geocoders) to geocode values
- Join and Merge with Pandas library


** Proximity Analysis **

Identify how hospitals have been responding to crash collisions in New York City.
- Measure the distance between points on a map.
- Select all points within some radius of a feature.
- Creating a buffer *If we want to understand all points on a map that are some radius away from a point, the simplest way is to create a buffer.*
- unary_union attribute collapses all of the polygons into a MultiPolygon object. More efficient to run one object instead of mutiple seperate objects.
