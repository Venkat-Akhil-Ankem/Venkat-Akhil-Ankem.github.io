---
layout: page
title: GNN for MILP Difficulty Prediction
description: Machine-learning models that predict MILP instance difficulty and guide solver strategy.
importance: 2
category: work
github: https://github.com/Venkat-Akhil-Ankem/mine-ai-optimizer
---

The applied-ML core of my third Ph.D. project: learning to predict how hard a MILP instance will be to solve, and using that prediction to guide solver strategy.

**Problem.** On industrial open-pit scheduling instances with 100,000+ variables, solver behaviour varies enormously across instances. Knowing difficulty ahead of time lets a planner pick the right algorithm, allocate compute, and warm-start effectively.

**Approach.**
- Graph neural networks and supervised models (scikit-learn, PyTorch) trained on instance structure
- Large-scale benchmark datasets generated via structured augmentation strategies across real-life Rio Tinto mine instances
- Models predict solve time / difficulty and recommend solver configurations

**Stack.** Python, PyTorch, scikit-learn, Graph Neural Networks, Gurobi.
