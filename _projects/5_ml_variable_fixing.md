---
layout: page
title: ML-Guided Variable Fixing for Mine Scheduling
description: Machine learning to accelerate Gurobi on open-pit mine production scheduling MIPs.
importance: 5
category: work
github: https://github.com/Venkat-Akhil-Ankem/mine-scheduling-ml-fixing
---

Using machine learning to accelerate Gurobi on the Constrained Pit (CPIT) open-pit mine production scheduling problem — a large-scale binary MIP.

**Problem.** The CPIT model decides binary variables x[b,t] (extract block *b* in period *t*) to maximise net present value, subject to precedence (slope stability), extraction capacity, and resource bounds. Real-world instances with thousands of blocks and tens of periods are expensive to solve to optimality.

**Approach.** Train ML models to predict which binary variables can be fixed to 0/1 with high confidence, shrinking the MIP before handing it to Gurobi — trading a small, controlled optimality risk for large speedups.

**Stack.** Python, Gurobi, scikit-learn.
