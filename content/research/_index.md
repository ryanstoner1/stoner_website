---
title: "Research"
description: "Geodynamics, subduction-zone fluid and heat transport, and computational methods for the solid Earth."
showTableOfContents: true
cascade:
  showReadingTime: false
---

I work on how tectonic processes can be constrained by their self-consistent evolution in
numerical geodynamic models — which pulls in geodynamics, petrology, thermochronology,
and a fair amount of numerical methods.

## Serpentinization and the plate interface

During subduction, the downgoing oceanic crust is exposed to high temperatures in the
mantle wedge, causing volatile-bearing minerals to break down and release hydrous fluids
into the forearc. These fluids percolate upwards, reacting with the mantle wedge to form
hydrated ultramafic lithologies, including serpentinite.

To accurately track the fate and impact of water on the forearc, we develop time-dependent
models that self-consistently capture both serpentinite ingrowth and the associated
rheological weakening of the plate interface. Unlike many subduction models that
investigate forearc serpentinization and prescribe plate velocities, geometries, or
steady-state conditions, our approach allows plates to evolve dynamically without
predefined velocities or geometries.

Subducting fully water-saturated sediments yield ~3× greater forearc serpentinite than the
moderately hydrated reference case. The water-saturated case produces a weaker interface
and, in turn, subduction zone convergence rates ~40% higher than in an endmember case with
anhydrous sediment. We find that hydrous sediments not only lubricate the interface
directly by weakening it, as previously suggested, but also by dehydrating and releasing
water that produces weak serpentinite in the mantle wedge — feedback only able to be
captured within fully coupled dynamic models.

## Thermal evolution and mantle wedge hydration

Hydration of the subduction zone forearc mantle wedge influences the downdip distribution
of seismicity, the availability of fluids for arc magmatism, and Earth's long-term water
cycle. Reconstructions of present-day subduction zone thermal structures using
time-invariant geodynamic models indicate relatively minor hydration, in contrast to many
geophysical and geologic observations.

By pairing a dynamic, time-evolving thermal model of subduction with phase equilibria
modeling, we found that the thermal state during the intermediate period of subduction —
as the slab freely descends through the upper mantle — promotes extensive forearc wedge
hydration. During early subduction the forearc is too hot to stabilize hydrous minerals in
the mantle wedge, while during mature subduction, slab dehydration dominantly occurs
beyond forearc depths.

Considering thermal evolution leads to an order of magnitude increase in estimates for
current extents of wedge hydration, suggesting the forearc mantle wedge represents a
potential vast reservoir of H₂O, on the order of 3.4–5.9 × 10²¹ g globally.

## Relamination, delamination, and foundering of the lower crust

My dissertation asked what happens to lower crust during continental collision, combining
numerical modeling with xenolith constraints.

I quantified the amount of sediment expected to relaminate and founder for an array of
subduction zones using numerical hydro-thermo-mechanical models (modified I2VIS code from
ETH), and fit models of sediment melting using Generalized Additive Models (GAMs) to
interpolate melt fraction and residuum densities. The Pamir — where deep xenoliths give an
unusually direct window into lower-crustal conditions — served as the natural laboratory.

## Thermochronology and sensitivity analysis

Thermochronological dates are the product of a thermal history and a radiation-damage
model, and both carry real uncertainty. I conducted Global Sensitivity Analysis (GSA) to
quantify the sensitivity of thermochronological dates to uncertain thermal history paths
and radiation damage model parameters.

That interest now runs the other direction as well. I've contributed to
[GDTchron](https://github.com/dyvasey/gdtchron), a Python package for using the outputs of
geodynamic models to predict thermochronometric ages. Earlier work coupled Raman
spectroscopy and zircon (U-Th)/He dating to improve interpretation of thermal histories
and crustal processes in the Kaapvaal Craton.

## Computational and open-science work

A recurring thread is that the modeling tools themselves need work. I contribute to
[ASPECT](https://aspect.geodynamics.org/), the community finite-element code for mantle
convection, and I'm interested in automatic differentiation as a route to tractable
adjoint-based inversion for geodynamic problems.

Throughout, I develop models to analyze fluid flow and chemical reactions, integrating
publicly available data to ensure reproducibility and accessibility.
