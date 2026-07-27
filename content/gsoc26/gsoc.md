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

## Week 5-6

This week, we have added another ICNN tuorial, this time using PyTorch. The PR for it can be viewed [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/287). We have also added a small training loop to both `Flux` [tutorial](https://lanl-ansi.github.io/MathOptAI.jl/stable/tutorials/input_convex/) and `PyTorch` [tutorial](https://lanl-ansi.github.io/MathOptAI.jl/stable/tutorials/input_convex_pytorch/) to show the fit on a convex function.

We have also finalized and added [`SoftPlusConicEpigraph`](https://lanl-ansi.github.io/MathOptAI.jl/dev/api/#SoftPlusConicEpigraph) with test using `SCS`. The PR for it can be viewed [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/288).

## Week 7-8

We wanted to implemennt the epigraph formulation of `LeakyReLU` but the way the predictor has been implemented, it wal already working so we just needed to add the tests. PR is [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/293).

The input convex `Flux` [tutorial](https://lanl-ansi.github.io/MathOptAI.jl/stable/tutorials/input_convex/) is updated to include `SoftPlusConicEpigraph`. We just changed the last layer of the ICNN and the fit seems to improve well. We did the same for the PyTorch [tutorial](https://lanl-ansi.github.io/MathOptAI.jl/stable/tutorials/input_convex_pytorch/) as well.

We proceeded to add support for epigraph formulations to `ExaModels`. PR can be found [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/294).