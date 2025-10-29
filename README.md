# 🌍 Google Earth Engine Landsat 4–9 Filter and Batch Export

This repository contains a **Google Earth Engine (GEE)** script to filter, visualise, and batch download **Landsat 4–9 Collection 2 Tier 1 Top-of-Atmosphere (TOA)** multispectral satellite imagery over a defined area and time range.  

Co-developed with [**iamdonovan**](https://github.com/iamdonovan).  
Our script uses [`batch`](https://github.com/fitoprincipe/geetools-code-editor/blob/master/batch) produced by [**fitoprincipe**](https://github.com/fitoprincipe).

---

## ✨ Features

- Filters Landsat 4–9 imagery by:
  - Geometry  
  - Date range (start and end year, month, day)  
  - Image cloud cover %  
  - Land cloud cover %  
  - WRS path and row  

- Renames bands across different Landsat sensors for consistency.  
- Displays both false-color and true-color composites for quick visualisation.  
- Exports filtered ImageCollection to Google Drive using [`batch`](https://github.com/fitoprincipe/geetools-code-editor/blob/master/batch).

---

## ⚙️ Requirements

- [Google Earth Engine](https://earthengine.google.com/) account  
- The following Earth Engine user modules:
  - `users/tomosdanielmorgan/EarthObservation:Landsats`
  - `users/fitoprincipe/geetools:batch`
- A defined `geometry` variable (either drawn or uploaded in GEE).  
- *(Optional)* A defined WRS path/row.

---

## 🚀 Usage

1. Open the [**Google Earth Engine Code Editor**](https://code.earthengine.google.com/).  
2. Paste the contents of [`landsat_example`](https://github.com/tomosglaciology/Landsat_Image_Filter/blob/main/Landsat_example) into a new script.  
3. Define your area of interest (AOI) by setting a `geometry` variable.  
4. Modify data filters and WRS path/row parameters to match your AOI.

---

## 🧩 Filtering Options with `funcs`

A summary of the filtering functions available in the `funcs` module, and the associated Landsat data availability:

| Function | Description | Data Availability |
|-----------|--------------|------------------|
| `funcs.allLandsat` | Filters **Landsat 4–9** | 1982 – Present |
| `funcs.NewLandsat` | Filters **Landsat 8 and 9** | 2013 – Present |
| `funcs.EarlyLandsat` | Filters **Landsat 4, 5, and 7** | 1982 – 2025 *(See individual data availability below)* |
| `funcs.Landsat4` | Filters only **Landsat 4** | 1982 – 1993 |
| `funcs.Landsat5` | Filters only **Landsat 5** | 1984 – 2013 |
| `funcs.Landsat7` | Filters only **Landsat 7** | 1999 – 2025 *(Scan Line Corrector failure after May 2003)* |
| `funcs.Landsat8` | Filters only **Landsat 8** | 2013 – Present |
| `funcs.Landsat9` | Filters only **Landsat 9** | 2021 – Present |

---

## 🛰️ About

A **Google Earth Engine** script to filter, visualise, and batch export Landsat 4–9 Collection 2 Tier 1 TOA multispectral imagery over user-defined areas and time ranges.  

This tool simplifies large-scale Landsat processing for **remote sensing researchers, students, and GIS professionals**.

---

## 🧾 Topics

`remote-sensing` • `satellite-imagery` • `batch-script` • `google-earth-engine` • `earth-observation` • `landsat-data` • `batch-export`

---

## 📚 Resources

- [Google Earth Engine](https://earthengine.google.com/)  
- [fitoprincipe/geetools](https://github.com/fitoprincipe/geetools-code-editor)  
- [iamdonovan](https://github.com/iamdonovan)

---

© 2025 Tomos D. Morgan. All rights reserved.

