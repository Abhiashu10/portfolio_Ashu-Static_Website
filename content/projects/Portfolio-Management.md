---
title: "Portfolio Management Using Python for Healthcare Stocks"
description: "Built a portfolio using Modern Portfolio Theory (MPT) with one-year data [2020], calculated Value at Risk (VaR) and Conditional Value at Risk (CVaR) at a 99% confidence level for each trading day and week, forward tested the portfolio with the next year's data [2021], conducted hypothesis testing on the calculation described in step 3, and compared the results to the market benchmark - S&P 500, with returns presented in percentage and annualized."
dateString: Dec 2022
draft: false
tags: ["Time Series", "ARIMA", "SARIMAX", "Hypothesis Testing", "VaR", "CVaR", "Portfolio Management", "Healthcare", "Finance"]
showToc: false
weight: 207
cover:
    image: "projects/PM/PM1.jpg"
--- 
### 🔗 [GitHub repository](https://github.com/Abhiashu10/Portfolio_Management_Python_Healthcare_Stocks.git)

## Description
As a portfolio manager, you are requested to design the fund's next flagship portfolio with $10 million in a specific industry (your pick) with at least 12 stocks.

1. Address the rationale picking those stocks 

2. Build portfolio with Modern Portfolio Theory (MPT) with one year data [2020] 

3. Calculate the Value at Risk(VaR) and Conditional Value at Risk(CVaR) at 99% confidence level for each  trading day and week

4. Forward testing with the next year data [2021]

5. After the testing phase, please run hypothesis testing regarding the calculation described in step 3  

6. Compare to market benchmark - S&P 500: return should be in percentage and annualized


## Introduction

The project is focused on utilizing Modern Portfolio Theory (MPT) to create and select an appropriate portfolio. It explores the process of identifying solid businesses with promising futures in the US stock market. The project addresses key questions of investment selection and allocation by leveraging MPT. Additionally, the research aims to evaluate the potential of an optimal portfolio to outperform an index fund, specifically the S&P 500.

## Dataset Information

The dataset used in the research consists of 253 rows and 14 columns, focusing on the closing prices of top healthcare companies. The specific companies included are Abbott Laboratories (ABT), AstraZeneca plc (AZN), GSK plc (GSK), Elevance Health Inc (ELV), Novartis AG(NVS), Merck & Co Inc (MRK), UnitedHealth Group Inc (UNH), Johnson & Johnson (JNJ), Eli Lilly and Co (LLY), Pfizer Inc (PFE), Novo Nordisk A/S (NVO), and Moderna (MRNA).

## What is Modern Portfolio Theory?

Modern Portfolio Theory, developed by Harry Markowitz, provides a framework for portfolio managers to construct portfolios based on projected returns and risk factors. The theory involves a two-step process: analyzing the future performance of available securities and selecting the portfolio that offers the highest expected return at a given risk level or the lowest risk level at a given expected return.

## Rationale for Picking Healthcare Sector and Stocks

The healthcare sector was chosen for analysis due to its lower risk factors compared to other industries. The sector experiences increased demand during times of epidemics and wars, and the rising concern for health has led to a surge in routine checkups and medication consumption. Furthermore, the healthcare industry is witnessing significant advancements in medical technologies, attracting government support and global demand.

## Build a Portfolio with Modern Portfolio Theory (2020 data)

The project involved importing data using the pandas data reader library, focusing on closing prices of top 14 healthcare companies. Statistical analysis was performed to assess risk and return, and two methodologies were applied: mean-variance optimization and hierarchical risk parity (HRP). The resulting portfolios were evaluated in terms of expected return, risk, and Sharpe ratio.

Visualizing the data: - We can see that the revelation of the vaccination has caused the price of Moderna's shares, MRNA, to skyrocket. Additionally, we can see that Danaher Corp (DHR) and United Health Group (UHG) will have healthy growth in 2020 along with Moderna (MRNA).
![my notes](/projects/PM/PM2.png)

## Risk vs Return Curve
A risk vs return curve was plotted to analyze the relationship between risk and return for the portfolios created using MPT.
![my notes](/projects/PM/PM3.png)

- Method 1: - Mean-Variance Optimization
We can build a portfolio of 2845 shares of MRNA, 678 shares of DHR and 99 shares of UNH. 

- Method 2: - Hierarchical Risk Parity (HRP)
We can build a portfolio of 107 shares of MRNA, 179 shares of DHR, 94 shares of UNH, 860 shares of MRK, 442 shares of NVS, 266 shares of LLY, 264 shares of JNJ, 179 shares of DHR, 569 shares of NVO, 1048 shares of GSK.


## Comparison with S&P 500

The project compares the performance of the portfolio to the S&P 500 index, considering the annual returns of both.

##Code
## [GitHub Code](https://github.com/Abhiashu10/Portfolio_Management_Python_Healthcare_Stocks/blob/07be44f91fe0e9a08de298627511d52d40233811/Portfolio%20Management%20Using%20python%20for%20healthcare%20stocks.ipynb)


