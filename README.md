# The-potential-for-renewable-energy

## How to Open in QGIS

To explore the spatial analysis and map visualizations for this project, you can open the project file directly in QGIS.

1.  Ensure you have **QGIS** installed on your system.
2.  Locate the file named `Qgis_project.qgz` in the root directory of this repository.
3.  Double-click the file or open QGIS and go to **Project -> Open**, then select `Qgis_project.qgz`.

### Recommended Plugins

For the best experience and to ensure all layers load and visualize correctly, we recommend installing the following plugins in QGIS:

*   **PDOK Services Plugin**: This is essential for accessing Dutch geospatial data services (PDOK). It allows you to easily add WMS/WFS layers from PDOK.
*   **OSM Plugin** (e.g., **QuickMapServices** or **QuickOSM**):
    *   **QuickMapServices**: Recommended for adding OpenStreetMap (OSM) background basemaps.
    *   **QuickOSM**: Useful if you need to download specific vector data from OpenStreetMap.

To install these plugins:
1.  Open QGIS.
2.  Go to **Plugins -> Manage and Install Plugins...**
3.  Search for the plugin name (e.g., "PDOK Services", "QuickMapServices").
4.  Click **Install Plugin**.

## Data Setup

To ensure all map layers load correctly, you need to have the local data files available.

1.  **Download the Data**:
    * Download the `layers.zip` file from the [layers](https://drive.google.com/file/d/19gNFlPqbDpwquv2_VeQXRk9POzU4SREb/view?usp=share_link). 
    * Unzip the file into the root directory of this project. You should end up with a folder named `layers` containing `.shp` and `.tif` files.

2.  **Open the Project**:
    *   Double-click `Qgis_project.qgz`.

3.  **Fixing Missing Layers (if needed)**:
    *   If QGIS warns about "Handle Bad Layers" upon opening, it means it can't find the data files.
    *   Click **Auto-Find** in the dialog, or manually browse to the `layers/` folder to locate the missing shapefiles (e.g., `gis_osm_buildings_a_free_1.shp`).
    *   Once one file is found, QGIS usually finds the rest automatically.
    *   Click **Apply Changes** or **OK**.

## Data Layers

The `layers/` directory contains the local geospatial data used in this project:

*   **OpenStreetMap (OSM) Data**: Shapefiles (`.shp`) for various features such as:
    *   Buildings (`gis_osm_buildings_a_free_1.shp`)
    *   Landuse (`gis_osm_landuse_a_free_1.shp`)
    *   Natural features (`gis_osm_natural_a_free_1.shp`)
    *   Infrastructure: Railways, Roads, Waterways.
*   **Wind Data**: Raster data for wind speed (`noord_holland_wind-speed_100m.tif`).
*   **Styles**: QGIS Layer Style files (`.qml`) for visualizing power infrastructure.