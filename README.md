# World_Weather_Analysis

**Data Analyst at PyBer**
Create line, bar, scatter, bubble, pie, and box-and-whisker plots using Matplotlib. And determine mean, median, and mode using Pandas, NumPy, and SciPy statistics.

## Overview of Project
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
* Explain the purpose of the new analysis:

    > The purpose of this written report for Data Analyst at PyBer is to create a complete summary of the Ride-Sharing data by city type. Including a quick summary of line, bar, scatter, bubble, pie, and box-and-whisker plots using Matplotlib libraries. And determine mean, median, and mode using Pandas, NumPy, and SciPy statistics. Our Final Analysis include multiple-line graphs of total weekly fares for each city type.


2. **The latitude and longitude pairs for each of the four cities are retrieved.** 
* Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types:
  
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