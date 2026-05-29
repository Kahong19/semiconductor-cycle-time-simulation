# Semiconductor Manufacturing Cycle Time Simulation (V1 → V2)

## Overview

This repository contains an evolving simulation framework for semiconductor manufacturing cycle time analysis.

The project demonstrates how stochastic process variability affects production performance, and how modeling evolves from process-level simulation (V1) to system-level behavior analysis (V2).

## Project Evolution

# V1 – Cycle Time Model
Focus: Process-level simulation

- Cycle time analysis per wafer lot
- Process variability modeling
- P90 / P95 planning metrics
- Sensitivity analysis under variability

Insight:
Demonstrates how variability affects cycle time distribution at the process level.

# V2 – Fab System Model
Focus: System-level behavior

- Queueing effects and WIP accumulation
- Capacity and utilization modeling
- Bottleneck identification under load
- System instability under high utilization
- Scenario-based planning and decision analysis

Insight:
Demonstrates that system performance is driven not only by process time, but by interactions between arrival rate, capacity, and queue dynamics.

## Key Conceptual Shift

V1 → Process Thinking

V2 → System Thinking

From:
Independent lot cycle time modeling

To:
Interdependent system dynamics with congestion effects

## Core Insights

Mean cycle time is insufficient for planning decisions
P90 / P95 better represent operational risk
System congestion emerges from utilization > capacity
Bottlenecks are dynamic under load, not static
Variability has amplified impact at system level

## Repository Structure

V1_Cycle_Time_Model/
Original cycle time simulation (process-level model)

V2_Fab_System_Model/
Enhanced system-level simulation (queueing + planning model)

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## How to Run

pip install numpy pandas matplotlib
