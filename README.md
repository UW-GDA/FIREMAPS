# FIREMAPS
Project Title:
FIREMAPS: Fire Imaging, Recognition, and Evaluation Mapping with AI Processing with SAR 

## Team Members:
Rafael Rubenstein and Matt McMaster

## Short 1-2 sentence summary:

We aim to utilize historical SAR data from the Sentinel-1 mission that imaged wildfires to create a supervised Convolutional Neural Network that will detect the geographic extent of a wildfire. Our model will use labeled wildfire data to train itself on such SAR images. We will use images covering a wildfire to track how it evolves through time. 

## Some introductory background information:

One of the main benefits of synthetic aperture radar (SAR) imagery is the ability to image day and night and during all weather. The ability to penetrate through thick smoke during an active wildfire emergency highlights a key advantage over normal optical imagery, which is blocked by the smoke. Designing a machine learning (ML) model that inputs a SAR image and can determine the active boundary of a wildfire presents a unique capability for first-responders to mitigate the spread of the fire and provide ample warning to nearby residents. 

## Problem statement, question(s) and/or objective(s):

Our main objective is to draw a bounding shape around the burned landscape. Pending time constraints, our secondary objective is to incorporate elevation data to create a topographical map of the damaged area and its surroundings, which would further inform the optimal locations for first-responders' response.

## Datasets you will use (with links, if available)

We will use at least the following datasets:
https://search.earthdata.nasa.gov/search?fi=SAR
https://developers.google.com/earth-engine/datasets/catalog/sentinel
https://dataspace.copernicus.eu/explore-data/data-collections/sentinel-data/sentinel-1

## Tools/packages you’ll use (with links)

For general coding and SAR handling we will use numpy, pandas, geopandas, rasterio, rioxarray, shapely, matplotlib, contextily, and sarpy, SNAP (Sentinel Application Platform)​​, and SARkit. Also, we will experiment with scikit-learn, pytorch, keras, and tensorflow for the machine learning aspect of the project.


## Planned methodology/approach

- Load in SAR data with active wildfires using methods learned in class/lab
- Do any necessary pre-processing and formatting, including partitioning for our ML model
- Train a convolutional neural network using available Python tools, then validate and test results

## Expected outcomes

Gain experience with SAR data and ML techniques. Produce a model with greater than 75% accuracy.

## Any other relevant information, images/tables, references, etc.


## References

https://www.nature.com/articles/s41598-019-56967-x#Tab1
