# Black–Scholes Option Pricing Model

## Project Overview
This project implements the Black–Scholes model to price European call and put options.  
It includes basic visualizations of option prices and Delta (sensitivity to stock price) to illustrate how option values change with underlying parameters.

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

## Features Implemented
- Pricing functions for European **Call** and **Put** options
- Simple plots: Option price vs Stock price
- Greeks: **Delta** (Call & Put)
- Markdown sections: Assumptions and Limitations

## Example Output
```text
Call price (S=100, K=100, T=1, r=0.05, σ=0.2): 10.45
Put price (S=100, K=100, T=1, r=0.05, σ=0.2): 5.57
