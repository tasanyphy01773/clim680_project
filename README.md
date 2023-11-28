
## **The Dual Drivers: How ENSO and IOD Modulate Global Evaporation Dynamics**
> **Author**: Tahmidul Azom Sany 
> **Course**: CLIM680 (Fall 2023)
> **Affiliation**: PhD Student, Climate Dynamics, George Mason University  
> **Contact**: [tsany@gmu.edu](mailto:tsany@gmu.edu)  

---
### Introduction
This study investigates the relationship between total evaporation and the dual influence of El Nino-Southern Oscillation (ENSO) and Indian Ocean Dipole (IOD) on global and regional scales. The dominant influence of ENSO on several climate variables is widely recognized. By combining the Indian Ocean Dipole (IOD), the phase change of the El Niño-Southern Oscillation (ENSO) can be accelerated, leading to the emergence of distinct global teleconnection patterns (Ham et al., 2017). The geographical locations of ENSO and IOD also overlap their effects in regions such as Australia, Indonesia, and certain parts of Africa. In this study, I quantified the individual and combined impacts of ENSO and IOD on global evaporation patterns. Also, I identified a region (Australia) most sensitive to these dual influences.

ENSO is the sea surface temperature (SST) anomaly in the central and equatorial Pacific Ocean. I used the Nino 3.4 index to identify El Nino, La Nina, and Neutral phases. According to NCEI, NOAA El Nino (La Nina) is a phenomenon in the equatorial Pacific Ocean where the SST anomalies in the Niño 3.4 region are consistently above (below) the threshold of +0.5°C (-0.5°C) for five consecutive 3-month periods. Whereas the IOD is the difference in SST between the equatorial western and eastern parts of the Indian Ocean. I used the Dipole Mode Index (DMI) to identify the Positive (DMI>0.2), Negative (DMI<0.2), and Neutral Phases of IOD. 

I chose the FLUXCOM xBase Dataset for its high spatial and temporal resolution, essential for accurately analyzing evaporation patterns influenced by the ENSO and the IOD. Its comprehensive global coverage is also crucial for examining the widespread impacts of these climatic phenomena. 

### Data

#### 📊 Primary Dataset: Evaporation
To generate the FLUXCOM dataset, researchers from the Max Planck Institutes for Biogeochemistry used machine learning techniques; specifically the upscaling approach to combine in-situ observations, satellite remote sensing, and meteorological data. 

- **Source**: [FLUXCOM xBase Data](https://www.fluxcom.org/)
- **Spatial Resolution**: 0.05° x 0.05°
- **Temporal Resolution**: Daily data (12UTC) from `2001-01-01` to `2004-12-30` 
- **Variable**: Total Evaporation (mm/hour)
  ![FLUXCOMOVerview](https://github.com/tasanyphy01773/clim680_project/assets/68806666/87ceb90e-6611-4ed7-a014-d339debec523)

#### Climate Indices: NINO 3.4 
- **Source**: [NOAA Climate Prediction Center](https://www.cpc.ncep.noaa.gov/)
- **Spatial Coverage**: Central Equatorial Pacific, between 5°N - 5°S and 170°W - 120°W
- **Temporal Resolution**: Monthly averages
- **Variable**: SST anomalies (°C)

#### Climate Indices: DMI 
- **Download Source**: [NOAA Physical Sciences Laboratory](https://psl.noaa.gov/gcos_wgsp/Timeseries/DMI/)
- **Spatial Coverage**: Western tropical Indian Ocean (50°E to 70°E and 10°S to 10°N) and Southeastern tropical Indian Ocean (90°E to 110°E and 10°S to 0°S)
- **Temporal Resolution**: Monthly averages
- **Variable**: SST anomalies (°C)

#### Code Description 

##### 💾 Zarr Format
"*Zarr is a format tailored for **chunked**, **compressed**, and **N-dimensional arrays**. It serves both as a storage and computational format to efficiently manage large datasets.*" More details can be found in the [official documentation](https://zarr.readthedocs.io/en/stable/).

##### 📂 Zarr Data Structure
Zarr employs a hierarchical storage model, similar to directories and files in a traditional file system:
- **Group**: The top-level container that can include other `groups` or `arrays`.
- **Array**: A N-dimensional chunked array within a `group`.
- **Metadata**: Stored in a human-readable JSON format.
- **Data Chunks**: Often compressed and stored as binary blobs.
---
#### Results

#### Summary


#### Reference
- Ham, YG., Choi, JY. & Kug, JS. The weakening of the ENSO–Indian Ocean Dipole (IOD) coupling strength in recent decades. Clim Dyn 49, 249–261 (2017). https://doi.org/10.1007/s00382-016-3339-5









