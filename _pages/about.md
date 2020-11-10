---
permalink: /
title: "About"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I'm a PhD student at the University of Oklahoma, working with Prof. John Wisniewski. My current research is focused on high contrast imaging of young circumstellar disk systems (primarily with the Subaru Telescope's SCExAO/CHARIS) toward the goal of better understanding how planetary systems form and evolve.  More broadly, my interests lie in improving the value of data through:

- improvements to data processing and analysis techniques, especially on the software-side
- better visualizations for both processing techniques and products to facilitate the dissemination of results (both to laypeople and those in the field)

![](images/HD15115.png)

In a recent paper, we demonstrated the utility of the Differential Evolution (DE) optimization algorithm for quickly navigating disk model parameters by applying it  to SCExAO/CHARIS data of the famous debris disk of HD 15115 (above). While DE doesn't provide the same detailed information regarding the parameter space as exploration-focused algorithms – like Markov-Chain Monte Carlo (MCMC) – it requires many fewer models be evaluated (~$10^3$ versus ~$10^6$ for MCMC) and is better equipped for complex parameter spaces. This makes it especially well-suited for the time consuming forward modeling required for ground-based adaptive optics (AO) disk studies. In fact, most prior studies in this area simply explore a small, coarse grid of models to keep modeling times tractable. Based loosely the samples we explored for the two-ring model of HD 15115, I created a toy-model parameter space to visualize how differential evolution moves a population of trial solutions toward the global solution:

![](images/toymodel_de.gif)

To put the improvement offered by DE into perspective: the background contours in the toy-model visualization are drawn using a 12 point grid, meaning 12⁷ or ~36 million evaluations of our toy-model objective function. Noting that this is effectively a massive analog to the commonly implemented grid search: the DE run beats the best solution from the grid after only 1330 evaluations.

Going forward, model optimization with DE will enable us to form a clearer picture of what we've observed, and will thus allow for more detailed analysis of things like dust grain distributions and disk geometry.

 
