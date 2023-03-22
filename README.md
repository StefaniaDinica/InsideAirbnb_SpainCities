# InsideAirbnb_SpainCities
The purpose of this project is to analyse and compare the prices of accommodations in Madrid and Barcelona.

The data is provided by http://insideairbnb.com/get-the-data/ and is organized in two folders with the names of the cities.

## Data cleanup
  Two data sets are used in this project, one for Madrid and one for Barcelona.
  Each set is composed of **listings.csv** and **calendar.csv** files, that are extracted into separate dataframes.
  
  Several steps are done in order to clean the data:
  1. Filter and keep only the data in [2022-03-10, 2023-03-10] interval
  2. Keep the listings with maximum 3 bedrooms
  3. For listings with NaN values in bedroom column, replace those values with 0 (consider that those properties are studios)
  4. Drop null prices
  5. Format the prices in order to be numeric
  6. Filter and keep only the prices in [5$, 1000$] interval
  
## Availability insights
The average availability of accommodations grouped by month is calculated for both cities and the result is the following plot:
<img src="/assets/availability.png" alt="Availability plot" style="height: 100px; width:100px;"/>

## Price insights
- Price per month
The average price of accommodations grouped by month is calculated for both cities and the result is the following plot:
- Price per month for studios
The average price of studios grouped by month is calculated for both cities and the result is the following plot:
- Price per month for 1 bedroom properties
The average price of 1 bedroom properties grouped by month is calculated for both cities and the result is the following plot:
- Price per month for 2 bedrooms properties
The average price of 2 bedrooms properties grouped by month is calculated for both cities and the result is the following plot:
- Price per month for 3 bedrooms properties
The average price of 2 bedrooms properties grouped by month is calculated for both cities and the result is the following plot:
- Price per month for all property types in Madrid
The average price for all property types in Madrid grouped by month is calculated for both cities and the result is the following plot:
- Price per month for all property types in Barcelona
The average price for all property types in Barcelona grouped by month is calculated for both cities and the result is the following plot:
- Price per city zone
Using the latitude and the longitude, I created the scatter plot of the listings in Madrid and 5 city zones:

The average price for all property types in Madrid grouped by city zone and the result is the following plot:

Using the latitude and the longitude, I created the scatter plot of the listings in Barcelona and 5 city zones:

The average price for all property types in Barcelona grouped by city zone and the result is the following plot:

## Used libraries
- Pandas
- Matplotlib



