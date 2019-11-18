# NASA-Algae-Bloom-Data
## Data Collection:
Data queried from 3 NASA satellites:  
CHLOROPHYLL: https://neo.sci.gsfc.nasa.gov/view.php?datasetId=MY1DMM_CHLORA  
SALINITY: https://salinity.oceansciences.org/data-smap-v4.htm  
SEA SURFACE TEMPERATURE: https://neo.sci.gsfc.nasa.gov/view.php?datasetId=MYD28M  

## Data Processing:
Data processed from .nc to .csv using Dataframes in Pandas. Data was interpolated using spline (order = 1) for salinity dataset, as resolution was different from chlorophyll and sea surface temperature. Masked from .shp shapefile using QGIS. Resulting .csv files are located in the "final" directory. Intermediate data (cropped to rectangle around shapefile for faster QGIS processing) is located in each dataset's respective directories.
