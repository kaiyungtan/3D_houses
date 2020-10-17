# Background information

The Digital Elevation Model Flanders (DHMV) is the collective name for all area-wide elevation data of Flanders available to the AGIV. 

The DHMV II constitutes the update of the DHMV I created in the period 2001-2004. 

For years, the acquisition technology has evolved significantly, many changes have occurred in Flemish landscape and new applications increasingly require a larger one detail degree.

The DHMV II is characterized by a high level of detail and includes data for the territory of the Flemish Region, including a buffer of 5 km and the Brussels-Capital Region. This product takes the first step towards Flanders in 3D.

The standard derivatives (DTM and DSM) are offered via transfer service in smaller units, respectively, representing data per 1/1 NGI map sheet (topographic map sheet of the National Geographic Institute at scale 1 / 50,000) (32 km x 20 km). Articles include geographic relationship exactly match and do not overlap. Every product becomes gradual open as the data becomes available per map sheet.

All geographic data is in Belgian Lambert 72 projection.

Both projection and georeference are documented in the geoTIFF file.

The height values ​​are referred to the Second General Leveling and are expressed in meters with centimeter precision.



## DSM

Digital surface model (DSM, 'digital surface model') of the ground level including objects
in grid format with a ground resolution of 1 meter. This DSM was derived from LiDAR elevation data provided within the framework of the Digital Elevation Model Flanders II (DHMV II).

This product is supplemented with an object 'flying day contour DHMV' that for each part of the DSM the accurate recording data.

The product is collected over the period 2013-2015 and will be released gradually. The object 'stand of cases DHMV II 'indicates where data is already available.

Purpose of manufacture: The raster format DSM is a derivative of the source data 'LiDAR Digital Altitude model Flanders II - raw remote sensing data '. 

The grid format allows this product in use a wide range of applications without the need for specific software.

The DSM is suitable for the representation and modeling of the ground level and the objects located on it to be.


### Limitation

Geographic boundary description: current boundary
Geographic boundary identifier: Flemish Region and Brussels-Capital Region 

Minimum longitude: 2.54154 °
Maximum longitude: 5.92 °
Minimum latitude: 50.6756 °
Maximum latitude: 51.51 °


## General description of origin: Digital Elevation Model Flanders II (DHMV II)

Description: Elevation data acquisition using LiDAR technology from an aircraft.
The resulting point cloud has an average point density of at least 8 points per m2 per
flight lane, in which there is in flight a transverse overlap of at least 50% between adjacent ones flying strips are provided.

Description: Processing of the point cloud into source data with the following characteristics: 
absolute planimetric accuracy: RMSExy less than or equal to 0.10m
absolute altimetric accuracy: RMSEz less than or equal to 0.05m 
filtering between the classes: 'ground level', 'water' and 'not ground level'

Description: Creation of the DSM based on the 'ground level' and 'off ground level' highlights with using the interpolation algorithm “streaming TINs via spatial finalization &streaming Delaunay” (http://www.cs.berkeley.edu/~jrs/papers/tin2dem.pdf).

Description: Creation of the raster file with the following specifications: 
format: geoTIFF
data type: 32bit float 
pixel resolution: 1m 
NoData Value: -9999 
compression: no 
pyramids: no 
colormaps: no


## DTM

Digital terrain model (DTM) of the ground level in grid format with a ground resolution of 1
meter. This DTM was derived from LiDAR elevation data provided in the context of the Digital Elevation Model Flanders II (DHMV II) were recruited.

This product is supplemented with an object 'flight day contour DHMV' that for each part of the DTM the accurate recording data.

The product is collected over the period 2013-2015 and will be released gradually. The object 'stand of cases DHMV II 'indicates where data is already available.

Purpose of manufacture: The DTM in raster format is a derivative of the source data 'LiDAR Digital Altitude model Flanders II - raw remote sensing data '. The grid format allows this product in use a wide range of applications without the need for specific software.

The DTM is suitable for the representation and modeling of the ground level.



Filename 			Format  	Description

<codeObject>.shp 	shp 		file containing the geometry of the object 

<codeObject>.shx 	shx 		file with the index of the geometry

<codeObject>.dbf 	dbf 		file with the attributes of the object

<codeObject>.prj 	prj 		file about the reference system for ArcGIS 

<codeObject>.shp.xml xml		file with metadata for ArcGIS


“GeoTIFF” contains the raster file.

 
<Projected CRS: EPSG:31370>

Name: Belge 1972 / Belgian Lambert 72
Axis Info [cartesian]:
- X[east]: Easting (metre)
- Y[north]: Northing (metre)
Area of Use:
- name: Belgium - onshore
- bounds: (2.5, 49.5, 6.4, 51.51)
Coordinate Operation:
- name: Belgian Lambert 72
- method: Lambert Conic Conformal (2SP)
Datum: Reseau National Belge 1972
- Ellipsoid: International 1924
- Prime Meridian: Greenwich


<Geographic 2D CRS: EPSG:4326>
Name: WGS 84
Axis Info [ellipsoidal]:
- Lat[north]: Geodetic latitude (degree)
- Lon[east]: Geodetic longitude (degree)
Area of Use:
- name: World
- bounds: (-180.0, -90.0, 180.0, 90.0)
Datum: World Geodetic System 1984
- Ellipsoid: WGS 84
- Prime Meridian: Greenwich

