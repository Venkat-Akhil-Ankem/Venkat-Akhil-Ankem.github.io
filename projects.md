# Projects

[Home](index) | [Research](research) | [Publications](publications) | [CV](cv) | [Contact](contact)

## Research projects (Ph.D. work)

### Open-Pit Mine Scheduling Optimizer
Large-scale MILP formulation and solution methods for long-term open-pit mine planning, developed with Rio Tinto under a MITACS industrial collaboration.
- **Problem:** multi-period block-extraction scheduling with precedence and resource constraints, at a scale generic solvers can't handle directly
- **Approach:** custom cutting planes, rolling-horizon decomposition, Large Neighborhood Search
- **Result:** 90% reduction in computation time vs. the baseline approach
- **Stack:** C++, Gurobi, OpenMP

### Relax-and-Repair Optimization Framework
A framework for quickly generating feasible solutions to MILP models too large to solve to optimality in reasonable time, using constraint relaxation, slack variables, and penalty-based repair.

### Machine Learning for MILP Difficulty Prediction
GNN- and supervised-learning models that predict how hard a mine-scheduling MILP instance will be to solve, and use that prediction to guide solver strategy and initialization before a run starts.
- **Stack:** Python, PyTorch, scikit-learn

---

## Independent / portfolio projects

> **Note to self before publishing:** the repos below are what's actually public on [GitHub](https://github.com/Venkat-Akhil-Ankem) today — `Pyomo_learning_1`, `Pyomo_learning_2`, `mine-scheduling-ml-fixing`, `MineLib`. Several are unnamed/undescribed on GitHub itself and read as practice notebooks rather than finished projects. Before linking them here, either (a) give each one a proper README with problem/approach/result and a one-line GitHub description, or (b) pull the polished ones into new repos named to match what you call them here. A recruiter who clicks through and finds a mismatch between "Mine Production AI Optimizer" here and "Pyomo_learning_1" on GitHub will trust the rest of the site less — better to under-promise and link only what's genuinely presentable.

- **MineLib** — [github.com/Venkat-Akhil-Ankem/MineLib](https://github.com/Venkat-Akhil-Ankem/MineLib)
- **Mine scheduling ML fixing** — [github.com/Venkat-Akhil-Ankem/mine-scheduling-ml-fixing](https://github.com/Venkat-Akhil-Ankem/mine-scheduling-ml-fixing)
- **Pyomo learning series** — [Pyomo_learning_1](https://github.com/Venkat-Akhil-Ankem/Pyomo_learning_1), [Pyomo_learning_2](https://github.com/Venkat-Akhil-Ankem/Pyomo_learning_2)

## Future application directions

Transportation optimization, airline and flight operations, sustainable energy systems, and other data-driven industrial optimization problems.
