## Glossary

* What is LIDAR?

	-	LIDAR (Light Detection and Ranging) is a method to measure distance using light. The device will illuminate a target with a laser light and a sensor will measure the reflection. Differences in wavelength and return times will be used to get 3D representations of an area.


* What are points clouds?

	- A point cloud is a set of data points in space. The points represent a 3D shape or object. Each point has its set of X, Y and Z coordinates. Point clouds are generally produced by 3D scanners or by photogrammetry software, which measure many points on the external surfaces of objects around them.

* What is DSM (Digital Surface Map)?

	- A DSM (Digital Surface Model) captures both the natural and built/artificial features of the environment. 

* What is DTM (Digital Terrain Map)?

	– A DTM (Digital Terrain Model) typically augments a DEM (Digital Elevation Model), by including vector features of the natural terrain, such as rivers and ridges.

* What is DEM (Digital Elevation Model)?

	- A DEM (Digital Elevation Model) Represents the bare-Earth surface, removing all natural and built features.

* What is CHM (Canopy Height Model)?

	- to derive a CHM is to take the difference between the digital surface model (DSM, tops of trees, buildings and other objects) and the Digital Terrain Model (DTM, ground level). The CHM represents the actual height of trees, buildings, etc. with the influence of ground elevation removed.

* What are shapefiles?

	- The shapefile format is a geospatial vector data format for geographic information system (GIS) software. It is developed and regulated by Esri as a mostly open specification for data interoperability among Esri and other GIS software products.

	- The shapefile format can spatially describe vector features: points, lines, and polygons, representing, for example, water wells, rivers, and lakes. Each item usually has attributes that describe it, such as name or temperature.

	From the dataset we have 6 files with .dbf .sbn .shp .prj .sbx .shx, upon researching, 

	ArcGIS shapefiles have mandatory and optional files. The mandatory file extensions needed for a shapefile are .shp, .shx and .dbf. But the optional files are: .prj, .xml, .sbn and .sbx

	example:
	DHMVII_vdc_k01.dbf  DHMVII_vdc_k01.sbn  DHMVII_vdc_k01.shp
	DHMVII_vdc_k01.prj  DHMVII_vdc_k01.sbx  DHMVII_vdc_k01.shx

	Main File (.SHP)

	.shp is a mandatory Esri file that gives features their geometry. Every shapefile has its own .shp file that represent spatial vector data. For example, it could be points, lines and polygons in a map.

	Index File (.SHX)

	.shx are mandatory Esri and AutoCAD shape index position. This type of file is used to search forward and backwards.

	dBASE File (.DBF)

	.dbf is a standard database file used to store attribute data and object IDs. A .dbf file is mandatory for shape files. You can open .DBF files in Microsoft Access or Excel.

	Projection File (.PRJ)

	.prj is an optional file that contains the metadata associated with the shapefiles coordinate and projection system. If this file does not exist, you will get the error “unknown coordinate system”. If you want to fix this error, you have to use the “define projection” tool which generates .prj files.

	Spatial Index File (.SBN)

	.sbn is an optional spatial index file that optimizes spatial queries. This file type is saved together with a .sbx file. These two files make up a shape index to speed up spatial queries.

	Spatial Index File (.SBX)

	.sbx are similar to .sbn files in which they speed up loading times. It works with .sbn files to optimize spatial queries. When tested with .sbn and .sbx extensions and it was found that there were faster load times when these files existed. It was 6 seconds faster (27.3 sec versus 33.3 sec) compared with/without .sbn and .sbx files.

	Extensible Markup Language File (.XML)

	.xml file types contains the metadata associated with the shapefile. If you delete this file, you essentially delete your metadata. You can open and edit this optional file type (.xml) in any text editor.
	
	https://gisgeography.com/arcgis-shapefile-files-types-extensions/

	* What is geographic information system (GIS)?

	- A geographic information system (GIS) is a framework for gathering, managing, and analyzing data. Rooted in the science of geography, GIS integrates many types of data. It analyzes spatial location and organizes layers of information into visualizations using maps and 3D scenes.

* What are geoTIFFs files?

	- GeoTIFFs files are raster image file types that are commonly used to store satellite and aerial imagery data, along with geographic metadata that describes the location in space of the image.  

	* What is a Raster?
	- Raster or “gridded” data are stored as a grid of values which are rendered on a map as pixels. Each pixel value represents an area on the Earth’s surface. 


* What is GDAL?

	- GDAL (Geospatial Data Abstraction Library) is the de facto standard library for interaction and manipulation of geospatial raster data. The primary purpose of GDAL or a GDAL-enabled library is to read, write and transform geospatial datasets in a way that makes sense in the context of its spatial metadata. GDAL also includes a set of command-line utilities (e.g., gdalinfo, gdal_translate) for convenient inspection and manipulation of raster data.




	