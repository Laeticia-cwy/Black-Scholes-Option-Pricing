# Black-Scholes Option Pricing Project

## Overview
This project demonstrates the **Black-Scholes model** for pricing **European call and put options**, combining **theoretical implementation** with **applied analysis using real stock data**.  

It contains:  
- A **general Black-Scholes model** for any stock or option parameters  
- An **applied example using Apple Inc. (AAPL) stock**, fetching real market data to price options and visualize sensitivities (Greeks)  

This project showcases **quantitative finance expertise**, Python programming skills, and the ability to **apply theoretical models to real-world data**.

## Formula Explanation
The Black–Scholes formulas used:

**Call Option Price:**  
C = S * N(d1) - K * e^(-rT) * N(d2)

**Put Option Price:**  
P = K * e^(-rT) * N(-d2) - S * N(-d1)

Where:  
- S = stock price  
- K = strike price  
- T = time to maturity  
- r = risk-free rate  
- σ = volatility  
- N() = cumulative distribution function of the standard normal distribution  

d1 = (ln(S/K) + (r + 0.5*σ²)*T) / (σ * sqrt(T))  
d2 = d1 - σ * sqrt(T)

Legend of Variables:  
- S = Current stock price  
- K = Strike price  
- T = Time to expiration (in years)  
- r = Risk-free interest rate  
- σ = Volatility of the underlying stock  
- N() = Cumulative distribution function of the standard normal  

## Features
- Compute **European call and put option prices**  
- Calculate **Delta Greeks** to measure sensitivity of option prices to stock price changes  
- Generate **visualizations**: option prices vs stock price, Delta vs stock price  
- Apply **real market data** for dynamic pricing (Apple Inc.)  

## Assumptions
- European options only (exercisable at expiration)  
- No dividends during the option’s life  
- Constant volatility and risk-free rate  

## Run the Notebook
For users who want to execute the code:  
- Clone the repository: `git clone https://github.com/Laeticia-cwy/Black-Scholes-Option-Pricing.git`  
- Install dependencies: `pip install numpy scipy matplotlib yfinance`  
- Open the Jupyter notebook and run all cells  
