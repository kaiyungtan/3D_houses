# 3D_houses

to model a house in 3D with only a home address

img src="https://github.com/kaiyungtan/3D_houses/blob/master/4.%203D%20House%20Images/3D_house_logo.png?raw=true"

https://kaiyungtan.github.io/3D_houses/

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
- [X] Better visualization
- [X] 3D Belgium's monuments i.e Château,Royal Place,Abbaye,Cathédrale etc...


## What are the requirements ?

	- to model a house in 3D with only a home address

	- with those points clouds we can easily identify houses, vegetation, roads, etc...The results we're insterested in are DSM (Digital Surface Map) and DTM (Digital Terrain Map).

## Step

- [X] Research and understand the term, concept and requirement of the project.

- [X] Use geopy to convert physical addresses to Geographic locations → Latitude and Longitude

- [X] Use folium map to show the the address on the map 

- [X] Create belgium houses addresses with coordinate from opendata.bosa.be website 

	* Result : http://bit.ly/Belgium_Addresses

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
	
- [X] Explore others 3D plotting libraries 
	* pptk (Point Processing Toolkit) - for visualizing and processing 2-d/3-d point clouds
	* open3d  - A Modern Library for 3D Data Processing
	* vtk (Visualization Toolkit) - for 3D computer graphics image processing and visualization.
	* pyntcloud - or working with 3D point clouds

- [X] Plot 3D houses only with flandres dataset.

https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Flandre_Beernem.html

- [X] Plot 3D houses only with wallonie dataset.


https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Wallonie_Wavre.html

- [X] Combined both dataset to produce one single way to render 3d houses regardless where the houses are located.

https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Belgium_Arlon.html

https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Belgium_Brecht.html

https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Belgium_Dinant.html

https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Belgium_Galmaarden.html

https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Belgium_Gent.html

### Diagram

<table style="width: 100%;" >
<tbody>
<tr>
<td>
<img src="https://github.com/kaiyungtan/3D_houses/blob/main/3.%20Diagram/3D_Houses_Belgium_Diagram_rev4.png">
</td>
</tr>
</tbody>
</table>


### Challenges

* to convert an address to a latitude,longtitude coordinate 

* to search the existing tif and determine which tif contain the coordinate

* to clip the tif with certain window size to allow rendering in 3D  

* to use new libraries to render a 3D plot 

* unable to host all the data - Flandre data (80GB) and Wallonie data (100GB) on the same place (due to limit of storage on machintosh)

* after updating macOS Catalina version 10.15.7, Anaconda-Navigator did not work and have to reinstall Anaconda-Navigator and all libraries for this project.

* after reinstall mayavi , mayavi did not work on python 3.8. Upon investigating, found out that have to install vtk in order for mayavi to work.


### Limitation

* due to the buffer zone of each tif file, some houses can be located on 2 tifs.

* geocoding of address to coordinates sometime did not give the correct location of the houses

* belgium addresses.csv may not be able to provide the coordinate for the address in question, due to the address provided may not actually the same as indicated in the csv or address has been removed during the cleaning process of the data.

* new houses after 2014 are not shown on the tif due to the fact the tif was dated 2014.










 