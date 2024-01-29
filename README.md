## Fuel Trend Analysis: Advanced Machine Learning for Predictive Fuel Pricing in Kenya
![fuel-price](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/e6f6c958-ddeb-4387-a768-946286925400)

**Group 6**
Student Names
* Eva Kiio
* George Odhiambo
* Bedan Njoroge
* Abdi S Mohammed
* Sophie Owour
* Laban Kariuki

## Business Problem 
This project, "Fuel Trend Analysis: Advanced Machine Learning for Predictive Fuel Pricing in Kenya," focuses on creating a sophisticated predictive model using machine learning techniques to accurately forecast fuel prices. By analyzing historical fuel price data from the Energy and Petroleum Regulatory Authority (EPRA), the project aims to address the challenges posed by the volatility of fuel prices on economic planning and policy, affecting consumers, businesses, and government agencies.

## Project Objective
The aim of this project is to utilize advanced time series analysis methods, such as ARIMA, SARIMA, Facebook Prophet, and LSTM models, to analyze fuel price data for super, diesel, and kerosene provided by the EPRA. The specific objectives of this project are:
1. Analyze fuel price trend 
2. Optimization of demand

### Significance
This project focuses on creating a model to forecast fuel prices, aiding consumers in budgeting, businesses in strategy, and government agencies in policy-making. Emphasizing data-driven decision-making, it aims to stabilize the economy against fuel price volatility and sets a new standard in Kenya's fuel market analytics, bolstering economic planning and resilience.



## Data Understanding 

The Dataset consists of fuel prices sourced from Energy and Petroleum Regulatory Authority(EPRA) https://www.epra.go.ke/services/petroleum/petroleum-prices/ and US Dollar Exchange Rate source Central Bank of Kenya https://www.centralbank.go.ke/rates/forex-exchange-rates/. 

The dataset consists of the following columns;

### EPRA Dataset

__Date__: This column records the date of the data entry.

__Towns__: This column lists various towns.

__Super__: This column refers to the price of 'Super' grade fuel.

__Diesel__: This column refers to the price of 'Diesel' grade fuel.

__Kerosene__: This column refers to the price of 'Kerosene' grade fuel.

### CBK Exchange Rate Data

__Date__: This column records the date of each exchange rate entry.

__Currency__: This column specifies the foreign currency for which the exchange rate is given.

__Mean__: This column shows the average exchange rate for the specified currency on the given date. 

__Buy__: This column indicates the buying rate of the currency.

__Sell__:This column shows the selling rate of the currency.

## Project Structure
1. Exploratory Data Analysis (EDA)
2. Data Preprocessing - Resampling, Testing for Trends, Diffencing, Decomposition, Train-Test Split, Checking for best ARIMA & SARIMA Orders
3. Modelling - ARIMA, SARIMA, Facebook Prophet & LSTM (Long Short - Term Memory)
4. Model Evaluation - using MAE and RSME
5. Deployment

## Results

### Super Price Forecast
### Forecast Prediction forecast
![image](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/aaa812d6-6711-4696-9deb-fc02b5b4cb9d)

The Facebook Prophet model performed the best in predicting super fuel values, with the lowest Mean Absolute Error (MAE) (3.30) and Root Mean Square Error (RMSE) (4.18) among the models evaluated. Following closely in performance, the SARIMA model exhibited the second-best results MAE (3.29) and RMSE (4.98), ARIMA was third with MAE (3.34) and RMSE (5.25) while the LSTM model showed the least accuracy among the models tested with MAE (4.02) and RMSE (6.09).

### 5 Year Forecast Using Facebook Prophet
![image](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/515d83ca-838d-43ab-af30-2bd9895a0ee1)


### Diesel Price Forecast
### Forecast Prediction forecast
![image](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/2fc953e9-26c9-47dd-9223-a9a1603aef5c)

The Facebook Prophet model outperformed the other models in terms of both MAE (3.55)  and RMSE (5.07), making it the best-performing model for predicting diesel fuel values. Following closely in performance, the ARIMA model displayed the second-best results MAE (3.59) and RMSE (5.99), SARIMA was third with MAE (3.98) and RMSE (6.37) while the LSTM model exhibited the least accuracy among the models evaluated with MAE (4.26) and RMSE (7.30).

### 5 Year Forecast Using Facebook Prophet
![image](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/40d3ebf1-ac12-410a-b2b8-3c90919bb3f9)

### Kerosene Price Forecast
### Forecast Prediction forecast
![image](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/996723b6-3f9f-4666-84ea-3bec9cd51285)

The Facebook Prophet model performed the best in predicting kerosene fuel values, with the lowest MAE (4.26) and RMSE (8.61) among the models evaluated. Following in performance, the ARIMA model displayed the second-best results with MAE (4.04) and RMSE (6.92), SARIMA was third with MAE (6.10), RMSE (8.61) while the LSTM model showed the least accuracy among the models tested for kerosene prediction with MAE (4.98) and RMSE (9.01).

### 5 Year Forecast Using Facebook Prophet
![image](https://github.com/Kichimbi/DSFP4P5-G6-Capstone-Project/assets/118848352/96abdd61-b74a-45b1-ac14-7fa92f295451)

## Model Deployment 
The deployed model can accessed and tested here

## Summary 
The forecasting models (ARIMA, SARIMA, Facebook Prophet, and LSTM) exhibit different performances, highlighting the importance of choosing the right model for each product category.

While the project yields valuable insights into fuel price trends and model performances, challenges in achieving precise forecasts persist due to government policies, fluctuations in USD exchange rates, and other external factors.

Efficient utilization of time series models can aid in predicting fuel price fluctuations, but ongoing adjustments to external factors are crucial to address the inherent unpredictability in fuel price changes.

### Recommendations





### Limitations

Predicting fuel prices using models has several limitations:

- **External Factors**: Fuel prices are heavily influenced by external factors such as geopolitical events, economic conditions, and government policies. Models may struggle to capture these complex and dynamic influences accurately.
  
- **Non-Stationarity**: Fuel price data often exhibits non-stationary behavior, with changing statistical properties over time.
  
- **Short-Term Focus**: Many models perform better in the short term but may struggle with long-term predictions due to the complexity of underlying factors.
  
- **Uncertainty**: Predictions are inherently uncertain, and models often provide a range of possible outcomes rather than precise values.
  
- **Regulatory Changes**: Government regulations and policies, like taxation or subsidies, can have abrupt and profound effects on fuel prices that models may struggle to predict accurately.


Capstone Checklist: https://github.com/learn-co-curriculum/dsc-capstone-submission-checklist.git
