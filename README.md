# MODIS-Snow-Cover-to-Binary-Snow-Covered-Area

Scripts for “Evaluating MODIS snow products using an extensive wildlife camera network" published in Remote Sensing of Environment. 

This code is written in java script for Google Earth Engine, python, and R.

- MOD10A1F_PointExtraction – extracts MOD10A1F NDSI values from camera locations in Google Earth Engine
- R_analysis – analysis code for paper in R
- SCA_Klein_allDays – how Klein et at al. 1998 proposed identifying snow and no snow pixels using a threshold 0.4, and a sliding scale from NDVI
- globalSCA_expression in Google Earth Engine
- mapExtraction – extracts MOD10A1 NDSI values from camera locations in Google Earth Engine
- pointExtraction_CGF_CloudPersistence – prepares MOD10A1F dataset for point extraction by mosaicking images (as input for MOD10A1F_PointExtraction) in Google Earth Engine.
- regionalThreshold_Norway – updates Norway MOD10A1 NDSI map using threshold derived in the paper
- segmentationAI – beta-model for repeating analysis using machine learning in python
- statistics – summary statistics for paper in R

