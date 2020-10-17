# 3D_houses

to model a house in 3D with only a home address

## Mission objectives

Consolidate the knowledge in Python, specifically in :

- [X] NumPy
- [X] Pandas
- [X] Matplotlib


## Learning Objectives

- [X] to be able to search and implement new librairies
- [X] to be able to read and use shapefiles
- [X] to be able to read and use geoTIFFs
- [X] to be able to render a 3D plot
- [X] to be able to present a final product


## The Mission

We are LIDAR PLANES , active in the Geospatial industy. We would like to use our data to launch a new branch in the insurrance business. So, we need you to build a solution with our data to model a house in 3D with only a home address.


## Must-have features

3D lookup of houses.


## Nice-to-have features

- [X] Optimize your solution to have the result as fast as possible.
- [ ] Features like the living area of the house in m², how many floors, if there is a pool, the vegetation in the neighborhood, etc...
- [ ] Better visualization.


## Step

- [X] Research and understand the term, concept and requirement of the project.

	* What are the requirements ?

	- to model a house in 3D with only a home address

	- with those points clouds we can easily identify houses, vegetation, roads, etc...The results we're insterested in are DSM (Digital Surface Map) and DTM (Digital Terrain Map).

- [X] Use geopy to convert physical addresses to Geographic locations → Latitude and Longitude

- [X] Use folium map to show the the address on the map 

- [X] Create belgium houses addresses with coordinate from opendata.bosa.be website 

- [X] Discover new libraries that can be used to render a 3D plot

	* glob - to search all file with the same extension
	* geopy - convert physical addresses to Geographic locations
	* folium - plot address on a map
	* rasterio -  read and write GEOTIFF format file 
	* pyproj - performs cartographic transformations and geodetic computations
	* rioarray - rasterio xarray extension (xarray - working with labelled multi-dimensional arrays)
	* imageio - interface to read and write a wide range of image data
	* matplotlib (mpl_toolkits.mplot3d Axes3D) - plot 3D objects on a 2D matplotlib figure 
	* Mayavi -  provide easy and interactive visualization of 3D data
	
- [ ] Others 3D plotting libraries 
	* pptk (Point Processing Toolkit)
	* open3d
	* vtk
	* pyntcloud


### Challenges

* due to limit hard disk - unable to have all the data - Flandre data (80GB) and Wallonie data (100GB) on the same place

* after updating macOS Catalina version 10.15.7, Anaconda-Navigator did not work. Have to reinstall Anaconda-Navigator and all libraries for this project.

* Ran into problem reinstall mayavi , in order for mayavi to work on python 3.8 have to brew install vtk
 