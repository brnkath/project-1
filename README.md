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
		- Airbnb_HypothesisTests.ipynb
		- Airbnb_analysis_datadescription.ipynb
  		- data_pulling.ipynb

	- Sub-folders
		- output
  			- average_price_per_listing.csv
     			- average_price_per_listing_2020.csv
			- average_price_per_listing_2023.csv
			- clean_2020.csv
			- clean_2023.csv
   			- per_city_2020.csv
			- per_city_2023.csv
   			- summary_data.csv
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
   			- boxplot_w_2k_ylim.png
			- fig1_2020.png
			- fig1_2023.png
			- fig2_2020.png
			- fig2_2023.png

## Overview - 
	-Airbnb
	Imports, prepares and cleans the data.  Narrows down the data to the 3 focus cities (New York City, San Francisco, Twin Cities Metro), removes unneccessary columns and reorganizes and renames remaining colums.  Removed all listings with zero days of availability.  Resets the index.  Exports the dataframe to csv. 

	-Airbnb Scatterplots
	Creates scatterplots for price and each of the numerical variables in the datasets (number of listings per host, days of availability, minimum nights per stay for a listing and number or reviews), runs a linear regression and calculates the r-value. 

	-Airbnb_analysis_chart
	Creates bar charts of the average listing prices for each city. 

	-Airbnb_analysis_hvplots
	Creates maps of each city for each year (2020 and 2023) taking a sample of 1000 random listings and plots them with marker colors indicating the type of listing (Entire home/apartment, Private room, Shared room or Hotel Room) and marker size indicating the price of the listing. 

	-Airbnb_analysis_stats
	Creates summary statistics (mean, median and mode) of price for each city and year. Creates box and whisker plots of prices for each city and year. 

	-Airbnb_HypothesisTests
	Conducts a one-way ANOVA for each year for listing types and for cities. 

	-Airbnb_analysis_datadescriptions
	Calculates data descriptions for all numerical data pieces for each year and city (number of listings per host, price, days of availability, minimum nights per stay for a listing, number of reviews)

## Written Analysis -
This project analyzes Airbnb data from three different cities (New York City, San Francisco and Twin Cities Metro Area).  We chose these particular cities to compare cities of various population sizes and housing markets. 

With our analysis we seek to answer the questions: (1) What factors have an impact on listing prices (such as location, reviews, listing types, etc.); and (2) How has the average price of Airbnb's changed from 2020 to 2023?

Based on hvplots for each city and year, we determined location within a city generally has an impact on price.  Higher prices tend to be concentrated in particular areas especially where there is a higher density of listings. Unfortunately our data sources differed as far as more specific location data (2020 data included zip codes while 2023 had neighborhood names) so we were not able to provide further analysis on this trend when comparing the two years. Additional data sources that include housing prices in these cities would be a topic for further analysis and study.

Through analyzing scatterplot data and linear regressions we determined that factors such as number of listings per host, availability of a listing, minimum nights per stay for a listing and number of reviews did not correlate with listing prices. 

Analyzing summary statistics and box and whisker plots we were able to see that the data in all cities is skewed by high priced outliers.  In 2020, New York City had a total of 25,648 listings with prices ranging from $10-$10,000 with an average price of $157.28. In 2023, New York City had a total of 28,941 listings with prices ranging from $10-$99,000 and average price of $218.03. In 2020, San Francisco had a total of 5438 listings with prices ranging from $10-$10,000 and average price of $202.77.  In 2023, San Francisco had a total of 5967 listings with prices ranging from $26-$25,000 and an average price of $324.52.  In 2020, the Twin Cities metro area had a total of 3902 listings with prices ranging from $10-$15,000 and an average price of $364.55.  In 2023, the Twin Cities metro area had a total of 4161 listings with prices ranging from $17-$9,900 and an average price of $181.99. 

Through datatables and bar graphs we were able to analyze average price based on listing types and city location for each year.  In 2020, the Twin Cities Metro Area had the highest average prices for three of the four listing types (Entire Home/Apt, Private Room, and Shared Room). Overall, the Twin Cities had the highest average price of Airbnb listings ($364.55), followed by San Francisco ($202.77), followed by New York City ($157.28). The higher average prices in the Twin Cities in 2020 is likely due to the Super Bowl taking place that year impacting area Airbnb prices due to greater demand.  In 2023, San Francisco had the highest average prices for all four listing types (Entire home/apt, Hotel room, Private room, and Shared Room).  Overall, San Francisco had the highest average price of Airbnb listings ($324.52), followed by New York City ($218.03), followed by the Twin Cities ($181.99). From 2020 to 2023, average prices per listing decreased for each listing type in the Twin Cities (except for Hotel rooms); while average prices increased for all listing types for both New York and San Francisco.

A one-way analysis of variance (ANOVA) compared the average price based on Listing Type (Entire home/apt, Private room, Shared room and Hotel Room) for each year's data.  The tests were found to be statistically significant with a pvalue < .01 for both 2020 and 2023 data. Another one-way analysis of variance (ANOVA) compared the average price based on City (New York City, San Francisco, Twin Cities MSA) for each year's data.  The tests were found to be statistically significant with pvalues < .01 for both 2020 and 2023 data. Therefore we can conclude both Listing Type and City have a statistically significant impact on Airbnb listing prices. 

In summary, we have concluded that city, location within a city and listing types all have an impact on an Airbnb's price.  Whereas other factors such as number of listings per host, minimum nights per stay, days of availability and number of reviews did not correlate with prices of listings.  From 2020 to 2023, average prices per listing decreased for each listing type in the Twin Cities (except for Hotel rooms); while average prices increased for all listing types for both New York and San Francisco.

Slide Deck
https://docs.google.com/presentation/d/1oWesPYfvMPgw-zK6yMqtW0Pb8tgWv-btZPZEQP_CLzY/edit?usp=sharing
