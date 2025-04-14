![image](https://github.com/user-attachments/assets/507a10d8-b4af-43a8-84b0-49ff4965b900)This repository contains my submission for the EDA assignment on optimizing NYC Taxi operations.

The project uses two main datasets:
1. NYC Yellow Taxi Trip Data of year 2023.
you can download parquet files for 2023 from the NYC TLC website:  
🔗 [NYC TLC Trip Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

- Place all downloaded files inside a folder called trip_records.

2. NYC Taxi Zone Geospatial Data these are shapefiles:
To map zone IDs pickup and dropoff ids to real locations, I used the Taxi Zones shapefile.  
Download it from:  
🔗 [NYC Taxi Zones Shapefile (ZIP)](https://www1.nyc.gov/assets/tlc/downloads/pdf/taxi_zones.zip)

- Unzip the contents into a folder named taxi_zones
- The shapefile contains columns like:
  - `LocationID`: zone ID
  - `zone`: zone name
  - `borough`: borough name
  - `geometry`: spatial polygon used for plotting

Just make sure your code loads from taxi_zones/taxi_zones.shp if you are using GeoPandas.
