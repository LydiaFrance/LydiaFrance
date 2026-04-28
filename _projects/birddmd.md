---
layout: page
title: BirdDMD
description: Dynamic Mode Decomposition tools for modelling bird flight.
img: assets/img/publication_preview/dmd_figure1.png
importance: 2
category: work
related_publications: false
permalink: /projects/birddmd/
---

BirdDMD is a Python toolkit for analysing bird flight motion-capture data with Dynamic Mode Decomposition. It supports preprocessing, mode fitting, reconstruction, forecasting, and visualisation workflows for the DMD hawk-flight preprint.

<div class="row justify-content-center">
  <div class="col-md-10 mt-3">
    <img src="{{ '/assets/img/publication_preview/dmd_figure1.png' | relative_url }}" class="img-fluid rounded z-depth-1" alt="Dynamic Mode Decomposition schematic for hawk flight analysis">
    <div class="caption">
      Dynamic Mode Decomposition applied to hawk motion-capture data.
    </div>
  </div>
</div>

The package is designed around reusable DMD utilities and hawk-specific convenience functions, with notebook examples for flapping modes, full-flight reconstruction, turning, and generative forecasting.

<div class="birddmd-links mt-4">
  <a href="https://arxiv.org/abs/2602.19196" class="birddmd-link" role="button">Preprint</a>
  <a href="https://github.com/LydiaFrance/BirdDMD" class="birddmd-link" role="button">Code</a>
  <a href="https://lydiafrance.github.io/BirdDMD/" class="birddmd-link" role="button">Website</a>
</div>

<style>
  .birddmd-links {
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
  }

  .birddmd-link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    min-width: 9rem;
    padding: 0.72rem 1.1rem;
    border: 1px solid var(--global-theme-color);
    border-radius: 6px;
    color: var(--global-theme-color);
    font-weight: 600;
    text-decoration: none;
  }

  .birddmd-link:hover {
    background: var(--global-theme-color);
    color: var(--global-hover-text-color);
    text-decoration: none;
  }
</style>
