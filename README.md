# Flood Exposure in Sub-Saharan African Cities

Data Repository and Code Repository with data and scripts used and generated in the article "Exposed yet unmapped? Evidence of differential flood exposure in deprived urban areas using citizen science". 

All input and output data are provided and properly described in the medatata files (.txt). 

We also provide a code pipeline with the following purposes:

#### 1_Grid_Creation.ipynb 
to create of 50x50m (changeable) grid for spatial analysis

#### 2_GIS_GridProcessing.ipynb 
to integrate the flood exposure elements (modelled flood hazard output + built-up layers) to the grid

#### 3_ProcessingExposure.ipynb 
to process the resulting flood exposure dataset above, including clean up, analyse the outputs, define built-up density thresholds, and calculate relative and absolute flood exposure

#### 4_DUA_Analysis.ipynb
to analyse the differences between DUAs and non-DUAs in each built-up dataset at city scale 

#### 5_ThematicAnalysis_CommunityData.ipynb 
to run the thematic analysis of reported flood impacts (from community survey) and to compute a hit-and-miss evaluation comparing the modelled and observed (surveyed) flood points at community level
   
## Requirements
- Python
- Jupyter Notebook
- Required libraries are described in each script

## Usage
Open the Jupyter Notebook and run the notebook step by step.

## Outputs
#### 1_Grid_Creation.ipynb: 
- Output Name: 'grid_cityName.shp'
- Output Description: 50x50m empty grid for each city

#### 2_GIS_GridProcessing.ipynb: 

- Intermediate Output Name: 'resampled_raster_proj.tif' + 'GHSL_proj.tif' + 'GOB_grid.gpkg'
- Output Name: 'CityInitial_grid_final.shp'
- Output Description: 50x50m grid for each area filled with values from modelled flood hazard output and two built-up layers (GOB and GHSL) for each city

#### 3_ProcessingExposure.ipynb: clean up data with all cities and relative and absolute flood exposure table for each built-up layer
- Output Name: 'FloodExposure_Dataset.csv' and 'FloodExposure_Absolute_Relative.xlsx'
- Output Description: clean up data with all cities and relative and absolute flood exposure table for each built-up layer
  
#### 4_DUA_Analysis.ipynb:  
- Output Name: visulization of flood exposure by city and built-up category
- Output Description: analysis of the differences between DUAs and non-DUAs in each built-up dataset at city scale

#### 5_ThematicAnalysis_CommunityData.ipynb: 
- Intermediate Output Name: 'MyMaps_Output_v1.csv' + 'MyMaps_Impacts_Processed.csv' + 'MyMaps_Impacts_LookUpTable.csv' + 'MyMaps_Impacts_Counts.csv' 
- Output Name: 'MyMaps_Impacts_Processed' + visualization of the thematic analysis and the hit-and-miss evaluation plot
- Output Description: Coding process with intermediate output tables, visualization of thematic analysis of reported flood impacts and hit-and-miss evaluation comparing the modelled and observed (surveyed) flood points at community level
