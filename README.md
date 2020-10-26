# World Weather Analysis

## Basic Project Plan
Here's an outline of your project plan:

* ***Task:*** Collect and analyze weather data across cities worldwide.
* ***Purpose:*** PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.
* ***Method:*** Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail collecting, analyzing, and visualizing the data.
Your analysis of the data will be split into three main parts, or stages.

1. Collect the Data

* Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
* Use the citipy module to list the nearest city to the latitudes and longitudes.
* Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
* Parse the JSON data from the API request.
* Collect the following data from the JSON file and add it to a DataFrame:
    * City, country, and date
    * Latitude and longitude
    * Maximum temperature
    * Humidity
    * Cloudiness
    * Wind speed

2. Exploratory Analysis with Visualization

* Create scatter plots of the weather data for the following comparisons:
    * Latitude versus temperature
    * Latitude versus humidity
    * Latitude versus cloudiness
    * Latitude versus wind speed
* Determine the correlations for the following weather data:
    * Latitude and temperature
    * Latitude and humidity
    * Latitude and cloudiness
    * Latitude and wind speed
* Create a series of heatmaps using the Google Maps and Places API that showcases the following:
    * Latitude and temperature
    * Latitude and humidity
    * Latitude and cloudiness
    * Latitude and wind speed

3. Visualize Travel Data

Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:

* Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
* Create a heatmap for the new DataFrame.
* Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
* Store the name of the first hotel in the DataFrame.
* Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.

## Projec Summary
Jack loves the PlanMyTrip app. Beta testers love it too. And, as with any new product, they’ve recommended a few changes to take the app to the next level. Specifically, they recommend adding the weather description to the weather data you’ve already retrieved in this module. Then, you'll have the beta testers use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, you will create a travel route between the four cities as well as a marker layer map. 

> This new assignment consists of three technical analyses. You will submit the following deliverables:

1. ***Deliverable 1***: Retrieve Weather Data
2. ***Deliverable 2***: Create a Customer Travel Destinations Map
3. ***Deliverable 3***: Create a Travel Itinerary Map

Including a [`README.md`](https://github.com/emmanuelmartinezs/PyBer_Analysis). 

## Resources and Before Start Notes:

* Data Source: `PyBer_Challenge_starter_code.ipynb` named later as `PyBer_Challenge.ipynb`
* Data File: file.csv
* Software: Matplotli 3.2.2, Python 3.9, Visual Studio Code 1.50.0, Anaconda 4.8.5, Jupyter Notebook 6.1.4, Pandas

For more information, read the [`Documentation on Python data typess`](https://docs.python.org/3.6/library/stdtypes.html#numeric-types-int-float-complex). 

## Review the Geographic Coordinate System

We use the **geographic coordinate system (GCS)** to reference any point on Earth by its latitude and longitude coordinates.

**Latitudes** are imaginary lines on Earth that run parallel east to west and are measured in angular units called degrees, minutes, and seconds, with 60 minutes in a degree and 60 seconds in a minute. Sometimes a latitude is referred to as a **parallel**. Consider, for example, the embattled 38th parallel (38° north) in East Asia that roughly demarcates North Korea and South Korea.

The **equator** is an imaginary line around the middle of the earth that is equidistant from the North and South Poles and has a latitude of 0°. The equator splits Earth into Northern and Southern Hemispheres.

Lines of latitude on Earth run east to west.

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/l1.png?raw=true)

All latitude lines above the equator are measured northward and considered positive, after 0° (the equator) and up to 90°, or 90° north (the North Pole). All latitude lines below the equator are measured southward and considered negative, before 0° (the equator) and down to –90°, or 90° south (the South Pole).

The equator splits Earth into the Northern and Southern hemispheres, with positive north and negative south latitudes.

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/l2.png?raw=true)

**Longitudes** are imaginary lines on Earth that run from the North to the South Poles and are called ****meridians**. The **prime meridian** represents zero meridian, the origin for longitude coordinates, and splits Earth into the Eastern and Western Hemispheres.

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/l3.png?raw=true)

The prime meridian passes through Greenwich, England, from which longitude east and west is measured.

The marker of the prime meridian in Greenwich,England

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/l4.png?raw=true)

All meridians east of the prime meridian are considered positive, after 0° and up to 180°. All meridians west of the prime meridian are considered negative, before 0° and down to –180°.

The prime meridian splits Earth into the Eastern and Western
hemispheres, with positive eastern and negative western
longitudes.

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/l5.png?raw=true)

All together, the lines of latitude (parallels) and longitude (meridians) make up a geographic grid, as if the Earth were wrapped in graph paper with intersecting horizontal and vertical lines mapping to specific locations.

GCS makes it possible to pinpoint any place on Earth by providing its precise address, which is the intersection of its latitude and longitude lines.

Longitude and latitude lines intersect and form a geographic grid
system across the Earth's
surface.


## Deliverable 1:  Retrieve Weather Data
Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.

### Deliverable Requirements:

1. Retrieve all of the following information from the API call:
    1. Latitude and longitude
    2. Maximum temperature
    3. Percent humidity
    4. Percent cloudiness
    5. Wind speed
    6. Weather description (for example, clouds, fog, light rain, clear sky)


2. Add the weather data to a new DataFrame
3. Export the DataFrame as WeatherPy_Database.csv into the Weather_Database folder

 
### Results with detail analysis:

**1. Retrieve all of the following information from the API call.**


**1.i. Latitude and longitude.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**1.ii. Maximum temperature.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**1.iii. Percent humidity.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**1.iv. Percent cloudiness.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**1.v. Wind speed.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**1.vi. Weather description (for example, clouds, fog, light rain, clear sky).**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)


**2. Add the weather data to a new DataFrame.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)


**3. Export the DataFrame as `WeatherPy_Database.csv` into the Weather_Database folder**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

### Deliverable 2: Create a Customer Travel Destinations Map.
Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

### Deliverable Requirements:

1. Input statements are written to prompt the customer for their minimum and maximum temperature preferences.
2. A new DataFrame is created based on the minimum and maximum temperature, and empty rows are dropped.
3. The hotel name is retrieved and added to the DataFrame, and the rows that don’t have a hotel name are dropped.
4. The DataFrame is exported as a CSV file into the Vacation_Search folder and is saved as `WeatherPy_vacation.csv`.
5. A marker layer map with pop-up markers for the cities in the vacation DataFrame is created, and it is uploaded as a PNG. Each marker has the following information:
    1. Hotel name
    2. City
    3. Country
    4. Current weather description with the maximum temperature
6. The marker layer map is saved and uploaded to the Vacation_Search folder as `WeatherPy_vacation_map.png`.

### Results with detail analysis:

**1. Input statements are written to prompt the customer for their minimum and maximum temperature preferences.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**2. A new DataFrame is created based on the minimum and maximum temperature, and empty rows are dropped."**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**3. The hotel name is retrieved and added to the DataFrame, and the rows that don’t have a hotel name are dropped.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**4. The DataFrame is exported as a CSV file into the Vacation_Search folder and is saved as `WeatherPy_vacation.csv`.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5. A marker layer map with pop-up markers for the cities in the vacation DataFrame is created, and it is uploaded as a PNG. Each marker has the following information:**


**5.i. Hotel name**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5.ii. City**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5.iii. Country**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5.iv. Current weather description with the maximum temperature**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)


**6. The marker layer map is saved and uploaded to the Vacation_Search folder as `WeatherPy_vacation_map.png`.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)


## Deliverable 3: Create a Travel Itinerary Map
Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

### Deliverable Requirements:

1. Four DataFrames are created, one for each city on the itinerary. 
2. The latitude and longitude pairs for each of the four cities are retrieved. 
3. A directions layer map between the cities and the travel map is created and uploaded as `WeatherPy_travel_map.png`. 
4. A DataFrame that contains the four cities on the itinerary is created.
5. A marker layer map with a pop-up marker for the cities on the itinerary is created, and it is uploaded as `WeatherPy_travel_map_markers.png`. Each marker has the following information: 
    1. Hotel name
    2. City
    3. Country
    4. Current weather description with the maximum temperature


### The analysis should contain the following:

1. **Four DataFrames are created, one for each city on the itinerary** 
Explain the purpose of the new analysis:

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)


2. **The latitude and longitude pairs for each of the four cities are retrieved.** 
Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types:
  
**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)
   

3. **A directions layer map between the cities and the travel map is created and uploaded as `WeatherPy_travel_map.png`.** 
types:
  
**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)
    

 4. **A DataFrame that contains the `four` cities on the itinerary is created.** 
types:
  
**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)
    
 **5. A marker layer map with a pop-up marker for the cities on the itinerary is created, and it is uploaded as `WeatherPy_travel_map_markers.png`. Each marker has the following information:**


**5.i. Hotel name**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5.ii. City**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5.iii. Country**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)

**5.iv. Current weather description with the maximum temperature**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/World_Weather_Analysis/blob/main/Resources/Images/demo.PNG?raw=true)


#### World Weather Analysis Completed by Emmanuel Martinez