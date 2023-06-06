# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
1. Pull data from 3 API’s

2. Transform data
 
3. EDA
 
4. Visualization
 
5. Statistical Modelling



## Process
### Step 1: CityBikes API
•	Grabbed live data from CityBikes API
•	Generated a list of ebike stations in Miami Beach, Florida, USA using CityBikes network id “decobike-miami-beach”
•	Parsed results into a dataframe and maintained the following columns – City, CityLatLon, Bike Company, Bike Stations, BikeStationsLatLon, freebikes, empty slots

### Step 2: FourSquare API 
•	Saved my id ,secret and api_key in a notepad and read it into the notebook 
•	Pulled the POI in the CITY using the LATLON from the city bikes API using a radius of 1000m (which may not be necessary in this case) and limited the records to 50.
•	I also was not specific with the POI and got info for bars, pharmacy, parks, café , sports centre, et.c

### Step 3: YELP API
•	For Yelp, I used 3 sample size of bike stations and I pulled the POI reading the pickle file from the city bikes API notebook using a radius of 1000m and limited the records to 20 for each stations making 60 records.
•	Again, I also was not specific with the POI and got info for bars, pharmacy, parks, café , sports centre, et.c so I split the categories attributes into 3 different categories 
•	Saved the file for each stations in a pickle for reference in the joining data notebook. That was where I did my cleaning as well.


## Results

![Combined Daraframe info](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/assets/128204536/4e0c56de-f50c-40e4-9dec-3fb13fef23c5)

![Review count versus rating relationship](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/blob/main/images/Review%20count%20versus%20rating%20relationship.jpg?raw=true)

![Florida avenue POI Counts](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/assets/128204536/59142a9e-3bb3-438e-9ddd-22e100f2fccc)

![Aviation avenue POI Counts](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/assets/128204536/004e47f6-1e25-408c-98f1-2328cdf7f87b)

![City Hall](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/assets/128204536/08b7238f-78f8-4b27-8c3c-b27da25c33bc)

## Model Building

The R-squared and Adjusted R-squared values measure the goodness of fit of the regression model. 

A value of 1.000 suggests that the model explains all the variation in the dependent variable, which may indicate overfitting??? Few observations??

A p-value more than the chosen significance level - 0.05 suggests that the predictor variables – review count, rating,coordinates latlon has no  significant effect on the dependent variable.

![OLS Regression](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/blob/main/images/Model%20Building%20-%20OLS%20Regression.png?raw=true)

## Backward Selection
![OLS Regression-Backward Selection ](https://github.com/Sarah-Data/LHL-Statistical-Modelling-with-Python/assets/128204536/b98cba91-5d32-48c8-847a-1ed0f3906cab)


## Challenges 
1. Poor API documentation

2. Issues with creating environmental variables

3. Iterating over different dataframe structures in the json file

## Future Goals
1. Increase observations
 
2. De-categorize the POI for better granular insights

3. Classification Model


