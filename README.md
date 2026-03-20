# Competition Modelling Project (Android vs iOS Market Dynamics)

## Project Overview

This project studies competition between two technological systems using a nonlinear dynamical model.  
We use real market share data of Android and iOS to understand how competing platforms evolve over time, how dominance appears, and how market dynamics change.

The goal of the project is to check whether nonlinear competition models (similar to Lotka–Volterra / logistic models) can describe real-world market behaviour, explain stability, and detect regime shifts in technological ecosystems.


## Model Used

We use a nonlinear competition model with shared market capacity:

dx/dt = r1 * x * (1 - (x + y)/K) - alpha * x * y  
dy/dt = r2 * y * (1 - (x + y)/K) - beta * x * y  

where

- x = Android market share  
- y = iOS market share  
- K = total market capacity  
- r1, r2 = growth rates  
- alpha, beta = competition coefficients  


## Project Pipeline

The project follows a structured modelling pipeline:

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


## Work Completed

### Literature Review
- Studied logistic, diffusion, Lotka–Volterra, and nonlinear competition models
- Compared different modelling approaches
- Identified need for nonlinear phase-wise modelling

### Data Analysis
- Cleaned and converted real Android–iOS market share data
- Checked saturation, trends, and phase change

### Model Justification
- Compared regression, diffusion, and dynamical models
- Justified nonlinear competition model with shared capacity

### Parameter Fitting and Simulation Validation
Three fitting methods were tested:

1. Derivative fitting  
   - unstable due to noise amplification  
   - poor simulation results  

2. Single trajectory fitting  
   - reasonable fit for Android  
   - failed to capture phase change  

3. Piecewise trajectory fitting (best)
   - different parameters for different phases
   - realistic simulation
   - captures change in dynamics

Conclusion:
Real market behaviour cannot be described using a single parameter set.

### Equilibrium Analysis
- Solved nonlinear model analytically
- Found equilibrium points:
  - (0,0)
  - (K,0)
  - (0,K)
- No coexistence equilibrium

### Stability Analysis
- Computed Jacobian matrix
- Calculated eigenvalues
- Phase 1 → Android dominance stable
- Phase 2 → iOS dominance stable

### Phase Comparison & Regime Shift
- Parameters change between phases
- Stable equilibrium changes
- System moves to new regime
- Indicates structural change in market dynamics

### Parameter Interpretation
- r1, r2 → growth rates
- K → market capacity
- alpha, beta → competition strength
- Early phase → expansion regime
- Later phase → saturation regime
- Change in parameters explains regime shift

### Real-World Interpretation
- Market has limited capacity
- Competition strength changes over time
- Dominance emerges after saturation
- Phase-wise modelling needed for real systems


## Current Status

Completed:

✔ Literature review  
✔ Data analysis  
✔ Model justification  
✔ Parameter fitting  
✔ Simulation validation  
✔ Equilibrium analysis  
✔ Stability analysis  
✔ Phase comparison  
✔ Parameter interpretation  
✔ Real-world interpretation  

Remaining:

- Prediction / forecasting stage (optional)
- Final report polishing


## Goal of the Project

- Study competition dynamics using real data
- Understand dominance in technological ecosystems
- Detect regime shifts in nonlinear systems
- Connect mathematical modelling with real-world behaviour
- Show why phase-wise modelling is needed in real markets