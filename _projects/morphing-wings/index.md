---
layout: page
title: Shape Changing Wings in Flight
description: Birds achieve extraordinary flight performance through continuous wing shape changes.
img: assets/img/publication_preview/morphing_preview.gif
importance: 1
category: work
related_publications: false
permalink: /projects/morphing-wings/
---

## Morphing Flight

In this slowed down video, the hawk uses many adjustments to her wings and tail to dodge the obstacle. Bending, flexing, folding and unfolding, these shape changes are called **morphing flight**.

<div class="row justify-content-center">
    <div class="col-md-8 mt-3">
        <img src="{{ '/assets/img/publication_preview/morphing_preview.gif' | relative_url }}" 
             title="Harris' hawk morphing her wings during flight" 
             class="img-fluid rounded z-depth-1" 
             alt="Hawk continuously changing wing shape during flight">
        <div class="caption">
            A Harris' hawk continuously reshapes her wings and tail during flight, achieving manoeuvres no aircraft can match.
        </div>
    </div>
</div>

## Adaptive, Reactive

Morphing flight gives birds extraordinary control. By adjusting their **shape** as they fly, birds precisely change their stability, lift, and drag continuously. Birds have evolved to fly through dense forest branches, execute sharp turns that no fighter jet can manage, and land on a perch no wider than your thumb. Meanwhile, our aircraft need long runways, can't handle sudden wind gusts, and can't stop in midair.

## Mystery of Shape-Shifting Flight

We still don't understand how morphing flight is controlled. We would like to learn from birds: how they control such super-manoeuvrability. Which **shape changes** are critical in flight? How do birds control so many coordinated movements all at once? It is no easy task, even recording wings in flight accurately is difficult as bird flight is high speed.

<div class="row mt-4">
    <div class="col-md-6">
        <h3>Traditional Aircraft</h3>
        <ul>
            <li>Fixed wing shapes</li>
            <li>Simple control surfaces</li>
            <li>Limited manoeuvrability</li>
            <li>Struggle with turbulence</li>
        </ul>
    </div>
    <div class="col-md-6">
        <h3>Birds</h3>
        <ul>
            <li>Continuously changing wing shapes</li>
            <li>Flexible control surfaces</li>
            <li>Extraordinary manoeuvrability</li>
            <li>Thrive in complex wind conditions</li>
        </ul>
    </div>
</div>

## High Speed Motion Capture

To uncover how morphing flight works, we filmed 5 Harris' hawks in a specially built motion capture lab. Twenty cameras recorded tiny markers on the feathers in a large flight hall. We gave the hawks perches to land on and obstacles to navigate. Looking at 2000 flights, we looked into the shape changes critical to bird flight.

<div class="row justify-content-center">
    <div class="col-md-10 mt-3">
        <img src="{{ '/assets/img/project_images/project_1_mocap.svg' | relative_url }}" 
             title="Motion capture setup and data" 
             class="img-fluid rounded z-depth-1" 
             alt="Motion capture flight hall setup showing camera positions and flight data">
        <div class="caption">
            Our motion capture flight hall setup with multiple camera angles recording markers worn by the hawks.
        </div>
    </div>
</div>

**Read on about the hidden patterns of bird flight.**

<!-- Progress Navigator -->
<div class="progress-navigator-container mt-5">
    <div class="progress-navigator-bar">
        <div class="step active" data-page="index">
            <div class="step-number">1</div>
            <div class="step-title">Morphing Flight</div>
        </div>
        <div class="step" data-page="page2">
            <div class="step-number">2</div>
            <div class="step-title">Hidden Patterns</div>
        </div>
        <div class="step" data-page="page3">
            <div class="step-number">3</div>
            <div class="step-title">Shape Change Modes</div>
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
