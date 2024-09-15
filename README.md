# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The project uses data from CityBikes, Foursquare, and Yelp to study bike-sharing services and local businesses in a specific area. The goal is to create a model that shows how bike availability affects business ratings.

Goals:
1. Retrieve and Consolidate Data:
> API Integration: Use HTTP requests to get data from CityBikes, Foursquare, and Yelp APIs. Handle authentication, make GET requests, and process JSON responses.

> Data Wrangling: Clean and organize the raw data into DataFrames using pandas. This includes handling missing values, converting data types, and merging datasets based on common fields like location coordinates.

2. Analyze Combined Data:
> Data Merging: Combine DataFrames from different APIs into one dataset by aligning data based on locations and business identifiers.

> Exploratory Data Analysis (EDA): Perform EDA to understand the data's distribution and relationships. Visualize bike station locations and business ratings, and identify patterns or anomalies.

3. Develop Regression Model:
> Model Creation: Create relevant features for the regression analysis, such as bike station density, average business rating, and distance metrics.

> Regression Analysis: Use regression techniques to model the relationship between bike availability and business ratings, including linear regression.

> Model Evaluation: Assess the model’s performance using metrics like R-squared, Mean Squared Error (MSE), and cross-validation to ensure accuracy and robustness.

### Techniques Used:
1. API Integration:
   > HTTP Requests: Use the requests library in Python to make API calls and handle responses.
   > JSON Parsing: Extract relevant data from JSON responses.
2. Data Wrangling:
   > Pandas DataFrames: Use pandas for data cleaning, transformation, and merging.
   > Data Cleaning: Handle missing data, outliers, and inconsistencies to ensure high-quality input for analysis.
3. Data Analysis:
   > Exploratory Data Analysis (EDA): Use visualizations (scatter plots, histograms) to understand data distributions and relationships.
   > Geospatial Analysis: Map bike stations and businesses to visualize spatial relationships and assess coverage.
4. Regression Modeling:
   > Feature Engineering: Create meaningful features from raw data to improve model performance.
   > Regression Techniques: Implement linear regression to model the impact of bike availability on business ratings.
   > Model Evaluation: Use metrics like R-squared and MSE to gauge model accuracy and interpret results.
## Process
Step 1: Connection to CityBikes API
> Established a connection to the CityBikes API.

> Retrieved data on bike station availability and locations.
 
> Created a DataFrame to organize and analyze the bike-sharing data.
 
Step 2: Connection to Foursquare and Yelp APIs

> Established connections to Foursquare and Yelp APIs.'

> Retrieved data on local businesses, including ratings, reviews, and locations.

> Created separate DataFrames for Foursquare and Yelp data.

Step 3: Data Integration

> Merged the CityBikes DataFrame with the Foursquare and Yelp DataFrames.

> Ensured data consistency and handled any discrepancies.

> Loaded the combined data into a database for further analysis.

Step 4: Regression Model and Analysis

> Developed a regression model to analyze the relationship between bike availability and local business ratings.

> Evaluated the model's performance and interpreted the results as below,
* Model Overview:
  
  Dependent Variable: Number of Bike Stations
  
  Independent Variable: Number of Restaurants and Bars
  
  Method: Least Squares
  
  No. Observations: 256

  Degrees of Freedom (DF Residuals): 254
  
  DF Model: 1 (indicating a single independent variable)
* R-squared: -inf (negative infinity)

  This value suggests that the model does not explain any variability in the dependent variable. This could indicate a serious issue with the data or model setup, like collinearity or poor model fit.

* F-statistic: -254.0 (Prob (F-statistic) = 1.00)

  The F-statistic and its probability suggest the model does not have any explanatory power.
* Coefficients:

  Intercept (const): 1.0000 with a P-value of 0.000 (indicating significance).
Number of Restaurants and Bars: The coefficient is 5.1e-16, and the associated P-value is 0.18 (suggesting it is not statistically significant).


## Results
### Specifically related to the project: 
> In vancouver city there are lots of bike station compared to restaurants and bars. 

> The regression model depicts that there's no relationship between places of bike staion and restaurants.

### Technical Skills
   
> API Integration and Data Retrieval: HTTP Requests, JSON Parsing

> Data Wrangling and Cleaning: Pandas DataFrames, Data Cleaning

> Data Analysis and Visualization:Exploratory Data Analysis (EDA)

> Regression Modeling:Model Creation, Regression Techniques, Model Evaluation

### Soft Skills

> Problem-Solving

> Attention to Detail

> Time Management

> Communication

> Collaboration:


## Challenges 

### Technical Challenges:

> Data Consistency: Ensuring consistency between different data sources was challenging due to varying formats and missing values.

> API Limitations: Rate limits and data access restrictions imposed by APIs required careful planning and efficient data retrieval strategies.

> Model Accuracy: Achieving a high level of accuracy in the regression model was difficult due to the complexity of factors influencing business ratings.

### Personal Challenges:

> Understanding API behavior is bit challenging. Often, API documentation is not standardized, it's difficult to find specific details. Additionally, each API behaves differently.

> Difficult to understand some questions. Providing more details would be helpful.

> Technical Barriers - Some technical concepts are unfamiliar, and new techniques are frequently introduced.

## Future Goals

> Expand Data Sources: Incorporate additional data sources to enrich the analysis, such as weather data or traffic patterns.

> Enhance Model: Improve the regression model by exploring advanced machine learning techniques and feature engineering.

> Geographic Expansion: Apply the analysis to other cities and regions to gain broader insights and validate findings.
