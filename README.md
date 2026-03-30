## Executive Summary ##

At 8.8 million barrels per day, the United States is the largest consumer of gasoline in the world and fuel prices play a key role for consumers and businesses in the U.S. This project will analyze the variables that impact fuel prices, and will propose a model to forecast gasoline prices in the United States. 

## Business case ##

Gasoline is an important part of the expenditures of certain industries like transportation. It also plays an important role in the budget of American consumers. Directly and through  transportation costs, motor fuel weighs close to 16% of the Consumer Price Index (CPI).  
A forecast for gasoline prices would help several industries in their price setting process and consumers in their budgeting. For instance, transportation companies could set more competitive rates while maintaining their margins, downstream oil and gas companies could improve their revenue forecast, and consumers would benefit from a better prediction of their expenses. 

## Main data: Retail gasoline prices ## 
• Monthly U.S. [Gasoline Prices](https://www.eia.gov/opendata/browser/petroleum/pri/gnd) \
• Granularity: monthly. Available since August 1990

## Exogenous variables ##
[Gasoline stockl evels](https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=PET&s=WGTSTUS1&f=W) \
• Granularity: weekly. Available since Jan 1, 2010 \
[US field production of crude oil](https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=PET&s=MCRFPUS1&f=M) \
• Granularity: monthly. Available since Jan 1, 2000 \
[Inflation without food and energy prices](https://fred.stlouisfed.org/series/CORESTICKM159SFRBATL) \
• Granularity: monthly or yearly. Available since 2000 \
[Crude oil imports](https://www.eia.gov/opendata/browser/petroleum/stoc/wstk) \
• Granularity: monthly. Available since August 1982 \
• Serves as a proxy of gasoline supply; use destination=US \
[Traffic volume trends](https://www.fhwa.dot.gov/policyinformation/travel_monitoring/tvt.cfm) \
• Granularity: monthly. Available from 1992 to 2025 \

## Methodology ##
Pre-modeling: \
• EDA \
• Train period: 16 years / 26 years \
• Test period: 12 months (2025) \
Modeling: \
• Three experiments \
• Types of models: SARIMA, SARIMAX,Transfer Function, TBATS, and BSTS. \
Post-Modeling: \
• Metrics: AIC, MAE, MAPE, and RMSE in train/test. \
• Verify significance of coefficients. \
• Check residuals (Correlogram, Ljung-box Test)



