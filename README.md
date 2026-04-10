# London Traffic Accident Hotspots Pipeline

This repository implements an automated, reproducible pipeline for detecting, ranking, and visualising traffic accident hotspots in Greater London using historical STATS19 data from UK government portals.

## Aim
To design, implement, and validate an open-source pipeline that:
- Downloads and pre-processes STATS19 accident data for Greater London (2020–2024).  
- Applies spatial analysis techniques (KDE, Getis-Ord Gi*, DBSCAN) to detect hotspots.  
- Computes severity‑ and persistence‑weighted composite rankings.  
- Validates results against TfL/Vision Zero data and temporal hold‑out (2024).

## Tech stack
- Python  
- GeoPandas  
- PySAL / `esda` (for Getis‑Ord Gi*)  
- `osmnx` (for London road network)  
- Google Colab (for interactive development)
- Kepler.gl / Folium (for interactive maps)
