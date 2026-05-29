V2 Fab System Model

Enhanced version of the semiconductor cycle time simulation project.

Focus:

System-level behavior (not just process-level simulation)
Queue dynamics and WIP accumulation
Capacity and utilization modeling
Bottleneck identification under load
Tail-risk planning (P90 / P95)
Scenario-based decision analysis

Key Improvements over V1:

Introduces system interaction effects (queue + WIP)
Models capacity constraints explicitly
Identifies dynamic bottlenecks under system load
Simulates instability under high utilization (>1)
Adds planning-oriented decision framework

Core Insight:

Fab performance is not driven by process times alone,
but by interactions between arrival rate, capacity, and queue dynamics.

Planning must therefore shift from:
Mean-based thinking → Tail-risk and system-level thinking
