# RWiener Tutorial

## Overview
- RWiener package provides R functions for the Wiener diffusion model.
- For further Information check:
  - https://cran.r-project.org/web/packages/RWiener/index.html
  - https://github.com/cran/RWiener/tree/master

## 1. Basic Tutorial
The tutorial begins by setting up the R environment and providing a brief overview of the functions and parameters associated with the diffusion model.
The functions introduced include `dwiener`, `pwiener`, `qwiener`, `rwiener`, `nlm`, and `optim`.
The parameters of the diffusion model discussed are α (boundary separation), 𝜏 (non-decision time), β (initial bias), and δ (drift rate parameter).
There's also a note on the Maximum likelihood estimation method using rWiener.


### 1.1 Defining Dataset and Parameters:

A dataset is generated using the rwiener function with 100 observations and parameters like boundary separation, non-decision time, bias, and drift rate.

### 1.2 d-Wiener-function:

This section demonstrates how to obtain the density of a specific quantile using the dwiener function.

### 1.3 p-Wiener function:

The tutorial explains how to calculate the cumulative distribution using the pwiener function.

### 1.4 q-Wiener function:

The inverse CDF function, qwiener, is introduced to find the appropriate quantile for a given probability.

### 1.5 Plot-function:

The wiener_plot function is used to visualize the observed lower and upper responses.

### 1.6 Model fitting:

The tutorial demonstrates how to fit the diffusion model to the data using optimization algorithms like Nelder-Mead and BFGS.
Comparing Model vs. Real Data:

The tutorial provides code to generate modeled data and compare it to real data using density plots.
### 1.7 Criteria:

This section introduces various criteria functions like `wiener_likelihood`, `wiener_deviance`, `wiener_aic`, and `wiener_bic` to evaluate the fit of the model.

### 1.8 Full Analysis Pipeline
The tutorial provides a comprehensive pipeline for analyzing the data:
- Pipeline Part 1: Parameter Estimation for each participant.
- Pipeline Part 2: Estimation parameters are extracted.
- Pipeline Part 3: Modeled data is generated.
- Pipeline Part 4: Modeled and real data are compared.
- Mean Parameters of Model vs. Real Data: The tutorial concludes by plotting the mean parameters of the model against the real data.