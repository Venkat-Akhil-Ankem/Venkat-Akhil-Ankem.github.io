---
layout: page
title: ML Scheduling Difficulty Predictor
description: PyTorch neural network that predicts whether a scheduling instance is hard or easy — without running a solver.
importance: 6
category: work
github: https://github.com/Venkat-Akhil-Ankem/ml-scheduling-difficulty
---

A PyTorch neural network that learns to predict whether a combinatorial scheduling problem instance is **hard** or **easy** to solve — purely from structural features of the instance, without ever running a solver.

**Problem.** Instance hardness prediction is an active research problem with direct uses in algorithm selection, portfolio solvers, and adaptive parameter tuning.

**Approach.**
- Feature engineering over instance structure: number of jobs, machines, constraint density, load balance
- Binary classifier (easy vs. hard relative to a solve-time threshold)
- Knowing difficulty *before* solving lets a planner pick the right algorithm and allocate compute

**Stack.** Python, PyTorch, scikit-learn.
