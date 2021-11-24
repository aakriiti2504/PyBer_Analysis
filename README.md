# PyBer_Analysis


## Overview:
As a data analyst for PyBer, a python based ride sharing app company. The first assignment is
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
4) In Deliverable 1, Adding the Matplotlib inline command and loading and reading the data from .csv files.

![1](https://user-images.githubusercontent.com/23488019/143162145-ae81bf8d-dd00-4367-a9f5-0d484eeefbe0.PNG)

5) Getting th etotal rides, drivers, amount of fares average fare per ride for each city type.

![2](https://user-images.githubusercontent.com/23488019/143162204-a787e8dc-d2c8-4a43-b91f-e918ba2984b5.PNG)

6) Getting the average fare per driver and the PyBer summary dataframe. Next we clean up the dataframe and delete the index name

![3](https://user-images.githubusercontent.com/23488019/143162223-3ed762ee-a151-469e-8a4b-d560a2c4e25e.PNG)

7) Formatting the columns and having comma separators as well as $ sign where needed.

![4](https://user-images.githubusercontent.com/23488019/143162234-4c918f21-d54e-4cae-9ee8-374f420de4f3.PNG)

8) In deliverable 2, reading the merged dataframe and using groupby() to create a new dataframe showing th esum of the fares for each date where the indices are the city type and date.

![5](https://user-images.githubusercontent.com/23488019/143162243-c7373e61-959d-4500-aa34-7d6ea4bb8972.PNG)

9) Resetting the index on the dataframe created in deliverable 1.

![6](https://user-images.githubusercontent.com/23488019/143162261-eecb33ab-996a-4093-9577-1c72a18e45e1.PNG)

10) Creating a pivot table with date as index to get the total fares for each typ eof city by the date.

![7](https://user-images.githubusercontent.com/23488019/143162281-f876ca0a-350a-4dce-9489-49410db0f8c6.PNG)

11) Creating a new dataframe from the pivot table dataframe using loc on the given dates.

![8](https://user-images.githubusercontent.com/23488019/143162301-b95d0eeb-360a-432e-9adb-3365556048f1.PNG)

12) Checking that the datatype for the index is datetime using df.info(). Next we create a new dataframe using the resample() function by week and get the sum of the fares for each week.

![9](https://user-images.githubusercontent.com/23488019/143162332-e036de0c-6e53-4f52-921f-b22ada32b4b9.PNG)

13) Plotting the resample Dataframe using the df.plot() function using th eobject oriented interface method.

![10](https://user-images.githubusercontent.com/23488019/143162348-03da2f3e-89c1-42f0-bef6-f1800ca57d98.PNG)

## Results:


## Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types
