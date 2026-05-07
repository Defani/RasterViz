# QRVIZ — Raster Visualization Plugin for QGIS

![QGIS](https://img.shields.io/badge/QGIS-3.x-green?logo=qgis)
![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-orange)

## Overview

QRVIZ is a QGIS plugin designed to simplify raster visualization workflows using customizable color maps and enhanced raster display utilities. The plugin helps users quickly visualize raster datasets for remote sensing, GIS analysis, environmental mapping, and land cover interpretation.

This plugin is suitable for:

* Remote sensing analysis
* Vegetation index visualization
* DEM and terrain rendering
* Land cover interpretation
* Scientific raster presentation
* GIS education and training

---

# Features

* Multiple raster visualization presets
* Custom color map support
* Fast raster rendering
* RGB raster preview support
* Simple GUI integration inside QGIS
* Lightweight Python-based plugin architecture

---

# Plugin Structure

```plaintext
raster_viz_plugin/
│
├── __init__.py
├── qrviz.py
├── dialog.py
├── colormaps.py
├── metadata.txt
├── icon.png
├── demo_rgb.png
└── __pycache__/
```

---

# Installation

## Method 1 — Manual Installation

1. Download the plugin ZIP file.
2. Extract the ZIP file.
3. Copy the folder:

```plaintext
raster_viz_plugin
```

into:

```plaintext
C:\Users\USERNAME\AppData\Roaming\QGIS\QGIS3\profiles\default\python\plugins\
```

4. Open QGIS.
5. Go to:

```plaintext
Plugins → Manage and Install Plugins
```

6. Enable:

```plaintext
QRVIZ
```

---

# Requirements

## Software Requirements

* QGIS 3.x
* Python 3.x
* GDAL
* PyQt5
* NumPy
* Rasterio *(optional)*
* Matplotlib *(optional for visualization previews)*

---

# Python Packages

The plugin uses several Python libraries integrated with QGIS.

| Package      | Function                      |
| ------------ | ----------------------------- |
| `qgis.core`  | Core QGIS raster processing   |
| `qgis.gui`   | GUI integration in QGIS       |
| `PyQt5`      | Interface and dialog windows  |
| `os`         | File and directory management |
| `numpy`      | Raster numerical operations   |
| `matplotlib` | Color map rendering           |
| `gdal`       | Raster data handling          |

---

# Installation Dependencies

Most dependencies are already included in QGIS.

If additional packages are required:

```bash
pip install numpy matplotlib rasterio
```

GDAL should preferably use the QGIS bundled environment.

---

# Supported Raster Data

* GeoTIFF (`.tif`)
* IMG Raster (`.img`)
* JPEG2000 (`.jp2`)
* ASCII Grid (`.asc`)
* DEM Raster
* Sentinel-2 Imagery
* Landsat Imagery

---

# Visualization Modes

| Visualization   | Description                  |
| --------------- | ---------------------------- |
| RGB Composite   | Natural color visualization  |
| False Color     | Vegetation enhancement       |
| NDVI Style      | Vegetation index rendering   |
| DEM Shading     | Terrain visualization        |
| Custom Colormap | User-defined color gradients |

---

# Usage

1. Open QGIS.
2. Load raster data.
3. Open QRVIZ plugin from toolbar or plugin menu.
4. Select visualization style.
5. Apply color map or raster enhancement.
6. Export visualization if needed.

---

# Example Visualization

## RGB Visualization Example

![Demo](demo_rgb.png)

---

# Metadata

| Property             | Value              |
| -------------------- | ------------------ |
| Plugin Name          | QRVIZ              |
| Type                 | QGIS Python Plugin |
| Main File            | qrviz.py           |
| GUI Module           | dialog.py          |
| Visualization Engine | colormaps.py       |

---

# Development

## Clone Repository

```bash
git clone https://github.com/USERNAME/QRVIZ.git
```

## Open Plugin Folder

```bash
cd QRVIZ
```

---

# Common Errors

## Plugin Not Showing in QGIS

Ensure the plugin folder structure is correct:

```plaintext
plugins/raster_viz_plugin/
```

not:

```plaintext
plugins/raster_viz_plugin/raster_viz_plugin/
```

---

## Missing About Dialog / HTML Error

If QGIS shows errors related to:

```python
html_text = open(about_file).read()
```

possible causes:

* Missing HTML resource file
* Incorrect plugin path
* Incompatible QGIS version
* Corrupted plugin extraction

Solution:

* Reinstall plugin
* Verify plugin folder structure
* Ensure all files are extracted correctly

---

# Citation

If you use this plugin in research, publication, or academic work, please cite:

```bibtex
@software{qrviz2026,
  author = {Defani Arman Alfitriansyah},
  title = {QRVIZ: Raster Visualization Plugin for QGIS},
  year = {2026},
  version = {1.0},
  url = {https://github.com/USERNAME/QRVIZ}
}
```

## APA Citation

Alfitriansyah, D. A. (2026). *QRVIZ: Raster Visualization Plugin for QGIS* (Version 1.0) [Computer software]. GitHub. [https://github.com/USERNAME/QRVIZ](https://github.com/USERNAME/QRVIZ)

---

# License

MIT License

---

# Author

**Defani Arman Alfitriansyah**

Forestry Student | GIS & Remote Sensing Enthusiast | QGIS Plugin Developer

---

# Support

If you find bugs or want to contribute:

* Open an issue
* Submit pull requests
* Share feature suggestions

---

# Keywords

QGIS Plugin, Raster Visualization, GIS, Remote Sensing, NDVI, DEM, Color Map, Spatial Analysis, Python Plugin, Geospatial Visualization
