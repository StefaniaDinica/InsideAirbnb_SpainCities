# InsideAirbnb_SpainCities
The purpose of this project is to analyse and compare the prices of accommodations in Madrid and Barcelona.

The data is provided by http://insideairbnb.com/get-the-data/ and is organized in two folders with the names of the cities.

## Content
1. [Data cleanup](#data-cleanup)
2. [Availability insights](#availability-insights)
3. [Price insights](#price-insights)
    *  [Price per month](#price-per-month)
    *  [Price per month for studios](#price-per-month-studios)
    *  [Price per month for 1 bedroom properties](#price-per-month-1bd)
    *  [Price per month for 2 bedrooms properties](#price-per-month-2bd)
    *  [Price per month for 3 bedrooms properties](#price-per-month-3bd)
    *  [Price per month for all property types in Madrid](#price-per-month-all-md)
    *  [Price per month for all property types in Barcelona](#price-per-month-all-bc)
    *  [Price per city zone in Madrid](#price-per-zone-md)
    *  [Price per city zone in Barcelona](#price-per-zone-bc)

## <a name='data-cleanup'>1. Data cleanup</a>
  Two data sets are used in this project, one for Madrid and one for Barcelona.
  Each set is composed of **listings.csv** and **calendar.csv** files, that are extracted into separate dataframes.
  
  Several steps are done in order to clean the data:
  - Filter and keep only the data in [2022-03-10, 2023-03-10] interval
  - Keep the listings with maximum 3 bedrooms
  - For listings with NaN values in bedroom column, replace those values with 0 (consider that those properties are studios)
  - Drop null prices
  - Format the prices in order to be numeric
  - Filter and keep only the prices in [5$, 1000$] interval
  
##  <a name='availability-insights'>2. Availability insights</a>
The average availability of accommodations grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/availability.png" alt="availability plot" style="height: 400px; width:400px;"/>

## <a name='price-insights'>3. Price insights</a>
- <a name='price-per-month'>Price per month</a>

The average price of accommodations grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/prices.png" alt="prices plot" style="height: 400px; width:400px;"/>

- <a name='price-per-month-studios'>Price per month for studios</a>

The average price of studios grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/md_vs_bc_studios.png" alt="md_vs_bc_studios plot" style="height: 400px; width:400px;"/>

- <a name='price-per-month-1bd'>Price per month for 1 bedroom properties</a>
The average price of 1 bedroom properties grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/md_vs_bc_1bd.png" alt="md_vs_bc_1bd plot" style="height: 400px; width:400px;"/>

- <a name='price-per-month-2bd'>Price per month for 2 bedrooms properties</a>
The average price of 2 bedrooms properties grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/md_vs_bc_2bd.png" alt="md_vs_bc_2bd plot" style="height: 400px; width:400px;"/>

- <a name='price-per-month-3bd'>Price per month for 3 bedrooms properties</a>
The average price of 3 bedrooms properties grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/md_vs_bc_3bd.png" alt="md_vs_bc_3bd plot" style="height: 400px; width:400px;"/>

- <a name='price-per-month-all-md'>Price per month for all property types in Madrid</a>
The average price for all property types in Madrid grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/md_all_prices.png" alt="md_all_prices plot" style="height: 400px; width:400px;"/>

- <a name='price-per-month-all-bc'>Price per month for all property types in Barcelona</a>
The average price for all property types in Barcelona grouped by month is calculated for both cities and the result is the following plot:

<img src="/plots/bc_all_prices.png" alt="bc_all_prices plot" style="height: 400px; width:400px;"/>

- <a name='price-per-zone-md'>Price per city zone in Madrid</a>
Using the latitude and the longitude, I created the scatter plot of the listings in Madrid and 5 city zones:

<img src="/plots/md_scatter.png" alt="md_scatter plot" style="height: 400px; width:400px;"/>

The average price for all property types in Madrid grouped by city zone and the result is the following plot:

<img src="/plots/md_zones_avg.png" alt="md_zones_avg plot" style="height: 400px; width:400px;"/>

- <a name='price-per-zone-bc'>Price per city zone in Barcelona</a>
Using the latitude and the longitude, I created the scatter plot of the listings in Barcelona and 5 city zones:

<img src="/plots/bc_scatter.png" alt="bc_scatter plot" style="height: 400px; width:400px;"/>

The average price for all property types in Barcelona grouped by city zone and the result is the following plot:

<img src="/plots/bc_zones_avg.png" alt="bc_zones_avg plot" style="height: 400px; width:400px;"/>

## Used libraries
- Pandas
- Matplotlib



