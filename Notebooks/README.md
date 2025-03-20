The Notebooks folder contains all of the necessary code to re-create this project. 
1) Download_Data.ipynb: Downloads the SAR imagery from Open Capella SAR data.
2) Label_Chip_Data.ipynb: This notebook will utilize Wildland Fire Interagency Geospatial Services (WFIGS) perimeter data to determine the extent of the wildfires present in the SAR images. Then it will chip the images into smaller tiles for training.
3) CNN.ipynb: This notebook will utilize Wildland Fire Interagency Geospatial Services (WFIGS) perimeter data to determine the extent of the wildfires present in the SAR images. Then it will chip the images into smaller tiles for training. To replicate this notebook, you need to download GeoJSON file from https://data-nifc.opendata.arcgis.com/datasets/7c81ab78d8464e5c9771e49b64e834e9_0/explore?showTable=true
4) DEM.ipynb: This notebook will create a Digital Elevation Map (DEM) around the area of our SAR imagery. Incorporating the DEM and overlaying the SAR images will provide a useful visualization and serve. Finally, this notebook will serve as the first step to eventually integrate the topographical data into the machine learning model to aid in prediction of wildfire progression.

In the Old folder, there are notebooks that were created earlier in the project that are now out of date with the current status of the project.
