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

<!-- Progress Navigator -->
<div class="progress-navigator-container mt-5">
    <div class="progress-navigator-bar">
        <div class="step" data-page="index">
            <div class="step-number">1</div>
            <div class="step-title">The Problem</div>
        </div>
        <div class="step active" data-page="page2">
            <div class="step-number">2</div>
            <div class="step-title">Hidden Patterns</div>
        </div>
        <div class="step" data-page="page3">
            <div class="step-number">3</div>
            <div class="step-title">Interactive Modes</div>
        </div>
        <div class="step" data-page="page4">
            <div class="step-number">4</div>
            <div class="step-title">Obstacle Avoidance</div>
        </div>
        <div class="step" data-page="page5">
            <div class="step-number">5</div>
            <div class="step-title">Simplified Flight</div>
        </div>
    </div>
</div>

<style>
.progress-navigator-container {
    margin-top: 3rem;
    margin-bottom: 2rem;
}

.progress-navigator-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    margin: 0 auto;
    max-width: 800px;
}

.progress-navigator-bar::before {
    content: '';
    position: absolute;
    top: 20px;
    left: 0;
    right: 0;
    height: 2px;
    background-color: #e9ecef;
    z-index: 1;
}

.step {
    display: flex;
    flex-direction: column;
    align-items: center;
    cursor: pointer;
    text-decoration: none;
    color: inherit;
    z-index: 2;
    position: relative;
    background: white;
    padding: 0 10px;
}

.step-number {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: #e9ecef;
    color: #6c757d;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 600;
    font-size: 0.9rem;
    margin-bottom: 8px;
    transition: all 0.3s ease;
}

.step-title {
    font-size: 0.8rem;
    text-align: center;
    color: #6c757d;
    font-weight: 500;
    transition: color 0.3s ease;
}

.step.active .step-number {
    background-color: #6f42c1;
    color: white;
}

.step.active .step-title {
    color: #6f42c1;
    font-weight: 600;
}

.step:hover .step-number {
    background-color: #6f42c1;
    color: white;
    transform: scale(1.1);
}

.step:hover .step-title {
    color: #6f42c1;
}
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
    const steps = document.querySelectorAll('.step');
    
    steps.forEach(step => {
        step.addEventListener('click', function() {
            const page = this.dataset.page;
            const baseUrl = '{{ "/projects/morphing-wings/" | relative_url }}';
            
            if (page === 'index') {
                window.location.href = baseUrl;
            } else if (page === 'page3') {
                window.location.href = baseUrl + 'page3.html';
            } else {
                window.location.href = baseUrl + page + '/';
            }
        });
    });
});
</script> 