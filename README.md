## DESCRIPTION

### Branch A - Short term rental / Airbnb - New York City
The Dataset contains data related to the short-term rental market in New York City. The primary objective of this study is to unveil significant trends sought-after neighborhoods, rental prices and property types. The aim is to offer an overview, catering to both potential inverstors seeking to venture into this business model and individuals planning a short stay in the city. By doing so, they can gain insights into estimated budgets and optimal choices tailored to their specific requirements.

## WORKFLOW

1. The database was made available in an open SQL server - ElephantSQL (Credentials inside the python file)
2. Data cleaning, primary visualization, and transformation were done using Python (Libraries used: Numpy - Pandas - Matplotlip - Seaborn)
3. Final data visualization, dashboarding, and providing business insights using Tableau Public

Files:

1. Jupyter notebook: Preliminary analysis over the dataset, uncovering general trends and tendencies of the data.
2. Tableau link: Visualization and analysis of rental trends and behaviors. Two dashboards were generated to provide an interactive tool for analyzing short-term rentals in city
[Tableau: Short Rental Review](https://public.tableau.com/views/NYcity-ShortRentalReview/PriceReview?:language=en-US&:display_count=n&:origin=viz_share_link)

## General Overview

Relational Database, formed by 3 tables (Price, Reviews and Room Type) with the data of around 25000 distinct listings from January 2019 to July 2019.

Listings are categorized according to the Borough (Brooklyn, Manhattan, Queens, Bronx, Staten Island) and Neighbourhood they belong to in the city of New York. 

Initially, it was found that the Boroughs of Brooklyn and Manhattan possess around 80% of the total places listed. As well as, Private rooms and entire homes are the predominant type of listings avaliable, they represent the 97% of them. 

Aditionally, it was ideintified that the price/night distribution is right-skewed, meaning that there are listings overpassing the 1000 USD a night. However, the most frequent price falls between 50 to 200 USD/night, which also cover the 70% of the data available.

<div style="display:flex; flex-direction: row;">
    <img src="https://raw.githubusercontent.com/luis12pez/Tableau-viz/A---Short-Rental-NYC/Histo-price.png" alt="Histogram-Price" style="width:40%;">
    <img src="https://raw.githubusercontent.com/luis12pez/Tableau-viz/A---Short-Rental-NYC/cumm-distri-price.png" alt="Cumulative-Distribution" style="width:50%;">
</div>

In terms of average prices, the Borough of Manhattan doubles most of the other boroughs, which is coherent with the fact that the borough is the center of tourism in the city. Additionally, as expected, the entire home type of room is the most expensive.

| borough        | Average price (USD/month) | Room type    | Average Price (USD/month) |
|----------------|---------------|-----------------|---------------|
| Manhattan      | 5600   | entire home/apt | 6000   |
| Brooklyn       | 3700   | private room    | 2500   |
| Queens         | 2800   | shared room     | 1600   |
| Staten Island  | 2600   |
| Bronx          | 2400   |

Having a quick look at the monthly variation in prices does not reveal a clear seasonality. However, some price increments are seen as summer approaches 

<div style="display:flex; flex-direction: row;">
    <img src="https://raw.githubusercontent.com/luis12pez/Tableau-viz/A---Short-Rental-NYC/price-variation.png" alt="Price Variation" style="width:100%;">
</div>


Finally, by following the Tableau link provided earlier, two interactive dashboards can be accessed. These dashboards allow users to interact with the available data.

The "Price Review" dashboard offers users the ability to investigate pricing behavior across the dataset. Whether the user is planning a visit to the city or considering investing in real estate, this dashboard provides an overall view per borough and neighborhood in terms of price distribution. It enables users to identify affordable and/or expensive regions, as well as the types of accommodations available for rent based on different budgets.

Some key points are
         
- 95% of the listed accommodations fall within the price range of $40 to $300 per night
- Entire home/apartment rentals typically range from $40 to $300 per night, while private rooms are in between $40 and $200 per night. On the other hand, the shared room option is the most affordable, with prices mostly below $100 per night
- Brooklyn and Manhattan have the highest number of listings available and also tend to have the most expensive rentals per night (reaching max. prices up to $7500 and $5100, respectively)
- Staten Island and the Bronx are the areas where you can find affordable rentals (max. prices of $600 and $300, respectively)
         
Additionally, "Review-Price-Availability" dashboard offers additional insights for users, including listing availability for the upcoming year and the impact of reviews on pricing and already booked nights. This information is particularly valuable for individuals interested in operating short-term rentals in the city.

Some key points are

- Not only the amount of reviews will impact in the price of the rental. But also factors, such as longevity of the place as rental, room type and amenities offered.
- Some rentals do not need many reviews in order to be at high rental price. As mention before, could be given by time renting, room type and amenities offered, but also, due to the location. It is well known that this area of New York city is one of the more exclusive (Business and Turistic nature)
- Nights booked vs price relationship will depend on the location of the rental and the type of room offered
- NY is a highly visited city, either for business or turisim. There will be always a fairly occupancy rate for any rental available, as it is shown in the histogram at the bottom right. Being Mahattan and Brooklyn, the areas which attract more guests

### [Go Back](https://github.com/luis12pez/Tableau-viz)
