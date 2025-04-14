This repository contains my submission for the EDA assignment on optimizing NYC Taxi operations.

The project uses two main datasets:

1. **NYC Yellow Taxi Trip Data (2023)**  
You can download the `.parquet` files for 2023 from the NYC TLC website:  
🔗 [NYC TLC Trip Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

- Place all downloaded files inside a folder called `trip_records`.

2. **NYC Taxi Zone Geospatial Data (Shapefiles)**  
To map pickup and drop-off zone IDs to real locations, I used the official Taxi Zones shapefile.  
This can be downloaded from the same link shared above — look for the section titled **"Taxi Zone Maps and Lookup Tables"**  
and click on the file **"Taxi Zone Shapefile (Parquet)"**.  
It downloads as a `.zip` shapefile.

- Unzip the contents into a folder named `taxi_zones`
- The shapefile contains columns like:
  - `LocationID`: zone ID
  - `zone`: zone name
  - `borough`: borough name
  - `geometry`: spatial polygon used for plotting

Make sure your code loads from `taxi_zones/taxi_zones.shp` if you're using GeoPandas.
