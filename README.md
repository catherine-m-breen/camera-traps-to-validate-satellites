# MODIS-Snow-Cover-to-Binary-Snow-Covered-Area
MODIS Collection 6 removed the Snow Covered Area (SCA) band, instead replacing it with the NDSI Snow Cover band. This band provides the normalized difference snow index (NDSI) for snow cover on a scale of 0 to 100. It is recommended that users convert the NDSI Snow Cover to binary and fractional snow cover area using their own thresholds and expressions determined by region constraints. The accuracy of the fSCA and binary SCA are heavily determined by vegetation density, for example. This repository provides the Google Earth Engine scripts for converting MODIS NDSI Snow Cover to fSCA and binary using the original global expressions. This uses Google Earth Engine.

Global Expression 1: global expression that includes a class for no snow (0), snow above 0.4 (1), and snow in the forest as proposed by Klein et al. 1998 (2). This approach classifies an image (not an image collection). The class for no snow currently is incomplete and misses some values. Please see global expression 2 for a more complete classification. 

Global Expression 2: global expression that includes a class for no snow (0), snow above 0.4 (1), and snow in the forest as proposed by Klein et al. 1998 (2). All other values are given a null value that reflect the conservative mask used for MODIS NDSI snow cover. This approach classifies an image collection (not an image). This code also includes a map and legend for visualization. 

Regional Expression 1: As recommended in the release of MODIS Collection 6, the global expression was removed, and instead it was recommended that users set their own regional thresholds. Here is code to set regional thresholds. A geometry can be used. In this case it an area in Norway is used that is a habitat that comprises four major Norwegian carnivores. 

Note: all code include statistics on the number of pixels in each snow class. Pixel counts can be used to find percent of snow-covered area, or multiplied by GEE's .pixelArea() function to determine area of snow in m^2. 

