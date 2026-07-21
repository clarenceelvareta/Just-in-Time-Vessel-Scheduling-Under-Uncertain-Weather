# Just-in-Time Vessel Scheduling Under Uncertain Weather
This project develops an optimization model for Just-in-Time (JIT) vessel arrivals at the Port of Singapore under uncertain weather conditions. The model minimizes total operational cost by jointly optimizing airborne and ground delays while balancing schedule reliability, anchorage waiting, and slow steaming decisions.

## Background 
With Singapore having the world’s busiest transshipment hubs and the ongoing transition towards the Tuas Megaport alongside the MPA’s push for ‘Just-in-Time’ arrivals to support Singapore’s Green Plan, we are attempting to solve the JIT arrival problem under uncertainty. 

## Problem Statement
How might we optimize vessel arrival schedules under uncertain weather and port conditions to enable reliable schedule arrivals at the Port of Singapore?

## Features
- Route optimization
- Cost-time tradeoff analysis
- Visualization of optimized routes
- Python implementation

## Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Julia

## Methodology
- Formulated the problem as a stochastic optimization model.
- Modelled uncertain weather scenarios using probability distributions.
- Optimized vessel scheduling across 48 time slots.
- Compared anchorage waiting and slow steaming strategies.
- Evaluated total operational costs under multiple scenarios.

## Results
- The model successfully schedules 94 vessels across 48 time slots under uncertain weather, achieving a total expected cost of $1,780,392 per operating day.
- The model naturally discovers a hybrid strategy (anchor for short delays, slow-steam for delays beyond 10 - 14 hours).
- The planning proves essential: Sumatra Squalls (15% probability) reduce large-berth capacity to zero.
- The 10 a.m. peak (7 vessels, 5 of them large) with only 2 large berths available per slot is the single biggest cost driver.
- Future work should incorporate real-time AIS updates to adjust JIT commands as live weather forecasts evolve throughout the day.
