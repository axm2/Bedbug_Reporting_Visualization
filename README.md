Bedbug Reporting Visualization
-----------------------

Visualizes the bedbug infestation history using deck.gl

#### Get data from API
The data for this project was provided by [NYC Open Data](https://opendata.cityofnewyork.us/)

Specificially,

https://data.cityofnewyork.us/Housing-Development/Bedbug-Reporting/wz6d-d3jb

https://data.cityofnewyork.us/City-Government/New-York-City-Population-By-Neighborhood-Tabulatio/swpk-hqdp

https://data.cityofnewyork.us/dataset/nynta/q2z5-ai38

#### Build and display bedbug map
The bedbug map was displayed using [deck.gl](https://deck.gl/#/) from Uber's data visualization team

A heatmap was used to show the hotspots of bedbug infestations

![](https://i.imgur.com/5REt8aH.png)

#### Build and display population density map

A population density dataset wasn't available, but a dataset for population by neighborhood tabulation was available

So, the dataset and the map had to be combined, normalized, and then mapped to a polygon layer that was overlayed on top of our previous heatmap

![](https://i.imgur.com/t73ygSm.png)

#### Toggle menu
Finally, using ipywidgets a dropdown menu was made to allow the user to toggle the layers on and off and easily observe the correlation.

![](https://i.imgur.com/8hDK6Cp.png)

![](https://i.imgur.com/5O6uz7e.png)

Installation
----------------------

### Download

* Clone this repo to your computer.
* In your terminal, run export MAPBOX_API_KEY=<mapbox-key-here\> which pydeck will read to use Mapbox basemaps. You can also refer to the pydeck docs to see how to pass the key as a variable.
* Open and run the notebook

### Install the requirements
 
* You will need to install pydeck, pandas, sodapy

Extending this
-------------------------

If you want to extend this work, here are a few places to start:

* Generate more layers 
  * Rental vs Owned
  * Property value
  * Education level
  * Proximity to park
  * Proximity to hospital
  * Proximity to schools
  
* Narrow down dataset to a specific year
* Check how bedbug infestation trends over the years
* Compare to weather changes
