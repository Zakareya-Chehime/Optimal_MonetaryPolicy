# Optimal Interest Rate Policy: An Optimization-Driven Alternative to the Taylor Rule

## Overview
This project explores whether central banks should move beyond the traditional Taylor Rule when setting monetary policy. Using the New Keynesian IS and Phillips Curve framework, I compare the performance of the Taylor Rule against an optimization-driven approach that directly minimizes macroeconomic losses.  

The work is split into two parts:
- **Parameter Estimation (Python):** Estimates structural parameters from macroeconomic data.  
- **Policy Optimization (Julia):** Solves for the optimal interest rate path under estimated dynamics and compares it against the Taylor Rule benchmark.  

---

## Motivation
Central banks often rely on simple rules such as the Taylor Rule to set interest rates. While effective in many cases, these rules are not flexible enough to handle dynamic shocks, bubbles, or recessions.  
This project investigates whether an optimization-based framework can deliver **better outcomes for inflation stability and output stabilization** compared to a rule-based approach.

---

## Key Findings
- For the specified quadratic loss function, the **optimization-driven interest rate path consistently outperforms the Taylor Rule**.  
- The Taylor Rule tends to generate excessive volatility:
  - It starts off with **interest rates set too high**.  
  - It **overcorrects** in response to shocks, pushing rates too high during inflationary episodes and too low during disinflationary ones.  
- In contrast, the optimized path adapts more smoothly to macroeconomic conditions, producing lower overall losses.

---

## Future Directions
Currently, this project serves as a **proof of concept**. Moving forward, I plan to extend it along several dimensions to make it more realistic and robust:
- **Regime-switching coefficients:** Capture changes in economic behavior across regimes (e.g., high vs. low inflation).  
- **Shock variety:** Go beyond random noise to analyze structured scenarios such as asset bubbles, recessions, or supply-side shocks.  
- **Broader economic features:** Incorporate financial markets, trade, and external sector dynamics.  
- **DSGE extensions:** Introduce elements from Dynamic Stochastic General Equilibrium (DSGE) models to strengthen the theoretical foundations.  
