# Python Code for MSc Thesis: Multispectral LiDAR River Bathymetry

This repository contains original Python research code developed for my MSc thesis:

**Applications of Multi-spectral LiDAR: River Channel Bathymetry and Canopy Vegetation Indices**  
Maxim Okhrimenko, MSc Thesis, University of Lethbridge, 2018.

The code is associated with the bathymetry component of the thesis, specifically:

**Chapter 2 — Urban river environment digital water surface model generation and in situ bathymetric correction using multi-spectral LiDAR**

## Thesis reference

Okhrimenko, M. (2018).  
**Applications of Multi-spectral LiDAR: River Channel Bathymetry and Canopy Vegetation Indices.**  
MSc Thesis, University of Lethbridge.

Available through the University of Lethbridge Library and ProQuest Dissertations & Theses.

ProQuest record:  
https://www.proquest.com/docview/2154850134

## Repository contents

```text
Thesis_Bathy_Py.txt
```

This is the original thesis-era Python script used in the bathymetric processing workflow.

## What the code does

The script was developed to support the generation of a **virtual water surface model** for airborne multispectral LiDAR bathymetry.

In the original workflow, the code used:

- river centerline points;
- LiDAR points clipped near the river centerline;
- local cross-section bins generated along the river;
- water-surface elevation statistics calculated from LiDAR points.

The script generates artificial point-cloud representations of the water surface using local elevation summaries, including:

- mean elevation;
- 90th percentile elevation;
- maximum elevation.

These virtual water surface models were then used in the broader thesis workflow for in situ bathymetric correction of green-channel LiDAR returns below the water surface.

## Scientific context

Airborne bathymetric LiDAR requires correction for refraction at the air-water interface. In complex urban river environments, water surface modelling can be difficult because of bridges, overhanging vegetation, islands, river gradients, and complex channel geometry.

The MSc thesis developed an end-user-oriented approach for generating a water surface model and applying simplified in situ bathymetric correction in shallow river environments.

The original case study used multispectral Teledyne Optech Titan LiDAR data collected over the Bow and Elbow Rivers in Calgary, Alberta.

## Note on code status

This repository preserves the original research code.

The script was written during the MSc thesis period and is shared as archival research code, not as a modern Python package. It may require adaptation before being run in a current Python environment.

The purpose of this repository is to document and share the Python component of the MSc research workflow.

## Skills demonstrated

This code illustrates experience with:

- Python scripting for geospatial research;
- LiDAR point-cloud processing workflows;
- river bathymetry and water-surface modelling;
- NumPy and pandas-based data handling;
- computational geometry for local transect/bin construction;
- integration of Python outputs with GIS and LiDAR processing software.

## Author

**Maxim Okhrimenko**  
MSc Geography, University of Lethbridge  
Remote sensing, LiDAR, bathymetry, forest structure, and geospatial modelling
