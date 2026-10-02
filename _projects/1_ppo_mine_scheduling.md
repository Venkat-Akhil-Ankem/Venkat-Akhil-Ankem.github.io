---
layout: page
title: PPO Mine Block Sequencing
description: Deep reinforcement learning agent that learns NPV-maximising open-pit extraction sequences.
importance: 1
category: work
github: https://github.com/Venkat-Akhil-Ankem/ppo-mine-scheduling
---

A deep reinforcement learning agent built **from scratch in PyTorch** that learns near-optimal open-pit mine block extraction sequences.

**Problem.** Open-pit mine production scheduling is a large-scale MILP: decide which blocks to extract in each period to maximise net present value (NPV), subject to precedence constraints (a block can only be extracted after the blocks above it) and per-period mining/processing capacity limits.

**Approach.**
- PPO actor-critic with Generalised Advantage Estimation (GAE)
- Action masking over precedence-feasible blocks, so every sampled action respects the block precedence graph
- Curriculum learning: train on small instances, transfer to larger ones
- MineLib-format instance parsing

**Evaluation.** Benchmarked against greedy extraction baselines and the LP-relaxation upper bound.

**Stack.** Python, PyTorch, NumPy, MineLib format, pytest.
