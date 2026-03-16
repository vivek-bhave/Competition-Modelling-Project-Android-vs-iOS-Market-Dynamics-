# Competition Modelling Project (Android vs iOS Market Dynamics)

## Project Overview

This project studies competition between two systems using a nonlinear mathematical model.
We use real market share data of Android and iOS to understand how competing technologies evolve over time.

The goal of the project is to check whether classical competition models (similar to Lotka–Volterra / logistic models) can describe real-world market behavior and explain dominance, coexistence, and stability.

## Model Used

We use a nonlinear competition model with shared market capacity:

dx/dt = r1 * x * (1 - (x + y)/K) - alpha * x * y
dy/dt = r2 * y * (1 - (x + y)/K) - beta * x * y

where:

* x = Android market share
* y = iOS market share
* K = total market capacity
* r1, r2 = growth rates
* alpha, beta = competition coefficients

## Work Done So Far

* Collected and cleaned real market share data
* Converted data to fraction form
* Implemented nonlinear competition model
* Estimated parameters using optimization
* Performed simulation using fitted parameters
* Compared simulation with real data
* Observed that different time periods may require different parameters

## Planned Pipeline

We will complete the project using the following steps:

1. Literature review
2. Data analysis
3. Model justification
4. Parameter fitting
5. Simulation validation
6. Prediction
7. Equilibrium analysis
8. Stability analysis
9. Phase comparison & regime shift
10. Parameter interpretation
11. Real-world meaning / policy relevance

## Current Status

Parameter fitting and simulation validation have been completed.
Remaining stages will be implemented step by step following the pipeline above.

## Goal of the Project

* Study competition dynamics using real data
* Check if nonlinear models explain market behavior
* Analyze stability and long-term outcomes
* Understand how dominance appears in technological ecosystems
* Connect mathematical results with real-world interpretation
