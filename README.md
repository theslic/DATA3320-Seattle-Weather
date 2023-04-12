# DATA3320 Seattle Weather
The purpose of the project is to get started with Python and using pandas to clean our data to make it easier to work with
and to learn about the different ways to visualize data though tables and other forms of visualizations.
We got the data from https://github.com/brian-fischer/DATA-3320 which is our professor's data files that we will be using.
These were taken from an other online source NOAA site.
seattle_rain.csv and stl_rain.csv are datasets on rainfall.

Data Preparation - To clean the data I first looked for the columns I was most interested in such as date and precipitation.
Then I checked for any missing or invalid values, once discovering them I imputed them using the mean for that
day across all the years, now not affecting my calculation as much. I also joined the tables on the date and precipitation
columns. Then I created a new column to the dataframe that would be true or false wether the precipitation for that day was
0 or not. This column 'zero_precip' is whether it rained that day or not as a boolean. Now the new cleaned data is a table with the day, month, year, precipitation, city, and zero_precip.

The file that prepares the data is: Li_Copy_DATA_3320_Seattle_St_Louis_Data_Preparation.ipynb
The file with the data is: clean_seattle_stl_weather.csv

Data Analysis - In the analysis I am trying to answer the questions of which city rains more often and which city has larger amounts of rainfall when it does rain. My first exploratory plot was a histogram of the amounts of rainfall where we saw that most of the rainfalss was on the lower end. We also made a histogram counting the number of days it did rain and the days it did not. We then used the information to create 2 new high definition plots where one displays the average amount of rainfall by month and city while the other is the number of days without rain by month and city.
