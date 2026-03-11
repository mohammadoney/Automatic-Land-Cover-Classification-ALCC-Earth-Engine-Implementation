# Automatic-Land-Cover-Classification-ALCC-Earth-Engine-Implementation

This project implements the Automatic Land Cover Classification (ALCC) methodology from Gašparović et al. (2019) as a web application in Google Earth Engine. The system automatically classifies satellite imagery into five land cover classes (Water, High Vegetation, Low Vegetation, Bare Land, and Built-up) using a novel sequential approach based on spectral indices and k-means clustering.

The implementation follows the paper's workflow :

Water extraction using MNDWI (Modified Normalized Difference Water Index) with 2-class k-means

Vegetation separation (high/low) using NDVI with 3-class k-means

Bare land identification using NDBaI with 3-class k-means

Built-up vs remaining bare land separation using NBLI with 2-class k-means

Key features include user input for any city name and year (2013-present), automatic Landsat 8 image retrieval with cloud filtering, atmospheric correction (DOS1 method via QA_Pixel band), accuracy assessment against Dynamic World V1 reference data, and safe download functionality.
