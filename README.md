# NASA-Algae-Bloom-Data
## Data Collection:
Data queried from 3 NASA satellites:  
CHLOROPHYLL: https://neo.sci.gsfc.nasa.gov/view.php?datasetId=MY1DMM_CHLORA  
SALINITY: https://salinity.oceansciences.org/data-smap-v4.htm  
SEA SURFACE TEMPERATURE: https://neo.sci.gsfc.nasa.gov/view.php?datasetId=MYD28M  

## Data Processing:
Data processed from .nc to .csv using Dataframes in Pandas. Masked from .shp shapefile using QGIS. Data was interpolated using spline (order = 1) for salinity dataset, as resolution was different from chlorophyll and sea surface temperature. Resulting .csv files are located in each dataset's respective directories.
