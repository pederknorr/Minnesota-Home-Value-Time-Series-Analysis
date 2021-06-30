
# Minnesota Home Value Time Series Analysis

**Authors**: Peder Norr

### Overview:

Real estate continues to be one of the most lucrative and secure investment vehicles available. This proposal contains an analysis of Minnesota home value time series data in order to provide a real estate investment firm the identification of the best locations to invest in Minnesota. Initial analysis of the data shows that there are 5 zip codes that provide the biggest opportunity for return on investment. The real estate investment firm can use this analysis to make their entry in the Minnesotan market more effective and profitable.

### Business problem:

Due to the booming housing market in the state, a real estate investment firm has decided to invest in property in Minnesota. However, they are unfamiliar with the state. They want to identify the top 5 best zip codes in the state in which to invest. This proposal will identify the top 5 zip codes for investment by calculating future potential return on investment.


### Data:

The data used in this analysis come from [Zillow Research](https://www.zillow.com/research/data/) which aggregates housing data. The data set contains 6 variables describing property sale including zip code, city, state, metro area, size rank It includes 14,723 individual entries recorded daily from 1996-2018.


## Methods

In this analysis, I create and iterate through several SARIMA models for each zip code time series to create forecasts of future home values. With those forecasted values, I calculated potential future ROI of investing in each zip code. I improved my model's iterations by adjusting parameters and differencing the data. This was done in an attempt to increase the accuracy of the model's forecasts.


## Results



## Recommendations:

Based on the forecasted ROI percentages calculated from the SARIMA model forecasts, I would provide the following recommendations to the real estate investment firm as they look to invest in Minnesota:

- **Zip Code 55415** Zip code 55415 had a forecasted ROI of 45.8% after three years, with a lower confidence interval of 12.8% and an upper confidence interval of 78.7%. The firm should invest in this zip code.

- **Zip Code 56314** Zip code 56314 had a forecasted ROI of 29.5% after three years, with a lower confidence interval of -1.7% and an upper confidence interval of 52.7%. The firm should invest in this zip code.

- **Zip Code 56570** Zip code 56570 had a forecasted ROI of 23.4% after three years, with a lower confidence interval of -24.8% and an upper confidence interval of 71.6%. The firm should invest in this zip code.

- **Zip Code 56578** Zip code 56578 had a forecasted ROI of 21.7% after three years, with a lower confidence interval of -9.3% and an upper confidence interval of 52.7%. The firm should invest in this zip code.

- **Zip Code 55449** Zip code 55449 had a forecasted ROI of 21.4% after three years, with a lower confidence interval of -8.6% and an upper confidence interval of 51.3%. The firm should invest in this zip code.


## Limitations & Next Steps

However, the SARIMA models and analysis are not complete solutions, nor are they perfect. The time series struggle to perfectly meet the assumption of stationarity, and as such the models will not be completely accurate.

I could improve this analysis in the future by further transforming the data to achieve stationarity, further tweaking the hyperparameters of the models, or by experimenting with other models like recurrent neural networks, Prophet, and Greykite.


### For further information
Please review the narrative of our analysis in [my jupyter notebook](./minnesota_home_value_time_series_analysis.ipynb) or review our [presentation](./minnesota_home_value_time_series_analysis_deck.pdf)

For any additional questions, please contact Peder Norr at <norr.peder@gmail.com>


##### Repository Structure:

```

├── README.md                         <- The top-level README for reviewers of this project.
├── minnesota_home_value_time_series_analysis.ipynb   <- narrative documentation of analysis in jupyter notebook
├── minnesota_home_value_time_series_analysis_deck.pdf   <- pdf version of project presentation
└── images
    └── images                        <- both sourced externally and generated from code
└── data
    └── 

```
