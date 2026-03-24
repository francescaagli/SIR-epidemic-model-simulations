# SIR epidemic model simulations

## Project description
This project is a simulation of the spread of an epidemic using the SIR (Susceptible-Infected-Recovered) model. The system of ordinary differential equations (ODEs) was solved numerically using a fourth-order Runge-Kutta integrator (RK4). A sensitivity analysis was performed varying the infection rate ( \beta ) and the recovery rate ( \gamma ).

## Mathematical Model
The SIR model describes the time evolution of three compartments:
( S(t) ): susceptible individuals
( I(t) ): infected individuals
( R(t) ): recovered individuals
The dynamics are governed by:
[
\frac{dS}{dt} = -\beta \frac{SI}{N}
]

[
\frac{dI}{dt} = \beta \frac{SI}{N} - \gamma I
]

[
\frac{dR}{dt} = \gamma I
]
where:
( \beta ) = infection rate
( \gamma ) = recovery rate
( N = S + I + R ) = total population

## Sensitivity measure

Sensitivity is computed as:
[
S_p = \left| \frac{Y(p + \Delta p) - Y(p)}{Y(p)} \cdot \frac{p}{\Delta p} \right|
]
where ( Y ) is a model output.

## Repository files

- `SIR.ipynb` – Jupyter notebook.
