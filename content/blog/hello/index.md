---
title: "Starting a notebook in public"
date: 2026-08-03
draft: false
tags: ["meta", "geodynamics"]
summary: "Why I'm keeping research notes in public, and what I plan to put here."
---

A lot of what I learn doing computational geoscience never makes it into a paper. The
paper gets the result. It does not get the two weeks spent working out why the solver
stalled, or the specific incantation that made a build work on a Mac, or the sensitivity
test that quietly ruled out an entire hypothesis.

That material is genuinely useful — mostly to the version of me who hits the same wall in
eighteen months, but also to anyone else running these codes. So I'm going to write some
of it down here.

Rough plan for what lands on this page:

- **Geodynamic modeling.** Notes from working with [ASPECT](https://aspect.geodynamics.org/)
  and other finite-element codes — setup, solver behavior, and the gap between what a
  benchmark tests and what your actual problem needs.
- **Numerical methods.** Adjoints, automatic differentiation, and inverse methods, with
  an eye toward making inversion tractable for problems that are currently too expensive.
- **Reproducibility.** Getting scientific software to build, run, and give the same answer
  twice — on someone else's machine.
- **Occasional field notes.** The rocks are why any of this matters.

Posts here are working notes, not peer-reviewed results. I'll try to be clear about which
claims are solid and which are me thinking out loud.

If something here is wrong or you want to talk about it, I'm at
[ryankstoner@gmail.com](mailto:ryankstoner@gmail.com).
