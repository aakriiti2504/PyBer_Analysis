# PyBer_Analysis
Analysis of a ride-sharing summary DataFrame of a ride sharing company PyBer.

## Overview:
As a data analyst for PyBer, a python based ride sharing app company, the first assignment is
to perform an exportory analysis on data in some CSV files. To aid the process, several types
of visualizations to tell a compelling story about the data will be created..

## Background:
It's my second week as a data analyst at PyBer, a ride-sharing app company valued at $2.3 billion.
I have just been assigned my first big project: analyze all the rideshare data from January to early
May of 2019 and create a compelling visualization for the CEO, V. Isualize.

Even before starting at PyBer,I had heard stories about V. Isualize. She is a former programmer who 
started out at MathWorks, a co-founder of PyBer, and is known for being extremely fair yet extremely 
demanding. Because of her programming expertise, she's particularly insistent that the analytical work
be comprehensive and correct. This assignment is both a once-in-a-lifetime challenge and a once-in-a-lifetime 
opportunity. My aim is to work on this project and bring out taccurate results.

My manager, Omar, is excited for my big break and has agreed to partner with me on getting the 
visualizations just right. As a new employee, this is a huge professional opportunity for me.



## Tools Used:

We will use Python scripts using Panda's libraries,Jupyter Notebook and MAtplotlib to create a variety of charts to showcase the relationship between the type of city and number of drivers and riders as well as the percentage of total fares, riders and drivers by type of city. Python graphing library Matplotlib is a favorite tool among data scientists and data analysts because of its robust visualization features. Matplotlib is a graphing and plotting library for Python that comes with the Anaconda installation. To use it with Jupyter Notebook, all we need to do is import it. Matplotlib is often used with another Python library, NumPy, a numerical mathematics library for making arrays or matrices. Using Pandas and Jupyter notebook we will inspect data, merge datasets, perform mathematical calculations and create data series and dataframes.

Omar has given me some backstory about the connection between V. Isualize and Matplotlib. Matplotlib was created as a Python alternative for MATLAB. MATLAB, which is short for matrix laboratory, was developed by the company MathWorks in the 1980s. It enabled scientists to perform linear algebra and numerical analysis without learning the programming language Fortran, which until then had been the best option for complex computations.


## Matlplotlib:
Matplotlib is a 2D plotting library. It also has rich styling options. One can customize annotations for chart axes, titles and legends, the color and size of lines, bars, and bubbles, and the chart's background. It also lets you save and print publication-quality charts. Because of these features, Matlplotlib is one of the most popular plotting libraries for Python. With matplotlib we can produce publication quality figures of various data series that tell a visual story from data. This presents complex findings in a way thats informative and engaging to all stakeholders. Data visualizations allow th eaudience to absorb information quickly that is difficult to do by just browsing large tabular datasets.
Matplotlib has two methods for graphing data. One uses MATLAB's plotting syntax and functionality and the other uses an object-oriented interface. MATLAB's plotting syntax is concise and the most useful when creating simple plots that require little coding. This method is most effective when graphing data directly from a DataFrame. The object-oriented method is better suited to more complicated graphs that require more coding, such as those with multiple lines or bars, or multiple plots in one graph. Here, we'll use Matplotlib's plotting methods in the Jupyter Notebook environment with data from the ride-sharing dataset. 


## Purpose:
The amount of analysis and visualizations produced will help PyBer improve access to ridesharing services and determine affordability for under served neighborhoods. This analysis consists of two technical deliverables and a written report presenting results on:
#### - A ride sharing summary DataFrame by city type, and
#### - A multiple -line chart of total fares for each city type.

## Scope:
Omar has approved the following project scope:
- Import your data into a Pandas DataFrame.
- Merge your DataFrames.
- Create a bubble chart that showcases the average fare versus the total number of rides with bubble size based on the total number of drivers for each city type, including urban, suburban, and rural.
- Determine the mean, median, and mode for the following:
	- The total number of rides for each city type.
	- The average fares for each city type.
	- The total number of drivers for each city type.
- Create box-and-whisker plots that visualize each of the following to determine if there are any outliers:
	- The number of rides for each city type.
	- The fares for each city type.
	- The number of drivers for each city type.
- Create a pie chart that visualizes each of the following data for each city type:
	- The percent of total fares.
	- The percent of total rides.
	- The percent of total drivers.

## Procedure:
1) A github reposirtory PyBer_Analysis is created so that I can share project details with Omar and other colleagues.
2) Checked the version of Matlplotlib library 
3) Omar has suggested that I start with one of the most common charts: a line chart. I will also be commenting on my code. This way, if he or the CEO wants to take a look at the repo, they'll know exactly what I am  doing and whether I am heading in the right direction.
4) Also, its important to inspect the data before starting the analysis. On opening the city_data.csv, it can be found out that there are three columns, city, driver_count and type. It can be noticed that there are 121 rows in total in the excel file. Inspecting further, we notice that each column has a header. each row has a city that has a driver_count and type of city that can be rural, suburban or urban. We also note that there are no empty rows. Once we add this csv file into a Pandas dataframe, we will be able to determine the data type for each column. On opening the ride_data.csv file we can note that there are 4 columns- city, date, fare and ride_id. There are in all 2376 rows. each column has a header. Each row contains a city that has a date when the ride was taken, the fare fpr the ride and a 12 to 13 digit ride identification number. We will use pandas to determine if there are empty rows and the data type for each column.
5) In Deliverable 1, Adding the Matplotlib inline command and loading and reading the data from .csv files.

![1](https://user-images.githubusercontent.com/23488019/143162145-ae81bf8d-dd00-4367-a9f5-0d484eeefbe0.PNG)

6) Getting the total rides, drivers, amount of fares average fare per ride for each city type.

![2](https://user-images.githubusercontent.com/23488019/143162204-a787e8dc-d2c8-4a43-b91f-e918ba2984b5.PNG)

7) Getting the average fare per driver and the PyBer summary dataframe. Next we clean up the dataframe and delete the index name

![3](https://user-images.githubusercontent.com/23488019/143162223-3ed762ee-a151-469e-8a4b-d560a2c4e25e.PNG)

8) Formatting the columns and having comma separators as well as $ sign where needed.

![4](https://user-images.githubusercontent.com/23488019/143162234-4c918f21-d54e-4cae-9ee8-374f420de4f3.PNG)

9) In deliverable 2, reading the merged dataframe and using groupby() to create a new dataframe showing the sum of the fares for each date where the indices are the city type and date.

![5](https://user-images.githubusercontent.com/23488019/143162243-c7373e61-959d-4500-aa34-7d6ea4bb8972.PNG)

10) Resetting the index on the dataframe created in deliverable 1.

![6](https://user-images.githubusercontent.com/23488019/143162261-eecb33ab-996a-4093-9577-1c72a18e45e1.PNG)

11) Creating a pivot table with date as index to get the total fares for each type of city by the date.

![7](https://user-images.githubusercontent.com/23488019/143162281-f876ca0a-350a-4dce-9489-49410db0f8c6.PNG)

12) Creating a new dataframe from the pivot table dataframe using loc on the given dates.

![8](https://user-images.githubusercontent.com/23488019/143162301-b95d0eeb-360a-432e-9adb-3365556048f1.PNG)

13) Checking that the datatype for the index is datetime using df.info(). Next we create a new dataframe using the resample() function by week and get the sum of the fares for each week.

![51](https://user-images.githubusercontent.com/23488019/143735918-728496b9-41de-410e-a677-f355bf2411fe.PNG)


14) Plotting the resample Dataframe using the df.plot() function using the object oriented interface method.

![52](https://user-images.githubusercontent.com/23488019/143735910-b942dd1b-2bc7-4d0d-b35c-7132bee405cf.PNG)


## Results:
The various differences in the ride-sharing data among different city types are discussed here. The ride sharing data include the total rides, total drivers, total fares, average fare per driver and ride and total fare by city type.
Using the various functions in Pandas, we could come up with the PyBer dataframe to calculate the total number of rides, fares, drivers and calculate various averages and totals. We formatted the dataframe and obtained the following result:
![62](https://user-images.githubusercontent.com/23488019/143762915-27207038-e09f-455d-8a6a-601503830dfe.PNG)

From the dataframe created, it can be observed that:
- The urban cities have the maximum amount of rides and drivers, hence fares. The rural cities however have the least. As a result the urban city types bring in the most revenue and rural bring in the least.
- It can be also noted that the drivers in the rural areas make 1/3rd of what the drivers make in the urban city types.
- The urban fares start with an average of $1800 with a consistent increase around $2300. Suburban starts at $1000 approx and the fare dropped in March and mid April. Hence the analysis was not profitable. In rural areas, fare started around $200 and the fares increased and then dropped until the ned of April.
- There are 13 times more number of rides in urban areas than in the rural areas. There are 30 times more number of drivers in the urban areas as compared to the rural areas. Also, there is a possibility of making 9 times the total revenue in urban areas as compared to rural areas.
- Rural cities have the highest average fare per driver representing 49% of the average fare per driver or $55 average fare per driver.Suburban cities have the second highest average fare per driver representing 36% of the average fare per driver or $40 average fare per driver. Urban cities have the least average fare per driver representing 15% of the average fare per driver or $17 average fare per driver.
- Rural cities have the highest average fare per ride representing 39% of the average fare per ride or $35 average fare per ride.Suburban cities have the second highest average fare per ride representing 34% of the average fare per ride or $31 average fare per ride. Urban cities have the least average fare per ride representing 27% of the average fare per ride or $24 average fare per ride


A bubble chart was created initially where the circle size correlates with the driver count per city. It was noted here that the urban city types have the highest driver counts and the total number of rides. Also, the rural aresa had the lowest of these values and suburban were a mid range performing city type.The average number of rides in rural cities are also lowest than in urban and suburban city types.
![Fig1](https://user-images.githubusercontent.com/23488019/143763133-1e3a43d4-a04c-42ca-84d1-f8ffaa824bd6.png)
 
 The box and whisker chart displays the city types and the number of rides. This shows that there is least number of rides in rural areas and the most in urbana areas. This can be because of less need in rural areas as compared to the urban areas.
 
 ![Fig2](https://user-images.githubusercontent.com/23488019/143763126-d595e79f-87da-4530-aaa9-4a531a4d8890.png)




 A multiple line chart was created after the dataframe creation using the object-oriented interface method and the df.plot() method and the matplotlib. The resampled dataframe was graphed to obtaing the line chart as shown in the graph. This line chart helps in visualizing and performing analysis of the total Fares from the month of January 2019 to April 2019 for each of the three city types.
 
![52](https://user-images.githubusercontent.com/23488019/143746870-d82a83e2-6906-4e3a-9c56-58df04165aa6.PNG)

From the above line graph it can be observed that:
- The urban cities had the highest total fares for all the months and weeks and the rural city type had the least of the fares generated.
- The third week of February has the highest number of fares for all the three city types. This shows that there was an increased demand in the ride sharing activities.


## Summary: 
Based on the results,  atleast three business recommendations to the CEO for addressing any disparities among the city types are discussed below:
- 1)There is a great potential to increase the revenue in rural as well as suburban areas if the number of drivers working in these two city types are increased. The urban cities have 80.9% drivers, however the rural and suburban have 2.6% and 16.5% drivers respectively. Hence, it can be concluded that there are opportunities to expand business in these areas. More special rates and deals need to be introduced in these areas. Also, there is a need to recruit more drivers in there so that under served areas can have access to more comfortable and frequent ride sharing facilities.

![53](https://user-images.githubusercontent.com/23488019/143736089-f785f088-1bbd-4e39-9e29-e0425ae06563.PNG)


- 2)Few attractive special event or weekly special deals can be introduced as a measure to increase the sales. The graph shows that there is not much difference in the fares hence PyBer can work on special fares and deals to attract more customers to use PyBer and this increase the total sales of the company.


- 3)The maximum number of rides are currently in the urban city type. Hence PyBer can increase their fares by little to get more profit as the ride traffic is much more and steady in the urban areas. Increasing fare based on per mile can be introduced initially to see change in total profit. 
- 4)Another way could be to reduce the number of drivers a little in the urban areas so that the fares could be increased and there is more utilization of resources with the headcount reduction. More drivers can be encouraged to drive in the rural areas. It can be seen that the drivers in urban are not at a100% utilization hence efforts should be made towards more utilization of drivers.

![54](https://user-images.githubusercontent.com/23488019/143763785-bdab7933-eb7c-4c72-8987-d493ad9fb41d.PNG)

- 5)The suburban city type are medium performing type and extra efforts can abe added to improve the business in this category too. More investments can be made to increase the performance in these areas.

These observations can be very helpful in finding the disparities in the fares for different city types and provide a foundation to plan steps ahead so that ride sharing can be more affordable as well as accessible in all the three city types.
