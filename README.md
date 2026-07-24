# Keefe-SOARS-2026
Code for research project, examining CESM2.2 CAM-chem regional sensitivities of ozone and PM2.5 due to wildfire emissions in Australia and North America. All necessary scripts are included.

  
 
1. emissions_masking.ipynb: Script used to read in original emissions datasets, apply regional mask, and create three masked collections of netcdf files

  
   
2. regions.ipynb: Script used to establish regions for our experiment and create regional files to use as the basis for the mask

   
3. utils: Contains modules for different types of plots, and the original regional netcdf files
   
    a) difference plot module - module with functions to plot surface spatial differences in pollutant concentrations between simulations, averaged both seasonally and over the whole study period
   
   b) mapping module - module with mapping functions, including surface concentrations and tropospheric concentrations for both pollutants, as well as stratospheric concentrations for ozone
   
   c) percent contribution - module with functions that calculated percent contribution of a given region when compared to the historical region. Also contains code to produce a table and time series of seasonal percent contributions
   
   d) timeseries module - module with functions to create a time series of surface ozone concentrations, surface pm25 concentrations, and concentration differences between all four simulations.
   
   e) utils helper funcs - contains helper functions for all other utility modules
   
   f) utils regions - contains a copy of the original regions.ipynb to be used in other utility modules
   
  

5. analysis: Contains notebooks with final data analyses
   
   a) PM2.5 analysis - notebook with time series of PM2.5 concentrations and percent contribution plots/tables
   
   b) difference analysis - notebook with spatial difference plots for all three masked simulations for PM2.5 and ozone, as well as difference timeseries
   
   c) dust maps - notebook with spatial maps of coarse dust and PM2.5 concentrations for the two dust schemes tested
   
   d) historical analysis - spatial maps of seasonal averages for ozone and PM2.5 for the historical, global fire simulation
   
   e) ozone analysis - notebook with time series of ozone concentrations and percent contribution plots/tables
