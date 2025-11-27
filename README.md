# Heatwave Impact and Forcasting

## Overview
This project explores heatwave trends in four cities, Madrid, New York, Copenhagen, and Islamabad, and analyzes their effects on public sentiment. The study combines historical temperature data, predictive modeling, and social media analysis to provide insights into extreme weather events and public perception.

The project uses ARIMA and XGBoost models to forecast maximum temperatures and performs sentiment analysis on Twitter and news articles to examine how heatwaves influence public opinion.

---

## Features

- **Temperature Analysis:**  
  - Exploratory analysis of maximum, minimum, and mean temperatures from 2000 to 2023,  
  - Visualization of seasonal trends and temperature patterns for each city,  
  - Correlation analysis between temperature variables and precipitation,  

- **Heatwave Identification:**  
  - Defines heatwaves based on local temperature thresholds,  
  - Identification of extreme heat events across the four cities,  

- **Forecasting Models:**  
  - ARIMA modeling for maximum temperature prediction,  
  - Inclusion of correlated variables, such as minimum temperature, to improve predictive accuracy,  
  - XGBoost modeling to capture non-linear relationships and enhance forecast precision,  

- **Sentiment Analysis:**  
  - Analysis of approximately 15 million tweets related to climate change and heatwaves,  
  - Sentiment scoring using TextBlob and Vader,  
  - Comparison of sentiment across cities, genders, and belief stances, believers versus deniers,  
  - Analysis of news articles, such as New York Times, for sentiment trends,  

- **Heatwave Impact on Sentiment:**  
  - Daily sentiment analysis during the longest heatwaves for each city,  
  - Visualization of sentiment dips during heatwave periods,  

---

## Data Sources

- **Weather Data:**  
  - Open-Meteo API for daily temperature, precipitation, and wind speed,  

- **Twitter Data:**  
  - Tweets mentioning climate change and heatwaves, including metadata, timestamp, location, gender, stance, sentiment score,  

- **News Data:**  
  - Article titles from The New York Times API for sentiment analysis,  

---

## Dependencies

- Pandas,  
- NumPy,  
- Matplotlib, Seaborn,  
- Scikit-learn,  
- XGBoost,  
- Statsmodels,  
- TextBlob,  
- VaderSentiment,  

---

# Results and Conclusions

## Prediction Model Results
- Maximum and minimum temperatures fluctuate with no consistent long-term increase, winter minimums rise in Copenhagen and Islamabad,  
- Strong correlation exists between maximum and minimum temperatures, weak correlation with precipitation,  
- XGBoost outperforms ARIMA in predicting maximum temperatures, including minimum temperature improves ARIMA performance,  

## Sentiment Analysis Results
- **New York:** Neutral sentiment on climate change, negative on extreme weather, deniers more negative than believers,  
- **Copenhagen:** Generally neutral to slightly positive, females more positive, deniers more negative,  
- **Madrid:** Consistent neutral trends, deniers more negative,  
- **Islamabad:** Less negative overall, no gender differences, deniers more negative,  

## Heatwave Impact
- Heatwaves in New York caused dips in sentiment, Copenhagen's rare heatwave slightly increased positivity,  
- Limited daily data prevented analysis for Islamabad and Madrid,  

## Key Takeaways
- Extreme heat affects public sentiment differently by city, gender, and belief,  
- XGBoost captures non-linear trends better than ARIMA,  
- Insights can help policymakers prepare for heatwaves and public reaction,  

---

# Sources

1. Effrosynidis, D., Sylaïos, G., Arampatzis, A. (2022), Exploring climate change on Twitter using seven aspects, Stance, sentiment, aggressiveness, temperature, gender, topics, and disasters, *PloS One, 17*(9), e0274213, https://doi.org/10.1371/journal.pone.0274213  

2. Effrosynidis, D., Karasakalidis, A. I., Sylaïos, G., Arampatzis, A. (2022), The climate change Twitter dataset, *Expert Systems With Applications, 204*, 117541, https://doi.org/10.1016/j.eswa.2022.117541  

- [Kaggle Climate Change Twitter Dataset](https://www.kaggle.com/datasets/deffro/the-climate-change-twitter-dataset?resource=download)  
- [Prometeo Sevilla – Heatwaves](https://prometeosevilla.com/en/heat-waves/)  
- [Weather.gov – Excessive Heat](https://www.weather.gov/okx/excessiveheat)  
- [Denmark Climate Adaptation – Changes in Temperature](https://en.klimatilpasning.dk/knowledge/climate/denmarksfutureclimate/changes-in-temperature/)  
- [New York Times API](https://developer.nytimes.com/docs/articlesearch-product/1/overview)  
- [Open-Meteo API](https://open-meteo.com/)
