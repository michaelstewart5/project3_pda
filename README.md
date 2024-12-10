# Simulation Study on Model Performance and Budget Constraints

## Overview

This project explores the performance of statistical models under different configurations of cluster sizes and observations per cluster. The simulation study investigates how variations in the number of clusters, the number of observations per cluster, and different intra-cluster correlation (ICC) levels affect model performance metrics such as bias, mean squared error (MSE), standard error (SE), and coverage. Additionally, the project incorporates budget constraints and aims to optimize the allocation of resources based on these constraints to minimize variance in model parameter estimates.

The analysis uses mixed-effects models to assess treatment effects while accounting for cluster-level variation, and investigates the impact of cost on achieving optimal model performance. The results can guide the design of cost-effective and efficient experiments in future research.

## Data

The data for this simulation study is synthetically generated under controlled conditions. The main parameters of the simulation include:
- **Number of Clusters (g)**: Varying from 10 to 100.
- **Observations per Cluster (r)**: Varying from 10 to 500.
- **Intra-cluster Correlation (ICC)**: Varying values of 0.05, 0.1, and 0.2.
- **Variance (sigma_sq)**: Varying from 1 to 3.
- **Treatment Effect (beta)**: Various effect sizes tested (0.2, 0.5, 0.8).

The simulation results include estimates of model performance, such as bias, MSE, SE, and coverage, under different settings.

## Main Dependencies

The project uses R (version 4.2.3) for analysis. The following R packages are required:

- **lme4** (version 1.1-31)
- **tidyverse** (version 2.0.0)
- **gt** (version 0.8.0)
- **kableExtra** (version 1.4.0)
- **ggplot2** (version 3.4.1)
