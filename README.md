# Transportation Mode Choice Model Calibration

## Project Overview
This repository contains an advanced Excel-based travel demand model. The project demonstrates the calibration of a Discrete Choice Model (DCM) to predict commuter preferences between traditional and innovative transportation modes.

## Technical Methodology
* **Algorithm:** Multinomial Logit Model (MNL)
* **Optimization:** Maximum Likelihood Estimation (MLE) used to calibrate beta coefficients by maximizing the sum of the log-likelihood (`Ln(p)`).
* **Utility Functions:** Calculated the systematic utility for competing transit alternatives based on multiple variables.

## Key Attributes Analyzed
The probability of mode selection was modeled against the following independent variables:
* **Travel Time (`MIN`)**
* **Service Reliability (`REL`)**
* **Financial Cost (`COST`)**
* **Alternative Specific Attributes (`ASA`)**

## Skills Demonstrated
This project highlights a strong foundation in macroscopic transport planning, commuter behavioral modeling, and the ability to build mathematical optimization frameworks directly within spreadsheet software.
