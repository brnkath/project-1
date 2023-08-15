# project-1

Contributors: Alex Calametti, Katy Yelle, Raeshawn Mcallister, and Brian Kath

## Repository Structure - 

	- Main folder
		- README.md
		- .gitignore
		- Airbnb.ipynb
		- Airbnb_Scatterplots.ipynb
		- Airbnb_analysis_chart.ipynb
		- Airbnb_analysis_hvplots.ipynb
		- Airbnb_analysis_stats.ipynb

	- Sub-folders
		- output
			- clean_2020.csv
			- clean_2023.csv
			- per_city_2023.csv
		- resources
			- AB_US_2020.csv
			- AB_US_2023.csv
		- images
			- 2020scatterplot1.png
			- 2020scatterplot2.png
			- 2020scatterplot3.png
			- 2020scatterplot4.png
			- 2023scatterplot1.png
			- 2023scatterplot2.png
			- 2023scatterplot3.png
			- 2023scatterplot4.png
			- Hvplots.png
			- fig1_2020.png
			- fig1_2023.png
			- fig2_2020.png
			- fig2_2023.png

## Overview - 
	-Airbnb

	-Airbnb Scatterplots

	-Airbnb_analysis_chart

	-Airbnb_analysis_hvplots

	-Airbnb_analysis_stats

## Written Analysis -
This project analyzes Airbnb data from three different cities (New York City, San Francisco and Twin Cities Metro Area).  We chose these cities to compare cities of various population sizes and housing markets. 

With our analysis we seek to answer the questions: (1) What factors have the greatest impact on listing prices (such as location, reviews, listing types, etc.); and (2) How has the average price of Airbnb's changed from 2020 to 2023?

Through analyzing scatterplot data we determined that factors such as number of listings per host, availability of a listing, minimum nights per stay for a listing and number of reviews did not correlate with listing prices. 

Based on hvplots for each city and year location within a city generally has an impact on price.  Higher prices tend to be concentrated in particular areas especially where there is a higher density of listings. Unfortunately our data sources differed with drilled down location data (one with zip codes while the other had neighborhood names) so we were not able to drill down more into this trend. 

In 2020, the Twin Cities Metro Area had the highest average prices for three of the four listing types (Entire Home/Apt, Private Room, and Shared Room). Overall, the Twin Cities had the highest average price of Airbnb listings, followed by San Francisco, followed by New York City. The higher average prices in the Twin Cities in 2020 is likely due to the Super Bowl taking place that impacting area Airbnb prices.  In 2023, San Francisco had the highest average prices for all four listing types (Entire home/apt, Hotel room, Private room, and Shared Room).  Average prices per listing decreased in the Twin Cities (excpet for Hotels), average prices increased in all types for both New York and San Francisco.

Slide Deck
https://docs.google.com/presentation/d/1oWesPYfvMPgw-zK6yMqtW0Pb8tgWv-btZPZEQP_CLzY/edit?usp=sharing
