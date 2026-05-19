# Semiconductor Manufacturing Cycle Time Simulation

## Overview

This project simulates a simplified semiconductor manufacturing process to analyze cycle time behavior under stochastic process variability.  
The goal is to demonstrate how variability impacts production planning and why tail-risk metrics (P90/P95) are important in operational decision-making.

---

## Problem Motivation

In semiconductor manufacturing, cycle time is not deterministic due to process variability across different production stages such as lithography, etching, cleaning, and testing.

Traditional planning often relies on average cycle time, which can underestimate delivery risk.

This project explores:
- How variability affects cycle time distribution
- Why mean-based planning is insufficient
- How tail metrics can improve planning robustness

---

## Model Design

The system simulates wafer lots flowing through 4 sequential process steps:

- Lithography
- Etching
- Cleaning
- Testing

Each process step is modeled using a normal distribution:

- Mean = nominal process time
- Std = process variability

Lot arrivals are generated using an exponential distribution to simulate stochastic job arrivals.

---

## Key Features

- Stochastic process simulation
- Cycle time computation per lot
- Statistical analysis (mean, std, distribution)
- Tail-risk metrics (P90, P95)
- Variability sensitivity analysis (+50% std scenario)
- Comparative scenario visualization

---

## Key Insights

- Mean cycle time remains relatively stable under increased variability
- P90 and P95 cycle times increase significantly with higher variability
- System performance is highly sensitive to process variation
- Planning should incorporate buffer based on tail-risk metrics, not just averages

---

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

---

## Files

- `fab_simulation.ipynb` → main simulation notebook
- `fab_simulation.html` → exported interactive report
- `fab_simulation.pdf` → printable report version

---

## How to Run

```bash
pip install numpy pandas matplotlib