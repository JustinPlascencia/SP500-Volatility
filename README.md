# S&P 500 Volatility Modeling and Prediction

## Overview

This project analyzes and predicts stock return volatility across S&P 500 sectors using a combination of machine learning, time series modeling, and Bayesian methods. The goal is to evaluate how well different modeling approaches capture volatility patterns and whether predictability varies by sector.

Understanding volatility is critical in finance for risk management, portfolio optimization, and derivative pricing. This project explores both statistical and data-driven approaches to modeling these dynamics.

---

## Key Results

* Volatility predictability varies significantly across sectors.
* Financial and Utilities sectors show the highest predictability.
* Healthcare exhibits low or negative predictive performance in some models.
* Neural networks outperform traditional models in certain sectors.
* Stock returns deviate from normality, supporting the use of advanced models like GARCH and Bayesian methods.

---

## Methods

### Data Collection

* Scraped S&P 500 company tickers and sector classifications
* Retrieved historical stock price data using `yfinance`

### Feature Engineering

* Computed daily returns
* Constructed rolling volatility measures
* Created lagged features to capture temporal dependence

### Models Implemented

#### Machine Learning

* **Random Forest Regressor**

  * Captures nonlinear relationships
  * Used as a baseline ensemble model

* **Multilayer Perceptron (PyTorch)**

  * Learns complex patterns in volatility dynamics
  * Compared against traditional approaches

#### Time Series Modeling

* **ARIMA-GARCH**

  * Models both mean and conditional variance
  * Widely used in financial econometrics

#### Bayesian Approach

* **Metropolis-Hastings Algorithm**

  * Estimates posterior distributions of volatility parameters
  * Provides probabilistic interpretation of uncertainty

---

## Statistical Analysis

* Conducted normality tests on returns
* Performed hypothesis testing on model outputs
* Evaluated model performance using R² and error metrics

---

## Results

Model performance differs by sector:

* **Financials:** Most consistent and predictable volatility patterns
* **Utilities:** Strong performance from neural networks
* **Healthcare:** Weak predictability across models
* **Technology:** Mixed results depending on model choice

These findings suggest that sector-specific characteristics influence volatility dynamics and model effectiveness.

---

## Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* PyTorch
* Statsmodels
* yfinance

---

## Project Structure

```
├── data/                # Raw and processed data
├── notebooks/           # Analysis and modeling notebooks
├── src/                 # (Optional) Modularized code
├── README.md
```

---

## Future Work

* Incorporate macroeconomic indicators
* Explore LSTM and transformer-based models
* Perform hyperparameter tuning for all models
* Extend analysis to international markets

---

## Conclusion

This project demonstrates that volatility is not uniformly predictable across sectors and that model selection plays a critical role. Combining statistical, machine learning, and Bayesian approaches provides a more comprehensive understanding of financial time series behavior.

---

## Author

Justin Plascencia
