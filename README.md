# Analyze Airbnb Data

This scripts use the Airbnb data from Seattle and Boston to answer a few questions about the availability and price of Airbnb homes and analyze the most features that impact on Airbnb price. 
The code is designed to gather, assess, clean and analyze the data in order to answer the following questions:
- Which is the period with less available Airbnbs in Seattle? And in Boston?
- Which city has the average higher price for AirBnb?
- Which is the most rented property in Seattle? And for Boston?
- Which is the most important feature regarding the AirBnb price?

A full post was written in Medium and it is available [here](https://gregorymarchesan.medium.com/what-most-affects-the-airbnb-prices-in-us-cities-38b0fa1c492a). 

To sum up, using data from Airbnb from cities as Seattle and Boston, we realized that Boston has an availability of properties lower than Seattle and a higher price also. Further, the analysis showed up that there are a lot of properties rented all over the period in Boston, much more than in Seattle.
Additionally, although our prediction model was not perfect, it gives a reasonable idea of the price of Airbnbs and we found out that the most important features in the price are the city, number of bedrooms and type of rooms.

## Instalation

The code runs in Python 3.7.3 and requires the following libraries:
- Numpy (1.16.2)
- Pandas (0.24.2)
- Sklearn (0.20.3)
- XGBoost (1.3.3)
- Plotly (4.14.3)
- Glob (0.6)
- Tqdm (4.31.1)

## File Description

The data used is available in raw_data folder, and is compiled with the '\_[city]' to tell the script what city are we talking about. This is an extensible feature, once you can use for other cities as well. Additionally, there are 3 .csv files for each city:
- listing.csv: A dataset containing the main information (e.g. number of rooms, price, fees, etc) to each property in that city.
- calendar.csv: A dataset containing the information about the property's availability all over the period.
- reviews.csv: A dataset containing the review information about each property. This dataset, although imported, will be not used in this post and work.

Once the script runs, it merge the files from different cities in one dataframe for each purpose, generating 3 datasets (listing, calendar, reviews).

## Acknowledgements & Licensing

The code provided here is free to use and it is under MIT Licensing.

