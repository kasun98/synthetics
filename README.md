# ML Trading

![Main Image](https://res.cloudinary.com/dlb65j6di/image/upload/v1721924134/a_6_kh6yjl.png)

In this project, I analyzed the prices of Deriv broker's synthetic trading indices, specifically focusing on Boom 500, Boom 1000, Crash 500, and Crash 1000 prices. The dataset consisted of 60 features extracted from 10 synthetic charts on MetaTrader 5. I experimented with different data transformations and machine learning models to predict these target prices.

**[Github Repository](https://github.com/kasun98/synthetics)**

## Feature Engineering

I started by extracting the price data for 10 synthetic charts from MetaTrader 5, resulting in a dataframe with 60 features. These features were analyzed for their correlation with the target synthetic indices: Boom 500, Boom 1000, Crash 500, and Crash 1000 prices.

![Correlation Matrix](https://res.cloudinary.com/dlb65j6di/image/upload/v1722008086/correlation_matrix_sbf0is.png)

![Synths1 B500](https://res.cloudinary.com/dlb65j6di/image/upload/v1722008118/synths1_b500_w4zd2n.png)

## Machine Learning Experiments

To evaluate the performance of different models and data transformations, I conducted the following experiments:

- **Raw Data**: Used the original price data without any scaling.
- **Log Transformation**: Applied natural logarithm to the price data.
- **Sine Transformation**: Converted the price data to sine values.
- **Standard Scaling**: Applied standard scaling to the price data.

For each experiment, I used **XGBoost** and **k-Nearest Neighbors (KNN)** models to predict the 'Is current market price good for a trade' (Binary classification). The performance was measured using accuracy and ROC-AUC scores.

## Observations

- **Boom500 index analysis**: Both XGBoost and KNN algorithms performed well with log price data.
- **Boom1000 index analysis**: XGBoost and KNN algorithms performed well with Standard scaled data and log price data respectively.
- **Crash500 index analysis**: XGBoost and KNN algorithms performed well with Raw data and log price data respectively.
- **Crash1000 index analysis**: XGBoost and KNN algorithms performed well with Standard scaled data and log price data respectively.

### Performance Charts

![Boom 500 Analysis](https://res.cloudinary.com/dlb65j6di/image/upload/v1722008139/b500_gfkjzg.png)

![Boom 1000 Analysis](https://res.cloudinary.com/dlb65j6di/image/upload/v1722008154/b1000_zuan42.png)

![Crash 500 Analysis](https://res.cloudinary.com/dlb65j6di/image/upload/v1722008169/c500_lc44bj.png)

![Crash 1000 Analysis](https://res.cloudinary.com/dlb65j6di/image/upload/v1722008178/c1000_lugasy.png)

## Results and Insights

The comparison charts above summarize the performance of XGBoost and KNN models across different data transformations. Here are some key insights:

- **Raw Data**: XGBoost and KNN models performed reasonably well with raw data.
- **Log Transformation**: Applying natural logarithm improved the performance of KNN significantly.
- **Sine Transformation**: Sine transformation resulted in lower performance compared to other transformations.
- **Standard Scaling**: Standard scaling provided a balanced performance for both models.

---
*© 2025 | Kasun Dewaka. All rights reserved.*
