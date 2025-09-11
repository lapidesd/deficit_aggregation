# deficit_aggregation
# deficit_aggregation
This repository is the code and data supplement for the publication "Impact of spatial variability in root-zone storage deficit on runoff generation". This repository contains:
* Code:
  
    * deficit_averaging_streamflow_theoretical.ipynb: Jupyter notebook showing theoretical calculations of differences between deficit and streamflow with different scales of analysis (pixel and basin)
    * deficit_averaging_data_processing.ipynb: Colab notebook for processing data in Google Earth Engine to do deficit/runoff calculations at pixel and basin scale for study basins in California
    * deficit_averaging_CA_basins.ipynb: Jupyter notebook analyzing deficit and runoff data for the study basins in California
      
* Data

    * B120Basins_w_FNF_area_plux.zip: shapefile of CA DWR basins with basin characteristics
    * Correlations: contains files with calculated correlations between different pixel fluxes for different dates at all sites
    * FNF: full natural flows at DWR study basins
    * joblib_files: joblib files containing numpy arrays for each dat for the different pixel fluxes produced for this study. The data types included for each site are:
      
       * arrays_wy: wy sums of precipitation, ET, SWE
       * arrays_monthly: monthly precipitation, ET, SWE
       * Dpix: monthly pixel deficit
       * Qpix: monthly pixel runoff
      
    * SWANN: calculations of deficit and runoff using snow data from SWANN SWE. The data files included for each site are:
      
        * data_SWANN.csv: csv file of basin deficit, runoff, and other fluxes
        * Dpix_SWANN.joblib: dataframe with numpy arrays for each month for pixel deficit
        * Qpix_SWANN.joblib: dataframe with numpy arrays for each month for pixel runoff
