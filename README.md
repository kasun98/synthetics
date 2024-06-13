# Predicting Synthetic Trading Pair Prices

This project aims to predict whether the current price of Deriv broker's synthetic trading pairs (Boom 500, Boom 1000, Crash 500, Crash 1000) is good for a trade (1 or 0) using various machine learning models. The models were trained and tested on data extracted from MetaTrader 5.

## Project Overview

In this project, I explored the impact of different data preprocessing techniques on the performance of XGBoost and k-Nearest Neighbors (KNN) classifiers. The preprocessing techniques included using raw price data, log-transformed data, sine-transformed data, and standard-scaled data.

### Data Preparation

- **Data Source**: Price data for 10 synthetic charts from MetaTrader 5.
- **Features**: 60 features representing various price attributes.
- **Targets**: Binary classification targets for Boom 500, Boom 1000, Crash 500, and Crash 1000 trading indices.

### Preprocessing Techniques

1. **Raw Data**: Original price data without any scaling.
2. **Log Transformation**: Natural logarithm of the price data.
3. **Sine Transformation**: Sine of the price data.
4. **Standard Scaling**: Standard scaling of the price data.

### Models Used

- **XGBoost**: Extreme Gradient Boosting classifier.
- **k-Nearest Neighbors (KNN)**: k-NN classifier.

## Experiments and Results

For each preprocessing technique, both XGBoost and KNN models were trained and evaluated. The performance was measured using accuracy and ROC-AUC scores.


### Key Insights

- **Log Transformation**: Significantly improved the performance of the KNN model.
- **Standard Scaling**: Provided a balanced performance for both models.
- **Raw Data**: XGBoost and KNN models performed reasonably well with raw data.
- **Sine Transformation**: Resulted in lower performance compared to other transformations.

## Conclusion

This project demonstrates the importance of data preprocessing in binary classification tasks for financial market insights. By experimenting with various approaches, identified that log transformation and standard scaling can enhance the accuracy of predictions.

