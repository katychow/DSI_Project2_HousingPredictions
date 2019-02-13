# DSI-6 Project 2 - Predicting Housing Prices in Ames, Iowa

## Katy Chow

### Problem Statement
We are trying to predict housing prices in Ames, Iowa given a dataset of 81 attributes.

### Executive Summary
Using linear regression methods along with a small subset of the data, we are able to explain more than 85% of the variance of housing prices with our model.  

### Data Sources & Dictionary
For the Ames dataset, I removed outliers recommended by the Data Document Linked below.  I also removed several data points where the lot area was unrealistically large give the cost of the home.  There were 


|Final Attribute | Data Type | Short Description |
|---|---|---|
|Gr Liv Area|INT64| Ground Living area in SF |
|Year Built|INT64| Year home was built |
|Overall Cond Bi|INT64| 1 if Overall Cond >= 5, else 0 |
|Year Remod/Add|INT64| Year home remodeled |
|Tot_bath_bsmt|INT64| Total number of bathrooms in the basement |
|Lot Area|INT64| Lot size |
|Sale Type Bi|INT64| 1 if 'New', 2 if 'Oth' or 'CWD', else 0 |
|Outdoor Liv Area|INT64| Wood Deck SF + Open Porch SF + Screen Porch|
|Bldg Type Bi|INT64| 1 if '1fam' or 'TwnhmE', else 0|
|TotRms AbvGrd|INT64| Total number of rooms above ground |
|Mo Sold|INT64| Month Sold |
|Yr Sold|INT64| Year Sold|
|Tot_bath_abv_grd|INT64| Total number bathrooms above ground |
|Kitchen AbvGr|INT64| Number of Kitchens above ground |
|Bedroom AbvGr|INT64| Total number of bedrooms above ground |


Please see the following websites for 
* [http://jse.amstat.org/v19n3/decock/DataDocumentation.txt] Data Dictionary of Original Data
* [https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge] Data Source
        
### Conclusions & Next Steps
Using lasso regression along with a few data transformations, removal of extreme outliers, and creating dummy variables allowed for us to fit a model that is performing with an r2 value of ~85%.  The next step, if we were trying to predict exactly the scores, we may want to try more advanced models or use classifying methods to variable select.  
