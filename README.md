# Equity-Portfolio-Optimization-MPT
A quantitative analysis project implementing Modern Portfolio Theory (MPT) and the Capital Asset Pricing Model (CAPM) to optimize a 6 stock equity portfolio using Python and Excel.

# FM3054: Equity Portfolio Optimization & CAPM Analysis
This repository contains the mid-term take-home assignment for FM3054: Portfolio Optimization at the University of Colombo, Department of Mathematics. The project serves as a practical implementation of Modern Portfolio Theory (MPT) and the Capital Asset Pricing Model (CAPM).

## Project Overview
Acting as a junior quantitative portfolio analyst, I have constructed and evaluated an optimal equity portfolio using a selected universe of 5-8 listed equities over a minimum 3-year sample period. The analysis integrates historical market data with computational optimization techniques to identify efficient investment allocations.

## Key Learning Outcomes
Designing and optimizing equity portfolios under realistic constraints.
Constructing and interpreting the Mean-Variance Efficient Frontier and the Capital Market Line (CML).
Evaluating performance using the Capital Asset Pricing Model (CAPM) framework.
Implementing financial models using Python (Google Colab) and Microsoft Excel.

## Project Structure
├── data/
│   └── stock_data.csv          # 3+ years of historical daily/monthly returns
├── notebooks/
│   └── Portfolio_Analysis.ipynb # Python code for optimization & CAPM regression
├── excel/
│   └── Portfolio_Solver.xlsx   # Return calculations, matrices, and Solver models
├── reports/
│   └── Final_Report.pdf        # 5-page formal academic report
└── README.md                   # Project documentation

## Technical Implementation
### 1. Data Preparation & Exploratory Analysis
Metrics: Computed annualized mean returns, volatility, and covariance/correlation matrices.Visuals: Risk-return profiles and correlation heatmaps.
### 2. Portfolio Construction
I constructed the following portfolios with and without short-selling constraints:
Minimum Volatility Portfolio: Minimizes variance for a given level of return.
Maximum Sharpe Ratio Portfolio: Maximizes the excess return per unit of risk.
Equal-Weighted Portfolio: Serves as the baseline benchmark.
### 3. Efficient Frontier Analysis
Derived the Mean-Variance Efficient Frontier using the Lagrangian Multiplier method. The optimization problem for the Minimum Volatility portfolio is defined as:$$\min \sigma_p^2 = w^T \Sigma w$$Subject to:$$\sum_{i=1}^{n} w_i = 1$$The Capital Market Line (CML) was constructed by introducing a risk-free asset consistent with the chosen market.
### 4. CAPM-Based Evaluation
Beta Estimation: Calculated systematic risk for individual stocks and optimized portfolios.
Jensen's Alpha: Measured the abnormal return of the portfolios over the CAPM predicted return.
Risk Decomposition: Partitioned total risk into Systematic (Market) and Idiosyncratic (Specific) components.

## How to Use
Python Notebook: Open notebooks/Portfolio_Analysis.ipynb in Google Colab. The code is well-commented and utilizes scipy.optimize for quadratic programming and seaborn for financial visualizations.
Excel Workbook: The excel/Portfolio_Solver.xlsx file contains the manual calculation of the covariance matrix and utilizes the Excel Solver Add-in for portfolio weighting.
Written Report: The reports/Final_Report.pdf provides the economic interpretation and critical assessment of the results.
