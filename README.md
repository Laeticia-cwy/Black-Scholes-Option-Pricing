# Black-Scholes Option Pricing Project

## Overview
This project demonstrates the **Black-Scholes model** for pricing **European call and put options**, combining theoretical implementation with applied analysis. It includes:  
- A **general implementation** of the Black-Scholes model for any stock or option parameters.  
- An **applied example using Apple Inc. (AAPL) stock**, incorporating real market data to price options and visualize sensitivities (Greeks).

The project showcases **quantitative finance expertise**, Python programming skills, and the ability to apply theoretical models to real-world data.

## Formulas Used

**Call Option Price:**  

```math
C = S N(d_1) - K e^{-rT} N(d_2)
Put Option Price:
P = K e^{-rT} N(-d_2) - S N(-d_1)
Delta(Put):
\Delta_{\text{call}} = N(d_1)
\Delta_{\text{put}} = N(d_1) - 1
Where
d_1 = \frac{\ln(S/K) + (r + 0.5\sigma^2)T}{\sigma \sqrt{T}}, \quad
d_2 = d_1 - \sigma \sqrt{T}

## Features
- Compute **European call and put option prices**  
- Calculate **Delta Greeks** to measure sensitivity of option prices to stock price changes  
- Generate **visualizations**:  
  - Option prices vs. stock price  
  - Delta vs. stock price  
- Integrate **real market data** for applied analysis (Apple Inc.)  
