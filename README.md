# Phase-2-Project
## **Business Problem**
A number of factors influence the pricing of houses. Therefore, a real estate agency would love to provide advisory services to homeowners who would love to sell their houses and to those clients who would want to purchase new houses on the prices of houses.
The agency needs to understand what factors have an effect on the house prices and to what extent. This is to enable homeowners who want to sell their homes to get the best price out of their sale. The clients who would love to buy homes wwill benefit from this advice as they'll be able to properly budget depending on their preferences. 
To be able to determine the factors that affect the prices of houses, the ```kc_house_data.csv``` will be used to carry out an analysis in order to provide the optimal advice.

## **Objective**
To find out the factors that influence house prices.

## **Data Understanding**
The dataset to be used is found in ```kc_house_data.csv```. The data is from house prices in King County.

Below is the data description:
* **id** - unique identified for a house
* **dateDate** - house was sold
* **pricePrice** -  is prediction target
* **bedroomsNumber** -  of Bedrooms/House
* **bathroomsNumber** -  of bathrooms/bedrooms
* **sqft_livingsquare** -  footage of the home
* **sqft_lotsquare** -  footage of the lot
* **floorsTotal** -  floors (levels) in house
* **waterfront** - House which has a view to a waterfront
* **view** - Has been viewed
* **condition** - How good the condition is ( Overall )
* **grade** - overall grade given to the housing unit, based on King County grading system
* **sqft_above** - square footage of house apart from basement
* **sqft_basement** - square footage of the basement
* **yr_built** - Built Year
* **yr_renovated** - Year when house was renovated
* **zipcode** - zip
* **lat** - Latitude coordinate
* **long** - Longitude coordinate
* **sqft_living15** - The square footage of interior housing living space for the nearest 15 neighbors
* **sqft_lot15** - The square footage of the land lots of the nearest 15 neighbors

## **Method**
Jupyter notebook was used in the analysis of the data. Having cleaned and scrubbed the data, Ordinary Least Squares was used in the modelling. The following were the variables that made it to  the modelling stage. They are shown in the correlation heatmap below.
![image](https://user-images.githubusercontent.com/104361809/176821150-4e78daa5-f74b-4df3-bae4-a3c153e26143.png)

## **Results**
From the moddelling, the final model selected included the followin features: ```sqft_living```, ```floors```, ```bedrooms```, ```Cond_5```, ```Cond_2``` and ```Cond_1```. The p-value of the the model was below 0.05 meaning that the features were statistically significant. The r-squared of this model was 48.2%.

## **Recommendations**
The following are the recommendations made after the analysis:
* For house sellers to reap the most out of their sales, they should increase the number of floors in the houses. They should also considerincreasing the footage of the home as such houses sell at better prices.
* House sellers should also make sure the houses they sell are in the best condition which is condition 5. This way they make the more profits.
* House buyers should plan their budget according to the specifications they would love. They should put into consideration that houses that have a larger footage, more floors and in the best condition are more expensive and may require them to save more or acquire financing to purchase. However there are  cheaper houses but they are not in the best condition. Therefore to get the best houses, house buyers should consider saving more or getting mortgages from financial institutions.
