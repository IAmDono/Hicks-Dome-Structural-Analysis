# Structural and Geological Analysis of Hicks Dome, Illinois

## Project Overview
This project visualizes the cryptoexplosive ring structure of Hicks Dome in Hardin County, Illinois. Hicks Dome is a dormant, prehistoric cryptovolcanic structure pushed upward by magma and gas over 270 million years ago, exposing concentrated sedimentary rings and extensive fault networks. 

This map combines high-resolution terrain visualization with statewide bedrock geology data to expose subsurface features hiding beneath the forest canopy.

## Visual Analysis
![Hicks Dome Geological Map](Hicks_Dome_Final_Map.png)

## Technical Workflow & Python Automation
1. **Data Acquisition**: Sourced a 1/3 arc-second Digital Elevation Model (DEM) from the USGS 3DEP program and vector bedrock layers from the Illinois State Geological Survey (ISGS).
2. **Terrain Engineering**: Developed a custom **PyQGIS script** inside the QGIS Python Console to automatically query the loaded project rasters and compute a multi-directional 3D hillshade layer using GDAL processing algorithms.
3. **Programmatic Data Styling**: Wrote an automated Python rendering script to read database attribute columns (`PYCODE`), filter regional classes, and apply distinct color palettes to separate geologic units wrapping around the core bull's-eye.
4. **Cartographic Design**: Blended geology polygon transparency (60% Opacity via Multiply blend mode) over texturized topography, layered structural fault vector lines on top, and configured a print layout with a scale-filtered dynamic legend.

## Skills Demonstrated
* Open-Source GIS Architecture (QGIS)
* PyQGIS Automation & Processing Libraries
* Digital Elevation Model (DEM) Terrain Analysis
* Cartographic Layout & Dynamic Item Styling
