+++
date = "2026-05-15T17:24:49+03:00"
draft = false
title = "GSoC '26"
+++

I will post any updates here on this page.

I might add more details later in order to make these more useful than just a simple log of activities.

# Week 1-2

So far I have a good handle on how the package MathOptAI.jl works and how the workflow of implementing a new predictor should be handled. I have implemented `ReLUEpigraph` and currently testing it on a practical problem.

I have also developed a `Flux` model which is an Input Convex Neural Network (ICNN) that can be embedded in a `JuMP.Model` and using `ReLUEpigraph` enables the ICNN to be represented with an LP formulation. The PR for the `ReLUEpigraph` is created [here](https://github.com/lanl-ansi/MathOptAI.jl/pull/274).