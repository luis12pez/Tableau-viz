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

### General Overview

Relational Database, formed by 3 tables (Price, Reviews and Room Type) with the data of around 25000 distinct listings from January 2019 to July 2019.

Listings are categorized according to the Borough (Brooklyn, Manhattan, Queens, Bronx, Staten Island) and Neighbourhood they belong to in the city of New York. 

Initially, it was find that the Boroughs of Brooklyn and Manhattan possess around 80% of the total places listed. As well as, Private rooms and entire homes are the predominant type of listings avaliable, they represent the 97% of them. 

Aditionally, it was ideintified that the price/night distribution is right-skewed, meaning that there are listings overpassing the 1000 USD a night. However, the most frequent price falls between 50 to 200 USD/night, which also cover the 70% of the data available.

<div style="display:flex; flex-direction: row;">
    <img src="https://raw.githubusercontent.com/luis12pez/Tableau-viz/A---Short-Rental-NYC/Histo-price.png" alt="Histogram-Price" style="width:40%;">
    <img src="https://raw.githubusercontent.com/luis12pez/Tableau-viz/A---Short-Rental-NYC/cumm-distri-price.png" alt="Cumulative-Distribution" style="width:50%;">
</div>

In term of average prices, the Borough of Manhattan double most of the other boroughs, being coherent with that the borough is the center of tourisim of the city. Where, as it will be expected the entire home type of room is the most expensive

| borough        | Average price (USD/month) |
|----------------|---------------|
| Manhattan      | 5600   |
| Brooklyn       | 3700   |
| Queens         | 2800   |
| Staten Island  | 2600   |
| Bronx          | 2400   |

| room_type       | Average Price |
|-----------------|---------------|
| entire home/apt | 5997.226536   |
| private room    | 2484.254654   |
| shared room     | 1631.789174   |

<div style="display:flex;">
    <div style="flex:1;margin-right:10px;">
        <table>
            <thead>
                <tr>
                    <th>borough</th>
                    <th>Average price (USD/month)</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Manhattan</td>
                    <td>5600</td>
                </tr>
                <tr>
                    <td>Brooklyn</td>
                    <td>3700</td>
                </tr>
                <tr>
                    <td>Queens</td>
                    <td>2800</td>
                </tr>
                <tr>
                    <td>Staten Island</td>
                    <td>2600</td>
                </tr>
                <tr>
                    <td>Bronx</td>
                    <td>2400</td>
                </tr>
            </tbody>
        </table>
    </div>

    <div style="flex:1;">
        <table>
            <thead>
                <tr>
                    <th>room_type</th>
                    <th>Average Price</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>entire home/apt</td>
                    <td>5997.226536</td>
                </tr>
                <tr>
                    <td>private room</td>
                    <td>2484.254654</td>
                </tr>
                <tr>
                    <td>shared room</td>
                    <td>1631.789174</td>
                </tr>
            </tbody>
        </table>
    </div>
</div>


### [Go Back](https://github.com/luis12pez/Tableau-viz)
