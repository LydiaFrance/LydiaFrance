---
layout: page
title: Testing the Modes on Other Birds
description: A proof of concept for comparing bird movement across species with different wing and tail shapes.
importance: 6
category: work
permalink: /projects/morphing-wings/page6/
---

Different bird species have long pointed handwings, broad arm wings, large tails, or very small tails. That makes a simple question surprisingly hard to answer: **how differently do different species move their wings and tails in flight?**

If we compare raw marker positions directly, body shape and movement get mixed together. A goose and a hawk can differ because they move differently, but also because their wings and tails have different proportions in the first place.

If we instead describe flight as shape changes, we can bring very different species into the same movement space. The morphing shape modes give us those shared movements: lifting the wings, spreading them, sweeping them, and changing the tail.

<div class="row mt-4 mb-4 align-items-start">
    <div class="col-md-4 mb-3">
        <div class="cross-species-panel">
            <span class="panel-kicker">large handwing</span>
            <img src="{{ '/assets/img/morphing-wings/cross-species/black-swift-vs-hawk.png' | relative_url }}"
                 class="img-fluid rounded z-depth-1"
                 alt="Black swift preserved specimen landmarks compared with the Harris' hawk reference shape">
            <div class="caption text-center">
                Black swift compared with the hawk reference shape.
            </div>
        </div>
    </div>
    <div class="col-md-4 mb-3">
        <div class="cross-species-panel">
            <span class="panel-kicker">very long tail</span>
            <img src="{{ '/assets/img/morphing-wings/cross-species/sharp-shinned-hawk-vs-hawk.png' | relative_url }}"
                 class="img-fluid rounded z-depth-1"
                 alt="Sharp-shinned hawk preserved specimen landmarks compared with the Harris' hawk reference shape">
            <div class="caption text-center">
                Sharp-shinned hawk compared with the hawk reference shape.
            </div>
        </div>
    </div>
    <div class="col-md-4 mb-3">
        <div class="cross-species-panel">
            <span class="panel-kicker">large wingspan</span>
            <img src="{{ '/assets/img/morphing-wings/cross-species/canada-goose-vs-hawk.png' | relative_url }}"
                 class="img-fluid rounded z-depth-1"
                 alt="Canada goose preserved specimen landmarks compared with the Harris' hawk reference shape">
            <div class="caption text-center">
                Canada goose compared with the hawk reference shape.
            </div>
        </div>
    </div>
</div>

## A First Test

For this proof of concept, we did **not** have movement data from other species. Instead, we used measurements from preserved bird specimens. These give us key body landmarks: wing tip, wrist, shoulders, tail base, tail tip, and head.

Those landmarks let us make a first, cautious visual test: what would the hawk movement modes look like on birds with different wing and tail proportions?

## Flying Like a Hawk

The animations below start with the real Harris' hawk movement. The three examples then show that same movement pattern mapped onto different species shapes. They are deliberately shown as a test, not as a claim about how these species truly fly.

<div class="row justify-content-center mt-4 mb-4">
    <div class="col-md-4 mb-3">
        <div class="caption text-center">
            Real Harris' hawk flight.
        </div>
        <img src="{{ '/assets/img/morphing-wings/cross-species/harris-hawk-reference-flight.gif' | relative_url }}"
             class="img-fluid rounded z-depth-1 species-gif"
             alt="Harris' hawk reference flight shape changes">
    </div>
</div>

<div class="row mt-4 mb-4">
    <div class="col-md-4 mb-3">
        <img src="{{ '/assets/img/morphing-wings/cross-species/black-swift-hawk-flight.gif' | relative_url }}"
             class="img-fluid rounded z-depth-1 species-gif"
             alt="Projected hawk flight shape changes on a black swift body shape">
        <div class="caption text-center">
            A shape where the handwing makes up a high proportion of the wing.
        </div>
    </div>
    <div class="col-md-4 mb-3">
        <img src="{{ '/assets/img/morphing-wings/cross-species/sharp-shinned-hawk-flight.gif' | relative_url }}"
             class="img-fluid rounded z-depth-1 species-gif"
             alt="Projected hawk flight shape changes on a sharp-shinned hawk body shape">
        <div class="caption text-center">
            A hawk-like body plan where the tail appears especially long.
        </div>
    </div>
    <div class="col-md-4 mb-3">
        <img src="{{ '/assets/img/morphing-wings/cross-species/canada-goose-hawk-flight.gif' | relative_url }}"
             class="img-fluid rounded z-depth-1 species-gif"
             alt="Projected hawk flight shape changes on a Canada goose body shape">
        <div class="caption text-center">
            A large-wingspan shape with a comparatively narrow tail. The wing twist appears stronger, which may be because the larger arm wing, relative to the handwing, changes how the hawk movement pattern is expressed on the goose-shaped wing.
        </div>
    </div>
</div>

## What We See

The transformed movements still look organised. The wings lift, spread, and sweep in recognisable ways even when the body shape is very different from a Harris' hawk.

That suggests the morphing modes could act as a shared coordinate system: a way to compare wing and tail shape changes across species without starting from scratch each time.

But this is not a substitute for real flight data. These animations show each species shape being asked to "fly like a hawk". A black swift, sharp-shinned hawk, or Canada goose would not actually use exactly these movements in life. The odd-looking parts are informative too: they show where the hawk pattern does not fit another body plan neatly.

## How It Works

Think of the hawk modes as building blocks of movement. The specimen measurements give us matching landmark positions, which we use to estimate how those building blocks would resize and rotate on a different body.

The method adjusts each landmark separately. For example, the hawk wing tip is transformed to the wing-tip position of the new species, while the wrist, shoulder, and tail points are transformed to their own matching locations. The result is a species-shaped version of the same underlying movement pattern.

This is useful because it keeps the comparison fair. We are not asking every bird to be hawk-sized. We are asking how the same morphing pattern changes when it is placed onto a different anatomy.

<div class="takeaway-box mt-4 mb-4">
    <h2>Takeaway</h2>
    <p>
        The specimen work is a cautious first test. It shows that hawk morphing modes can be mapped onto other species in a way that is visually and biologically plausible enough to justify the next step: testing the same idea with real flight data from more birds.
    </p>
</div>

## Source

This prototype is based on the cross-species generalisation notebook in the kinematic morphospace project, using specimen measurements from Harvey et al. (2022).

<!-- Progress Navigator -->
<div class="progress-navigator-container mt-5">
    <div class="progress-navigator-bar">
        <div class="step" data-page="index">
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
        <div class="step active" data-page="page6">
            <div class="step-number">6</div>
            <div class="step-title">Other Species</div>
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
    max-width: 900px;
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
    padding: 0 8px;
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
    font-size: 0.75rem;
    text-align: center;
    color: #6c757d;
    font-weight: 500;
    transition: color 0.3s ease;
    max-width: 92px;
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

.cross-species-panel {
    height: 100%;
}

.panel-kicker {
    display: block;
    margin-bottom: 0.5rem;
    color: #6f42c1;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.06em;
    text-transform: uppercase;
}

.species-gif {
    border: 2px solid #e9ecef;
    background: #ffffff;
}

.takeaway-box {
    border-left: 4px solid #6f42c1;
    background: #f8f9fa;
    border-radius: 8px;
    padding: 1.25rem 1.5rem;
}

.takeaway-box h2 {
    color: #6f42c1;
    font-size: 1.25rem;
    margin-bottom: 0.75rem;
}

@media (max-width: 767px) {
    .progress-navigator-bar {
        align-items: flex-start;
        gap: 0.5rem;
        overflow-x: auto;
        padding-bottom: 0.75rem;
    }

    .progress-navigator-bar::before {
        display: none;
    }

    .step {
        min-width: 82px;
    }
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
