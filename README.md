## DESCRIPTION

### Branch A - Short term rental / Airbnb - New York City
The Dataset contains data related to the short-term rental market in New York City. The primary objective of this study is to unveil significant trends sought-after neighborhoods, rental prices and property types. The aim is to offer an overview, catering to both potential inverstors seeking to venture into this business model and individuals planning a short stay in the city. By doing so, they can gain insights into estimated budgets and optimal choices tailored to their specific requirements.

## WORKFLOW

1. The database was made available in an open SQL server - ElephantSQL (Credentials inside the python file)
2. Data cleaning, primary visualization, and transformation were done using Python
3. Final data visualization, dashboarding, and providing business insights using Tableau

Files:

1. Jupyter notebook: Preliminary analysis over the dataset, uncovering general trends and tendencies of the data.
2. Tableau link: Visualization and analysis of rental trends and behaviors. Two dashboards were generated to provide an interactive tool for analyzing short-term rentals in city
[Tableau: Short Rental Review](https://public.tableau.com/views/NYcity-ShortRentalReview/PriceReview?:language=en-US&:display_count=n&:origin=viz_share_link)

## EXECUTIVE SUMMARY

General
Relational Database, formed by 3 tables (Price, Reviews and Room Type) with the data of around 25000 distinct listings from January 2019 to July 2019.

Listings are categorized according to the Borough they belong to (Brooklyn, Manhattan, Queens, Bronx, Staten Island) in the city of New York. 
Initially, it was find that the Boroughs of Brooklyn and Manhattan possess around 80% of the total places listed. As well as, Private rooms and entire homes are the predominant type of listings avaliable. 
Aditionally, it was ideintified that the price/night distribution is right-skewed, meaning that there are listings overpassing the 1000 USD a night. However, the most frequent price falls between 50 to 200 USD/night, which also cover the 70% of the data available.

![Histogram-Price](https://raw.githubusercontent.com/luis12pez/Tableau-viz/A---Short-Rental-NYC/Histo-price.png)



### [Go Back](https://github.com/luis12pez/Tableau-viz)
