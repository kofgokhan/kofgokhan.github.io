+++
date = "2026-05-15T17:24:49+03:00"
draft = false
title = "GSoC '26"
+++

I will post any updates here on this page.

I might add more details later in order to make these more useful than just a simple log of activities.

## Week 1-2

So far I have a good handle on how the package MathOptAI.jl works and how the workflow of implementing a new predictor should be handled. I have implemented `ReLUEpigraph` and currently testing it on a practical problem.

I have also developed a `Flux` model which is an Input Convex Neural Network (ICNN) that can be embedded in a `JuMP.Model` and using `ReLUEpigraph` enables the ICNN to be represented with an LP formulation. The PR for the `ReLUEpigraph` is created [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/274).

## Week 3-4

Currently working on conic reformulations and more epigraph formulations. Activation functions like `softplus` can be represented with exponential cones and then we can use solvers like [MOSEK](https://github.com/MOSEK/Mosek.jl) or [SCS](https://github.com/jump-dev/SCS.jl) to solve the conic problems.

I have also submitted a PR for the `Flux` tutorial of ICNN. It can be viewed [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/279).