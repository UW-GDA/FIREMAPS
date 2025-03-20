# FIREMAPS
Project Title:
FIREMAPS: Fire Imaging, Recognition, and Evaluation Mapping with AI Processing SAR 

## Team Members:
Rafael Rubenstein and Matt McMaster

## Background:

One of the main benefits of synthetic aperture radar (SAR) imagery is the ability to image day and night and during all weather. The ability to penetrate through thick smoke during an active wildfire emergency highlights a key advantage over normal optical imagery, which is blocked by the smoke. Designing a machine learning (ML) model that inputs a SAR image and can determine the active boundary of a wildfire presents a unique capability for first-responders to mitigate the spread of the fire and provide ample warning to nearby residents. We utilized imagery from the Open Capella SAR Dataset to create a supervised Convolutional Neural Network that will detect the geographic extent of a wildfire. We trained a model using labeled wildfire data. Our main objective was to draw a bounding shape around the burned landscape with our trained model. Our secondary objective was to incorporate elevation data to create a topographical map of the damaged area and its surroundings to further inform the optimal locations for first-responders' response.

## Datasets we used:

We used the following datasets:
- https://felt.com/map/Capella-Space-Open-Data-bB24xsH3SuiUlpMdDbVRaA?loc=0,-20.53,1.88z
- https://radiantearth.github.io/stac-browser/#/external/capella-open-data.s3.us-west-2.amazonaws.com/stac/catalog.json?.language=en
- https://data-nifc.opendata.arcgis.com/datasets/7c81ab78d8464e5c9771e49b64e834e9_0/explore?showTable=true
- https://planetarycomputer.microsoft.com/dataset/cop-dem-glo-30

## Tools/packages we used:

Download_Data.ipynb requires the following Python packages:
- os
- requests
- json
- urllib.parse
- numpy
- rastero
- matplotlib

Label_Chip_Data.ipynb requires the following Python packages:
- numpy
- geopandas
- matplotlib
- matplotlib_scalebar
- contextily
- os
- rasterio
- shapely
- warnings

CNN.ipynb requires the following Python packages: 
- json
- numpy
- rasterio
- torch
- PIL
- os
- itertools
- sklearn

DEM.ipynb requires the following Python packages:
- pystac_client
- planetary_computer
- os
- rasterio
- geopandas
- shapely
- matplotlib
- matplotlib_scalebar
- contextily
- rioxarray

## Methodology:

- Load in SAR data in regions with active wildfires using methods learned in class/lab
- Clip wildfire boundaries to SAR images
- Chip labeled SAR data to prepare for CNN training
- Train CNN using hyperparameter grid search and evaluate accuracy to choose model
- Apply model to subset of chipped, labeled data to validate accuracy

## Results:

Gain experience with SAR data and ML techniques. Produce a model with greater than 75% accuracy.

## References

We used the following references as a guide:

- https://www.nature.com/articles/s41598-019-56967-x#Tab1
- https://www.sciencedirect.com/science/article/abs/pii/S0143622822002259
- https://tema-project.eu/articles/wildfire-mapping-using-sar-derived-nbr-through-generative-adversarial-network
- https://www.diva-portal.org/smash/get/diva2:1557423/FULLTEXT02.pdf
- https://arxiv.org/html/2501.09129v1
- https://www.earthdata.nasa.gov/learn/earth-observation-data-basics/sar
- https://byrd.osu.edu/news/revolutionizing-wildfire-management-sar-technology-enhances-detection-and-response
- https://medium.com/@robmarkcole/deep-learning-with-sar-18b27972a4b5
