---
layout: page
title: BirdDMD
description: Dynamic Mode Decomposition tools for modelling bird flight.
img: assets/img/publication_preview/dmd_figure1.png
importance: 2
category: work
related_publications: true
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

<div class="links mt-3">
  <a href="https://arxiv.org/abs/2602.19196" class="btn btn-sm z-depth-0" role="button">Preprint</a>
  <a href="https://github.com/LydiaFrance/BirdDMD" class="btn btn-sm z-depth-0" role="button">Code</a>
  <a href="https://lydiafrance.github.io/BirdDMD/" class="btn btn-sm z-depth-0" role="button">Documentation</a>
</div>
