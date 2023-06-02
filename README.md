# P01_Explore-weather-trends
This is the project for the first module from the Data Analyst Nanodegree at Udacity.

## Project Overview
This is the first project in the Nanodegree and consists of a smooth introduction 
to data analysis. Here students had to **make a comparison of weather trends at 
local and global levels.** To accomplish this, Udacity provided us with three tables 
in a database, `city_list` with a list of cities and countries, `city_data` with 
the average temperatures for each of these cities by year, and `global_data` 
containing the average global temperatures annually.

I extracted the weather data for both city and global levels using this SQL query:
```
SELECT g.year, g.avg_temp global_temp, c.city, c.avg_temp city_temp
FROM global_data g
JOIN city_data c
ON c.year = g.year
WHERE g.year >= 1851 AND g.year <= 2013 AND c.city = ‘Rio De Janeiro’
```
After that, I exported the data as CSV and opened it in Excel to wrangle and produce 
a data visualization for analysis. The final product is the [report](https://github.com/affonsociekalski/P01_Explore-weather-trends/blob/main/Report_project-1.pdf) in this repository where you will find a more complete description of my project.

## Technologies Used
* Excel
* SQL
* InDesign

## Author
* Affonso Ciekalski Soares Campos

## License
<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.
 
