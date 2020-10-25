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
    * 1. Latitude and longitude
    * 2. Maximum temperature
    * 3. Percent humidity
    * 4. Percent cloudiness
    * 5. Wind speed
    * 6. Weather description (for example, clouds, fog, light rain, clear sky)


2. Add the weather data to a new DataFrame
3. Export the DataFrame as WeatherPy_Database.csv into the Weather_Database folder

 
### Results with detail analysis:

**1. The total number of rides for each city type is retrieved.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.1.PNG?raw=true)

**2. The total number of drivers for each city type is retrieved.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.2.PNG?raw=true)

**3. The sum of the fares for each city type is retrieved.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.3.PNG?raw=true)

**4. The average fare per ride for each city type is calculated.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.4.PNG?raw=true)

**5. The average fare per driver for each city type is calculated.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.5.PNG?raw=true)

**6. A PyBer summary DataFrame is created.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.6.PNG?raw=true)

**7. The PyBer summary DataFrame is formatted as shown in the example.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.7.PNG?raw=true)



### Deliverable 2: A multiple-line chart of total fares for each city type
### Deliverable Requirements:

1. A DataFrame was created using the `groupby()` function on the "type" and "date" columns, and the `sum()` method is applied on the "fare" column to show the total fare amount for each date and time.
2. A DataFrame was created using the `pivot()` function where the index is the "date," the columns are the city "type," and the values are the "fare."
3. A DataFrame was created using the `loc` method on the date range: 2019-01-01 through 2019-04-29.
4. A DataFrame was created using the `resample()` function in weekly bins and shows the sum of the fares for each week.
5. An annotated chart showing the total fares by city type is created and saved to the "analysis" folder. 


### Results with detail analysis:

**1. A DataFrame was created using the `groupby()` function on the "type" and "date" columns, and the `sum()` method is applied on the "fare" column to show the total fare amount for each date and time.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/2.1.PNG?raw=true)

**2. A DataFrame was created using the `pivot()` function where the index is the "date," the columns are the city "type," and the values are the "fare."**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/2.2.PNG?raw=true)

**3. A DataFrame was created using the `loc` method on the date range: 2019-01-01 through 2019-04-29.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/2.3.PNG?raw=true)

**4. A DataFrame was created using the `resample()` function in weekly bins and shows the sum of the fares for each week.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/2.4.PNG?raw=true)

**5. An annotated chart showing the total fares by city type is created and saved to the "analysis" folder.**

> Image with `Jupyter Notebook` & `Python` Code below.

**Code and Image**

![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/2.5.PNG?raw=true)



## Deliverable 3: A written report for the PyBer Analysis
### The analysis should contain the following:

1. **Overview of the analysis** 
* Explain the purpose of the new analysis:

    > The purpose of this written report for Data Analyst at PyBer is to create a complete summary of the Ride-Sharing data by city type. Including a quick summary of line, bar, scatter, bubble, pie, and box-and-whisker plots using Matplotlib libraries. And determine mean, median, and mode using Pandas, NumPy, and SciPy statistics. Our Final Analysis include multiple-line graphs of total weekly fares for each city type.


2. **Results** 
* Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types:

    > * The Suburban fares started around $1,000, and the analysis was not profitable, fare dropped in March and in mid-April.  
    > * The Rural fares started at around $200, the analysis shows fares increase and dropped till the end of April.  
    > * The Urban fares start with an average of $1,800 with a consistent increase around 2,300. 
    
    > The PyBer summary DataFrame, 
    ![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/1.7.PNG?raw=true)

     > A multiple-line chart of total fares for each city type,
    ![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/Resources/Images/2.5.PNG?raw=true)

     > PyBer Ride-Sharing Data (2019), 
    ![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/analysis/Fig1.png?raw=true)      

3. **Summary** 
* Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types:

    > **1)** From our analysis, we can predict that there are good opportunities to expand the business in rural and suburban cities, including hiring drivers to operate and explode business in rural and suburban cities.

    > % of Total Drivers by City Type,
    ![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/analysis/Fig7.png?raw=true)
    
    > **2)** The Urban cities fare is the highest and consistent, giving us great and new business opportunities to expand rides.  

    > % of Total Fares by City Type, 
    ![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/analysis/Fig5.png?raw=true)
    
    > **3)** The Rural cities fare is the lowest of the other two city types (Urban and Suburban cities), in addition, fares never intersect.  Knowing that all fares never intersect, we can expand fares and increase business financial income to the company without affecting our rate.

     > Total Fare by City Type,
    ![name-of-you-image](https://github.com/emmanuelmartinezs/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png?raw=true) 


#### PyBer Analysis Completed by Emmanuel Martinez