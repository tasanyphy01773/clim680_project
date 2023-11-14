# 
## 🌍 **The Dual Drivers: How ENSO and IOD Modulate Global Evaporation Dynamics**
> **Author**: *Tahmidul Azom Sany*  
> **Affiliation**: PhD Student, Climate Dynamics, George Mason University  
> **Contact**: [tsany@gmu.edu](mailto:tsany@gmu.edu)  

---

### 📊 Dataset Details
- **Source**: FLUXCOM xBase Data
- **Spatial Resolution**: 0.05° x 0.05°
- **Temporal Resolution**: Daily data (12UTC) from `2001-01-01` to `2003-12-30` (Reduced Dataset)
- **Variable**: Total Evaporation (ET Daily (mm/hour)

---

### 💾 Zarr Format
"*Zarr is a format tailored for **chunked**, **compressed**, and **N-dimensional arrays**. It serves both as a storage and computational format to efficiently manage large datasets.*" More details can be found in the [official documentation](https://zarr.readthedocs.io/en/stable/).

---

### 📂 Zarr Data Structure
Zarr employs a hierarchical storage model, similar to directories and files in a traditional file system:
- **Group**: The top-level container that can include other `groups` or `arrays`.
- **Array**: A N-dimensional chunked array within a `group`.
- **Metadata**: Stored in a human-readable JSON format.
- **Data Chunks**: Often compressed and stored as binary blobs.

