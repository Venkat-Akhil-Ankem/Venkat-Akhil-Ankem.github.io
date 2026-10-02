---
layout: page
title: RL Job Scheduler
description: Tabular Q-learning agent for parallel machine scheduling.
importance: 3
category: work
github: https://github.com/Venkat-Akhil-Ankem/rl-job-scheduler
---

A reinforcement learning agent for **parallel machine scheduling** — assigning jobs to machines over time to minimise makespan and tardiness.

**Problem.** Classical scheduling is NP-hard; dispatching rules are fast but myopic. A tabular Q-learning agent learns a scheduling policy from experience, trading off exploration and exploitation across episodes.

**Approach.**
- Tabular Q-learning with ε-greedy exploration
- State: machine availability and remaining job queue; actions: job-to-machine assignments
- Reward shaped around makespan and completion-time objectives
- Compared against standard dispatching-rule baselines

**Stack.** Python, NumPy.
