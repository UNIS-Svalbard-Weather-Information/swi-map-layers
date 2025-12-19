# SWI Map Layers

This repository stores static map layers for the **Svalbard Weather Information (SWI)** project.

## **Folder Structure**
Each layer must have its own folder containing:
- **Shapefile or GeoJSON** (or other Mapnik-compatible format)
- **Mapnik XML config** (for styling)
- **HTML legend** (visual reference)
- **LICENSE file** (specify data provider and license terms)

Example:
```
swi-map-layers/
├── my_layer/
│   ├── my_layer.shp (or .geojson)
│   ├── my_layer.xml
│   ├── legend.html
│   └── LICENSE
└── ...
```

## **How to Add a New Layer**
1. **Add your layer files** in a new folder.
2. **Include all required files** (shapefile, XML, legend, and LICENSE).
3. **Open a pull request** in this repository.
4. **Open an issue** in:
   - [swi-mapproxy-configuration](https://github.com/UNIS-Svalbard-Weather-Information/swi-mapproxy-configuration) (for map server integration)
   - [swi-frontend](https://github.com/UNIS-Svalbard-Weather-Information/swi-frontend) (for frontend inclusion)

## **Tools**
- **[TileMill](https://github.com/tilemill-project/tilemill)** is a great tool to generate Mapnik XML files.
- **[QGIS](https://qgis.org/)** is a great Geo Information Software
