---
title: "Research"
description: "Geodynamics, subduction-zone fluid and heat transport, and computational methods for the solid Earth."
showTableOfContents: true
cascade:
  showReadingTime: false
---

My research asks how the deep Earth transports mass, heat, and fluids — and how we can
constrain those processes with the sparse, indirect observations we actually have. That
question pulls in geodynamic modeling, petrology, thermochronology, and a fair amount of
numerical methods work.

## Subduction-zone fluid and heat transport

At Miami I model coupled fluid and heat transport in subduction zones, with a focus on
how mineral phase stability controls where water is bound, carried, and released. The
thermal structure of a subduction zone is not static: it evolves over the lifetime of the
margin, and that evolution changes which dehydration reactions run and where.

Work with Epstein, Condit, Holt, and Guevara showed that this evolving thermal structure
drives far more extensive hydration of the forearc mantle wedge than steady-state models
predict — a result with direct consequences for seismicity, arc volcanism, and the global
water budget.

## Foundering and relamination of the lower crust

My dissertation work combined numerical modeling with xenolith constraints to ask what
happens to dense lower crust once it becomes gravitationally unstable. Does it founder
into the mantle, or does buoyant material relaminate to the base of the crust?

Using hydro-thermo-mechanical models (a modified I2VIS code from ETH) together with
Generalized Additive Models fit to sediment-melting experiments, I quantified how much
sediment should relaminate versus founder across an array of subduction zones. The Pamir
— where deep xenoliths give an unusually direct window into lower-crustal conditions —
served as the natural laboratory.

## Thermochronology and sensitivity analysis

Thermochronological dates are the product of a thermal history and a radiation-damage
model, and both carry real uncertainty. I've worked on quantifying how much: conducting
global sensitivity analysis to determine which parts of a thermal history a date actually
constrains, and which are effectively unconstrained.

This became [COAST.jl](https://github.com/ryanstoner1/COAST.jl), a Julia package for
sensitivity-analysis modeling of geologic thermal histories. Earlier work paired Raman
spectroscopy with zircon (U-Th)/He dating to characterize radiation damage in Kaapvaal
Craton samples.

## Computational and open-science work

A recurring thread is that the modeling tools themselves need work. I contribute to
[ASPECT](https://aspect.geodynamics.org/), the community finite-element code for mantle
convection, and I'm interested in automatic differentiation as a route to tractable
adjoint-based inversion for geodynamic problems.

Where possible I build on publicly available data and release code openly, so that
results can be reproduced rather than taken on faith.
