# nifty50-multiple-linear-regression
A Machine Learning Model which is a trained regression model, and produces a mathematical equation with learned weights and bias, predicted NIFTY returns, a comparison of actual vs predicted returns and a R score.

# NIFTY 50 Returns: A Linear Regression Experiment

## Overview

Can market volatility and changes in government bond yields help explain movements in the NIFTY 50?

This project explores that question using **Linear Regression**, a supervised machine learning algorithm.

I investigated the relationship between two financial indicators:
- **India VIX:** An indicator of expected market volatility and investor uncertainty.
- **Government Bond Yield Changes:** Changes in Indian government bond yields, representing movements in interest rates.

The objective was to investigate whether these indicators could explain variations in monthly NIFTY 50 returns.

## Objectives

- Explore the relationship between market volatility, bond yields, and equity market returns.
- Process and prepare financial time-series data for machine learning.
- Implement a linear regression model using Python and Scikit-learn.
- Evaluate model performance using the R² score.
- Understand the limitations of using a small number of macroeconomic indicators to explain stock market movements.

## Methodology

The project followed these steps:

1. **Data Collection:** Collected historical data for India VIX, Indian government bond yields, and NIFTY 50.
2. **Data Preparation:** Processed the datasets, calculated monthly returns and bond yield changes, and aligned observations.
3. **Feature Selection:** Used India VIX and government bond yield changes as independent variables.
4. **Model Training:** Implemented a multiple linear regression model to estimate NIFTY 50 monthly returns.
5. **Evaluation:** Compared actual and predicted returns and evaluated the model using R².

## Results

The model achieved an **R² score of approximately 0.09**.

This means that the fitted model explained approximately 9% of the variation in historical NIFTY 50 monthly returns within the evaluated dataset.

The model also identified negative relationships between NIFTY 50 returns and both selected indicators.

However, the relatively low R² suggests that these two variables alone capture only a limited portion of the variation in equity market returns.

### Key Takeaways

- Successfully implemented a multiple linear regression model on financial time-series data.
- Explored relationships between market volatility, bond yield changes, and equity returns.
- Observed the limitations of a simple linear model when applied to financial markets.
- Learned the importance of feature selection, data preparation, and model evaluation.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## Limitations

- The model uses only two independent variables.
- Linear regression assumes a linear relationship between the selected features and returns.
- An R² score of 0.09 indicates limited explanatory power.
- The result does not establish causation or demonstrate predictive accuracy on unseen data.
- Financial markets are influenced by numerous economic, geopolitical, and company-specific factors that are not included in this experiment.

## Conclusion

This project was an introduction to applying supervised machine learning to financial market data.

Although the model explained only a small portion of historical NIFTY 50 return variation, the experiment provided practical experience with financial data processing, feature selection, regression modelling, and model evaluation.

**The main learning:** Building a machine learning model is not just about obtaining predictions. Understanding what a model can and cannot explain is equally important.
