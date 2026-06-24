# Discrete Choice Model Calibration (Excel) 📊🚗

## Overview
This repository contains a fully transparent, spreadsheet-based implementation for calibrating **Discrete Choice Models**, specifically the Multinomial Logit (MNL) model. 

While modern travel demand modeling often relies on Python or R packages (like Biogeme), this Excel-based approach was engineered to demonstrate a fundamental, "white-box" mathematical understanding of Utility Theory, probability calculations, and the Maximum Likelihood Estimation (MLE) optimization process.

## Mathematical Architecture & Workflow
This workbook is structured to process revealed preference (RP) or stated preference (SP) travel data through the following pipeline:

1. **Utility Function Formulation:** * Calculates deterministic utility ($V_{in}$) for different transport modes based on explicit parameters such as travel time, cost, and alternative-specific constants (ASCs).
2. **Logit Probability Calculation:** * Implements the core MNL mathematical framework to calculate the probability of an individual choosing a specific mode: $P_i = e^{V_i} / \sum e^{V_j}$.
3. **Log-Likelihood Maximization:** * Constructs the log-likelihood function across the entire dataset, mapping the calculated probabilities to the actual observed choices.
4. **Parameter Optimization (Solver):** * Utilizes the **Excel GRG Nonlinear Solver** engine to iteratively adjust the $\beta$ parameters (Value of Time, cost coefficients, etc.) until the maximum log-likelihood is achieved, thereby calibrating the model to the observed data.

## Key Engineering Takeaways
* **Mathematical Transparency:** Proves an applied understanding of non-linear optimization and econometric modeling.
* **Economic Valuation:** Extracts critical behavioral indicators, such as the Value of Travel Time Savings (VTTS), directly from the calibrated $\beta$ coefficients.
* **Algorithm Mechanics:** Demonstrates how maximum likelihood algorithms converge on optimal solutions under mathematical constraints.

## Tech Stack
* **Software:** Advanced Microsoft Excel
* **Optimization Engine:** Excel Solver Add-in (GRG Nonlinear)
* **Domain:** Travel Demand Modeling, Transport Economics, Behavioral Econometrics
