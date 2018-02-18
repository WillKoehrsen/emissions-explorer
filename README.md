# Interactive Data Visualization of Global CO2 Emissions

[Try it Out](http://emissions.online.s3-website.us-east-2.amazonaws.com/)

(Only tested on Chrome browser on desktop!)

## Motivation

The Emissions Explorer is an interactive application designed to illustrate the 
potential of data visualization to derive knowledge from data.
Everyone - corporations, governments, individuals - has data, but very few people 
know what to do with it. All these numbers contain useful information that can improve 
lives but often it is inaccessible. One issue is that most often the data looks like this: 

![image](https://raw.githubusercontent.com/WillKoehrsen/emissions-explorer/master/static/img/emissions_images/raw_data.png)

Endless spreadsheet rows full of numbers with no meaning in their current form. There
is nothing wrong with spreadsheets, and as a data scientist, I spend much of time 
my time working with and extracting data from them. However, they don't really 
speak to people and it's difficult to convince someone to take action based on those rows and columns.
The cliche is that a picture is worth 1000 words and the data version is that a good visualization
is worth millions of individual numbers. My objective with the emissions explorer is to take 
publically available data that currently is hidden in spreadsheets and make it widely accessible. 
By using free tools - with plenty of resources for learning online - we can take these 
meaningless figures and turn them into useful knowledge through effective visualizations. 

## Features

The Emissions Explorer has 3 main parts:

![image](https://raw.githubusercontent.com/WillKoehrsen/emissions-explorer/master/static/img/emissions_images/map.PNG)

1. Global Map: Displays historical emissions of all countries with available data 
on a world map. Circles on the country are sized according to the amount of CO2 emitted
and colored by the rank. The map can be animated to show all the years in sequence or
a specific year can be selected. Tooltips that appear on mouseover show the emissions,
rank for that year, and country name. 

![image](https://raw.githubusercontent.com/WillKoehrsen/emissions-explorer/master/static/img/emissions_images/chart.PNG)

2. Top 15 Chart: Shows the Top 15 CO2 emitting countries historical emissions. The world
is also shown for comparion. The y-axis automatically scales to the data (this took a long
time to figure out in d3) and tooltips on mouseover show the CO2 emissions for that year.

![image](https://raw.githubusercontent.com/WillKoehrsen/emissions-explorer/master/static/img/emissions_images/socio.PNG)

3. Demographic and Emissions Trends: Presents 4 pieces of information for the 
top 15 emitting countries on one chart. The y-axis is GDP per capita (a measure of a country's wealth),
the x-axis is population,the size of the circles is the amount of emissions 
(area of the circle is proportional to emissions), and the color indicates the 
country's rank for that year. The graph automatically transitions through all the years (1850-2014)
and a year also can be selected by moving the cursor over the year on the graph. Text displays the 
name of the country and the rank for that country. 



