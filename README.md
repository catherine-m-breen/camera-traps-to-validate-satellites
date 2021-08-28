# MODIS-Snow-Cover-to-Binary-Snow-Covered-Area
MODIS Collection 6 removed the Snow Covered Area (SCA) band, instead replacing it with the NDSI Snow Cover band. This band provides the normalized difference snow index (NDSI) for snow cover on a scale of 0 to 100. It is recommended that users convert the NDSI Snow Cover to binary and fractional snow cover area using their own thresholds and expressions determined by region constraints. The accuracy of the fSCA and binary SCA are heavily determined by vegetation density, for example. This repository provides the Google Earth Engine scripts for converting MODIS NDSI Snow Cover to fSCA and binary using the original global expressions. This uses Google Earth Engine.



Put in differentiation between global expression 1 and global expression 2.

Global Expression 1: global expression is a file that takes even masked values and gives them a 3. This can inflate the no snow values, because clouds will be considered as no snow. The count for 1s and 2s should be the same though. 

