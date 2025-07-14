Since 2015, I have started working with Sentinel-1 TOPS SAR data using python. There are several personal modules,e.g. pS1/pDATA/pSAR, to have been developped for almost 10 years. With extensive tests and improvements, these codes and scripts have been proved helpful particularly for new InSAR beginners. There are several example scripts to show you how to run python scripts to get InSAR processing done based on GMTSAR with no harm...

Modules:
-pS1           a simple python module to read meta information of TOPS SAR data in either ZIP or unZIP files/folders...
-pSAR          a merged python module to handle general InSAR analysis 
-pDATA         a merged python module to manipulate variable scientific data format, e.g. netCDF, geotif, roi_pac(pSAR can do better). 


Scripts:
-pSAR_s1sorting.py    0/1, a useful light python script to sort TOPS SAR data based on its track information (relativeOrbit) directly from zip files.
-pSAR_gmtsar_s1.py    a batch script to drive GMTSAR to get a TOPS SAR InSAR processing done in one script, including 
     * DEM preparation (I have prepared DEM database in our own server. If you have no such dataset. You can prepare a dem ahead. The code will ignore to make DEM data for target projects.
     * Crop TOPS data, "-roi minlon,maxlon,minlat,maxlat" can pass spatial information to pSAR_gmtsar_s1.py. The codes will select TOPS data and crop the data for target processing automatically. 

