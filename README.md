# Flood Exposure in Sub-Saharan African Cities

Repository of scripts (Jupyter notebooks) and respective data used in the article "Exposed yet unmapped? Evidence of differential flood exposure in deprived urban areas using citizen science". 
Here we provide a series of codes with the following purposes:
1_Grid_Creation: to create of 50x50m (changeable) grid for spatial analysis
2_GIS_GridProcessing: to integrate the flood exposure elements (modelled flood hazard output + built-up layers) to the grid
3_ProcessingExposure: to process the resulting flood exposure dataset above, including clean up, analyse the outputs, define built-up density thresholds, and calculate relative and absolute flood exposure
4_DUA_Analysis: to analyse the differences between DUAs and non-DUAs in each built-up dataset at city scale 
5_ThematicAnalysis_CommunityData: run the thematic analysis of reported flood impacts (from community survey) and to compute a hit-and-miss evaluation comparing the modelled and observed (surveyed) flood points at community level
   
## Requirements
- Python
- Jupyter Notebook
- Required libraries are described in each script

## Usage
Open the Jupyter Notebook and run the notebook step by step

## Outputs
1_Grid_Creation: 50x50m empty grid for each city
Output Name: 'grid_cityName.shp'
2_GIS_GridProcessing: 50x50m grid for each area filled with values from modelled flood hazard output and two built-up layers (GOB and GHSL) for each city
Intermediate Output Name: 'resampled_raster_proj.tif' + 'GHSL_proj.tif' + 'GOB_grid.gpkg'
Output Name: 'CityInitial_grid_final.shp' 
3_ProcessingExposure: clean up data with all cities and relative and absolute flood exposure table for each built-up layer
Output Name: 'FloodExposure_Dataset.csv' and 'FloodExposure_Absolute_Relative.xlsx'
4_DUA_Analysis: to analyse the differences between DUAs and non-DUAs in each built-up dataset at city scale 
Output Name: 'FloodExposure_Dataset_DUA' + visulization of flood exposure by city and built-up category
5_ThematicAnalysis_CommunityData: coding and visualization of thematic analysis of reported flood impacts (from community survey) and hit-and-miss evaluation comparing the modelled and observed (surveyed) flood points at community level
Intermediate Output Name: 'MyMaps_Output_v1.csv' + 'MyMaps_Impacts_Processed.csv' + 'MyMaps_Impacts_LookUpTable.csv' + 'MyMaps_Impacts_Counts.csv' 
Output Name: 'MyMaps_Impacts_Processed' + visualization of the thematic analysis and the hit-and-miss evaluation plot
