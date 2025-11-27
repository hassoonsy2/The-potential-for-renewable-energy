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

## Data Layers

The `layers/` directory contains the local geospatial data used in this project. This ensures that the project can be opened with the necessary data sources even without an active internet connection for some layers (though WMS/WFS layers from plugins will still require internet).

**Contents:**

*   **OpenStreetMap (OSM) Data**: Shapefiles (`.shp`) for various features such as:
    *   Buildings (`gis_osm_buildings_a_free_1.shp`)
    *   Landuse (`gis_osm_landuse_a_free_1.shp`)
    *   Natural features (`gis_osm_natural_a_free_1.shp`)
    *   Infrastructure: Railways, Roads, Waterways.
*   **Wind Data**: Raster data for wind speed (`noord_holland_wind-speed_100m.tif`).
*   **Styles**: QGIS Layer Style files (`.qml`) for visualizing power infrastructure (power lines, substations).