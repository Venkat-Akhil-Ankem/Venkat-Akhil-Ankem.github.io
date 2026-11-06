---
layout: page
title: OR-Verifier
description: Solver-verified evaluation and GRPO training for LLMs that write optimisation models.
importance: 2
category: work
github: https://github.com/Venkat-Akhil-Ankem/or-verifier
---

An LLM reads a plain-English operations-research problem and writes a Python `solve(data)` function. The code runs in a sandbox on visible **and hidden** instances, and an independent checker recomputes feasibility and objective value against the **proven optimum from an exact MILP solver (HiGHS)**. The same solver verdict doubles as the reward for GRPO training — the solver *is* the reward function.

**Benchmark.** 40 tasks across 8 problem families (knapsack, assignment, transportation, production planning, facility location, machine scheduling, set cover, open-pit block selection). Reference solutions score 40/40; greedy heuristics are caught as suboptimal.

**Agent.** Generate → verify → repair loop with three feedback modes (single attempt, repair from visible-instance errors, repair with oracle optimum), plus a failure taxonomy and per-family metrics.

**RL.** GRPO training setup (TRL + LoRA) with a shaped verifiable reward — format, runs, feasible, visible-optimal, hidden-optimal — and a before/after evaluation protocol on benchmark instances disjoint from training data. Training code is complete but not yet run (needs a GPU); no improvement is claimed.

**Stack.** Python, PyTorch, TRL, PuLP/HiGHS, Anthropic API, pytest (74 tests).
