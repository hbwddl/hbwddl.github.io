---
layout: archive
title: "Code"
permalink: /codepage/
author_profile: true
redirect_from:
  - /codepage
---

{% include base_path %}

SEIR Simulation
------
This is a simulation of an SEIR (Susceptible-Exposed-Infected-Recovered) model using Gillespie's algorithm for simulating continuous-time Markov processes and [Sellke's threshold](https://www.jstor.org/stable/3213811?seq=1#metadata_info_tab_contents) for modeling the exposure threshold.

[SEIR simulation in Rshiny](https://hbwaddel.shinyapps.io/seir_sellke_threshold/) : 
[Github Repository for Infectious Disease/Phylodynamics Simulations](https://github.com/hbwddl/Phylodynamics_Simulations)

2D "density" generator
------
For some of my movement modeling work, I wanted a quick way to generate a 2d spatial "density" for the purposes of simulations. This application generates a function defined over a 2-dimensional square by overlaying multiple bivariate normal distributions on top of each other. I keep saying "density", because the function doesn't necessarily integrate to 1. 

[Density Generator in RShiny](https://hbwaddel.shinyapps.io/GenerateDensity/) : 
[Github Repository](https://github.com/hbwddl/spatial-density-generator/)

BIOS 591P R Materials
------
For my TA duties for BIOS 591P (Biostatistical Methods II), I translate SAS analyses into R code for students who opt to learn R programming. These files were used in the Spring 2022 semester. More information can be found on my teaching page.

[Github Repository](https://github.com/hbwddl/BIOS-591P-2022)

Applied Spatial Statistics for Public Health Data
------
Found on my [github](https://github.com/hbwddl/Bios-737-Applied-Spatial-2019). This repository contains my code for the course Bios 737, which I took in Fall 2019. The course primarily focused on spatial point processes.
