---
layout: default
title: Aircraft Performance Simulator
---

# Aircraft Performance & Emissions Simulator
*Tools: MATLAB, Numerical Integration (RK4)*
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/claire-m-richardson/portfolio/blob/main/sustainable_aircraft_sim.ipynb)

## Executive Summary
I developed a flight-cycle simulator to quantify the reduction in carbon emissions when transitioning from Jet-A1 to Sustainable Aviation Fuel (SAF) on a long-range business jet platform.

## Technical Implementation
The model solves the following energy balance for a quasi-steady climb and cruise:
$$T = D + W \sin(\gamma)$$

I implemented an LU decomposition to solve for aerodynamic coefficients and used MATLAB's `ode45` to track mass depletion over a 3,000 nautical mile mission.

## Key Findings
* Switching to 100% SAF resulted in a net lifecycle CO2 reduction of **80%**.
* Optimized cruise altitudes for the model aircraft were found to be between 41,000 and 45,000 ft.
