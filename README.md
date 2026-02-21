# Black-Scholes Option Pricing

## Project Overview
This project implements the **Black-Scholes model** to calculate the prices of **European call and put options**. It also computes the **Delta Greeks** to measure sensitivity of option prices to stock price changes. Visualizations are included to illustrate how option prices and Delta vary with the underlying stock price.  

## Features
- Black-Scholes call and put pricing functions  
- Delta calculation for both call and put options  
- Plots of option prices vs stock price  
- Plots of Delta vs stock price  
- Optional integration with **real stock data** for applied analysis  

## Formulas Used
- **Call Option Price:**  
\[
C = S N(d_1) - K e^{-rT} N(d_2)
\]
- **Put Option Price:**  
\[
P = K e^{-rT} N(-d_2) - S N(-d_1)
\]
- **Delta (Call):** \( \Delta_{call} = N(d_1) \)  
- **Delta (Put):** \( \Delta_{put} = N(d_1) - 1 \)  
Where:  
\[
d_1 = \frac{\ln(S/K) + (r + 0.5\sigma^2)T}{\sigma \sqrt{T}}, \quad d_2 = d_1 - \sigma \sqrt{T}
\]

## How to Run
1. Clone the repository:  
```bash
git clone https://github.com/Laeticia-cwy/Black-Scholes-Option-Pricing.git
