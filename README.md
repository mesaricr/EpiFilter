# EpiFilter
Optimised estimates of reproduction numbers (R) over time.

Uses Bayesian recursive filtering and smoothing to maximise the incidence data used.
Takes a forward-backward approach and provides estimates that combine advantages of EpiEstim and the Wallinga-Teunis method.
Method is exact (and optimal given a grid over R) and deterministic (produces the same answer on the same data).

For full details see: 
Parag, KV, (2020) “Improved real-time estimation of reproduction numbers at low case incidence and between epidemic waves” medRxiv.

Here we provide Matlab and R code to implement the main methods described in the text.

Main functions: epiFilter (or epiFilterSm) performs forward filtering to generate causal R estimates.
              : epiSmooth performs backward smoothing to generate R estimates that use all possible information.
              : recursPredict provides one-step-ahead predictions
