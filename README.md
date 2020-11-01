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

We are LIDAR PLANES , active in the Geospatial industy. We would like to use our data to launch a new branch in the insurrance business. So, we need you to build a solution with our data to model a house in 3D with only a home address.The results we're insterested in are DSM (Digital Surface Map) and DTM (Digital Terrain Map).


## Must-have features

3D lookup of houses.


## Nice-to-have features

- [X] Optimize your solution to have the result as fast as possible.
- [X] Better visualization
- [X] 3D Belgium's monuments i.e Château,Royal Place,Abbaye,Cathédrale etc...

## Process Flow

![image](https://user-images.githubusercontent.com/69633814/97796615-638c6100-1c14-11eb-8c03-2ad258c66999.png)

## Research

- [X] Research and understand the term, concept and requirement of the project.

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
	
## Data Collecting

- [X] DTM file for Flandre including Brussels: http://bit.ly/DTM_Flandre
- [X] DSM file for Flandre including Brussels: http://bit.ly/DSM_Flandre
- [X] DTM file for Wallonie: http://bit.ly/DTM_Walloine_2013-2014
- [X] DSM file for Wallonie: http://bit.ly/DSM_Wallonie_2013-2014
- [X] BeST: Geographical coordinates with addresses in Belgium: https://opendata.bosa.be/index.fr.html
- [X] CSV Flandres - https://opendata.bosa.be/download/best/openaddress-bevlg.zip
- [X] CSV Région de Bruxelles - https://opendata.bosa.be/download/best/openaddress-bebru.zip
- [X] CSV Wallonie - https://opendata.bosa.be/download/best/openaddress-bewal.zip

## Data Cleaning

- [X] Create belgium houses addresses with coordinate from opendata.bosa.be website 

	* Result : http://bit.ly/Belgium_Addresses	


## Data Processing 

- [X] Use geopy to convert physical addresses to Geographic locations → Latitude and Longitude
- [X] Use folium map to show the the address on the map 
- [X] The diagram below describe the flow of the process where the input is the address of the house and the output is the 3D plot of the house.

![image](https://user-images.githubusercontent.com/69633814/97796724-e235ce00-1c15-11eb-9ba0-b708831f8961.png)

## Data Visualization

- [X] Plot 3D houses only with flandres dataset.

	* https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Flandre_Beernem.html

- [X] Plot 3D houses only with wallonie dataset.


	* https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Wallonie_Wavre.html

- [X] Combined both dataset to produce one single way to render 3d houses regardless where the houses are located.

	
	* https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_houses/Project_3D_Houses_Belgium_Arlon.html


- [X] Plot 3D monuments in Belgium

	* https://kaiyungtan.github.io/3D_houses/Examples_Code_3D_monuments/Project_3D_Monument_Royal_Palace_of_Brussels.html
	

![image](https://user-images.githubusercontent.com/69633814/97797278-0e544d80-1c1c-11eb-81ab-abf183b62ed0.png)

![image](https://user-images.githubusercontent.com/69633814/97797286-1d3b0000-1c1c-11eb-9846-50763163e2ce.png)

![image](https://user-images.githubusercontent.com/69633814/97797269-fb417d80-1c1b-11eb-82bb-0b0177882a3a.png)

![image](https://user-images.githubusercontent.com/69633814/97797295-288e2b80-1c1c-11eb-8e27-183e56893e96.png)


## Challenges

* to convert an address to a latitude,longtitude coordinate 

* to search the existing tif and determine which tif contain the coordinate

* to clip the tif with certain window size to allow rendering in 3D  

* to use new libraries to render a 3D plot 

* unable to host all the data - Flandre data (80GB) and Wallonie data (100GB) on the same place (due to limit of storage)

* after updating macOS Catalina version 10.15.7, Anaconda-Navigator did not work and have to reinstall Anaconda-Navigator and all libraries for this project.

* after reinstall mayavi , mayavi did not work on python 3.8. Upon investigating, found out that have to install vtk in order for mayavi to work.


## Limitation

* due to the buffer zone of each tif file, some houses can be located on 2 tifs.

* geocoding of address to coordinates sometime did not give the correct location of the houses

* belgium addresses.csv may not be able to provide the coordinate for the address in question, due to the address provided may not actually the same as indicated in the csv or address has been removed during the cleaning process of the data.

* new houses after 2014 are not shown on the tif due to the fact the tif was dated 2014.

## Further Development

* to host the data on an online server.
* to develop web application allowing client to type in any address in belgium to view 3D houses.
* to obtain latest LIDAR images so that new houses after 2014 can be rendered.
* to incorparate cadastral plan of each property in the 3D rendering so that only the requested house is rendered.
* to explore other 3D plotting libraries
