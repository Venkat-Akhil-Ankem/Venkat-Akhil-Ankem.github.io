# Research

[Home](index) | [Projects](projects) | [Publications](publications) | [CV](cv) | [Contact](contact)

My doctoral research addresses the **Open-Pit Mine Production Scheduling Problem (OPMPSP)** — a large-scale mixed-integer optimization problem involving multi-period block-extraction decisions, precedence constraints, and resource limits, at a scale where exact solvers alone don't finish in time and heuristics alone aren't strong enough.

## Contributions

- **Cutting planes** that strengthen the MILP formulation directly, tightening LP relaxation bounds and reducing branch-and-bound search on instances with 100,000+ variables
- **Relax-and-repair frameworks** and a parallel warm-start hybrid heuristic for quickly obtaining feasible solutions on instances too large to solve to optimality
- **Rolling-horizon decomposition** to break multi-period planning into tractable sub-problems without losing solution quality
- **Graph neural networks and supervised ML** to predict instance difficulty and steer solver strategy before a run starts, trained on benchmark datasets built from Rio Tinto's real mine models via structured augmentation
- Research software engineering (C++/OpenMP, Python) to make these methods reproducible at industrial scale

## Impact

Through a three-year MITACS industrial collaboration with Rio Tinto, these methods cut mine-scheduling computation time by **90%** and time-to-feasibility by **80%** — and were deployed directly into Rio Tinto's production planning workflows, not left as a research prototype. The formal collaboration ran 2022–2025; I continue monthly technical check-ins with the team. See [Publications](publications) for the papers and [Projects](projects) for the software this work produced.

## Application areas

Mining operations and mine production scheduling are the primary testbed, but the underlying methods — MILP strengthening, decomposition, and ML-guided heuristics — generalize to transportation and logistics, aviation and flight operations, and other large-scale industrial decision-support systems.

## Research vision

I want optimization methods that are mathematically strong, computationally scalable, and actually deployable — which in practice means exact methods, heuristics, and software design have to be designed together, not bolted on after the fact.
