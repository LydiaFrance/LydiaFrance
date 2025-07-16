---
layout: page
title: Morphing Flight - Hidden Patterns
description: Discovering the fundamental patterns behind complex wing morphing
importance: 2
category: work
permalink: /projects/morphing-wings/page2/
---

We measured millions of feather positions around five Harris hawks in flight. In our flight hall, the hawks were recorded during taking off, flapping, gliding, turning, obstacle avoiding, and landing. Two thousand flights were recorded, at around 200 frames per second. 

## Diversity of Motion

Each dot in the point cloud below is a real marker position from a feather on the hawk (Toothless). We overlaid hundreds of flights to see how the wings and tails move in flight. Every marker position is shown here centred around the middle of the hawk, with any whole body rotations removed. The dark areas show where the feather markers most frequently appear. The arcs show the curving path of the wings during flapping. 

<div class="row justify-content-center mt-3 mb-4">
    <div class="col-md-6">
        <video autoplay loop muted playsinline class="img-fluid rounded z-depth-1">
            <source src="{{ '/assets/img/bird_gifs/media6.mp4' | relative_url }}" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        <div class="caption">
            Point cloud visualization of feather marker positions from hundreds of flights.
        </div>
    </div>
    <div class="col-md-6 d-flex flex-column justify-content-center">
        <img src="{{ '/assets/img/publication_preview/takeoff_preview.gif' | relative_url }}" 
             title="We recorded the movement of feather markers around the centre of the hawks." 
             class="img-fluid rounded z-depth-1" 
             alt="We recorded the movement of feather markers around the centre of the hawks.">
        <div class="caption">
            We recorded the movement of feather markers around the centre of the hawks.
        </div>
    </div>
</div>


## Extracting Patterns

With this huge dataset of natural flight behaviours, we asked the data **"What are the most important shape changes during flight?** We made no predefined assumptions, instead finding the dominant patterns in the spatial relationships between the markers. 


Most biomechanics and bird flight analysis track joint angles. Instead we treat the bird as a shape and analyse it as a whole. This is a different way of thinking about natural motion, and can be used with other animals. 


## Breaking Down Complexity

The hawks' morphing flight can be thought as a series of modes, or building blocks, that combine together. Separately, these shape change patterns help us see what is underneath bigger movements of the wings that would otherwise be hard to see. The most important shape changes are those critical in flapping, wing <span style="color: #7BBE23; font-weight: bold;">lifting and lowering</span> and <span style="color: #2FB177; font-weight: bold;">spreading and folding</span>. 


<div class="row justify-content-center mt-4 mb-4">
    <div class="col-md-5 col-sm-6">
        <img src="{{ '/assets/img/bird_gifs/PCs/PC01.gif' | relative_url }}" 
             title="First principal component of wing motion" 
             class="img-fluid rounded z-depth-1" 
             alt="PC01 wing motion pattern">
        <div class="caption text-center">
            <small>First mode - lifting wings</small>
        </div>
    </div>
    <div class="col-md-5 col-sm-6">
        <img src="{{ '/assets/img/bird_gifs/PCs/PC02.gif' | relative_url }}" 
             title="Second principal component of wing motion" 
             class="img-fluid rounded z-depth-1" 
             alt="PC02 wing motion pattern">
        <div class="caption text-center">
            <small>Second mode - spreading wings</small>
        </div>
    </div>
</div>

Each shape change mode is mathematically simple for comparison across behaviours, individuals, and even species. 

These are the first two, we have found **nine morphing shape modes** which together account for over 99.9% of morphing flight in the hawks. 

## Why This Matters

- **Birds aren't randomly flapping** - they're following predictable patterns
- **Complex flight can be understood** through simple mathematical principles  
- **We can potentially replicate** these patterns in artificial flight systems
- **Nature has already solved** the optimisation problem we're struggling with in aviation

**Read on to interact with all the shape change modes.**


<!-- Navigation -->
<div class="d-flex justify-content-between mt-5">
    <a href="{{ '/projects/morphing-wings/index/' | relative_url }}" class="btn btn-outline-primary">
        ← Previous: The Problem
    </a>
    <a href="{{ '/projects/morphing-wings/page3.html' | relative_url }}" class="btn btn-primary">
        Next: Interactive Analysis →
    </a>
</div> 