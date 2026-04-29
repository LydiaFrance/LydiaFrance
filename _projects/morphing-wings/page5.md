---
layout: page
title: Make Morphing Flight Simpler
description: See how reducing dimensions affects our understanding of bird flight patterns
importance: 5
category: work
permalink: /projects/morphing-wings/page5/
---

Bird flight involves many _degrees of freedom_ - which means multiple joints with multiple muscles and many possible configurations.

We can rebuild full morphing flight with different numbers of morphing shape modes. This is known as **dimension reduction**.

## Dimension Reduction

Here is a real flight by Toothless as recorded by motion capture. We can use the morphing shape modes to simplify the flight. You can see which morphing shape modes are used for each example.

Toggle the animation with or without the original data underneath (in grey). Hover over the morphing shape modes to see their effect.

---

<div class="row mt-4">
    <div class="col-md-12">
        <!-- Button layout: comparison buttons on left, dimension selector on right -->
        <div class="text-center mb-4">
            <div class="d-flex justify-content-center align-items-center">
                <!-- Comparison toggle button on the left -->
                <div class="me-4">
                    <button type="button" class="btn btn-comparison active" id="compare-toggle">VS ORIGINAL</button>
                </div>
                
                <!-- Dimension selector buttons on the right -->
                <div class="btn-group" role="group" aria-label="Dimension selector">
                    <button type="button" class="btn" data-dims="full">Original</button>
                    <button type="button" class="btn" data-dims="9">9 Modes</button>
                    <button type="button" class="btn" data-dims="4">4 Modes</button>
                    <button type="button" class="btn active" data-dims="2">2 Modes</button>
                    <button type="button" class="btn" data-dims="1">1 Mode</button>
                </div>
            </div>
        </div>
        
        <!-- GIF display area -->
        <div class="row">
            <!-- Main dimensional reduction gif -->
            <div class="col-md-7">
                <div class="gif-container text-center" style="min-height: 400px;">
                    <img id="dimensional-gif" 
                         src="{{ '/assets/img/bird_gifs/right_turn_2dims_compare.gif' | relative_url }}" 
                         class="img-fluid rounded z-depth-1" 
                         style="max-height: 500px;"
                         alt="Bird flight dimensional reduction">
                </div>
            </div>
            
                        <!-- Contributing PC modes -->
            <div class="col-md-5 d-flex flex-column">
                <div id="pc-modes-container">
                    <div class="text-center mb-2">
                        <h6 class="mb-2" style="color: #6f42c1; font-weight: 500; font-size: 0.9rem;">Contributing Modes</h6>
                    </div>
                    <div id="pc-modes-grid">
                        <!-- PC gifs will be dynamically added here -->
                    </div>
                    <!-- Hover description text -->
                    <div id="pc-description" class="text-center mt-2" style="opacity: 0; transition: opacity 0.3s ease; height: 20px;">
                        <span style="font-size: 0.8rem; color: #6c757d; font-weight: 600;"></span>
                    </div>
                </div>
                
                <!-- Percentage accuracy display -->
                <div class="mt-auto">
                    <div class="text-center p-3" style="background-color: #f8f9fa; border-radius: 10px; border: 1px solid #e9ecef;">
                        <h6 class="mb-2" style="color: #6f42c1; font-weight: 500; font-size: 0.9rem;">Accuracy to Original</h6>
                        <div class="d-flex justify-content-center align-items-center mb-2">
                            <span id="accuracy-percentage" style="font-size: 1.8rem; font-weight: 600; color: #6f42c1;">92%</span>
                            <span style="font-size: 0.9rem; color: #6c757d; margin-left: 8px;">captured</span>
                        </div>
                        <div class="progress mb-2" style="height: 12px; border-radius: 8px;">
                            <div id="accuracy-bar" class="progress-bar" 
                                 style="width: 92%; background-color: #6f42c1; border-radius: 8px; transition: width 0.5s ease;" 
                                 role="progressbar" aria-valuenow="92" aria-valuemin="0" aria-valuemax="100">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
 
    </div>
</div>

---

## Subtle Shape Changes

With fewer modes, the representation drifts away from the original. Even with 4 modes, 96% of the original, the tail is not well represented.

Morphing flight has very subtle elements and the hawks need more modes for manoeuvres.

**Read on to see an early test of whether these hawk modes can be mapped onto other bird body shapes.**

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
        <div class="step active" data-page="page5">
            <div class="step-number">5</div>
            <div class="step-title">Simplified Flight</div>
        </div>
        <div class="step" data-page="page6">
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

.btn-group .btn {
    margin: 0 8px;
    border-color: #6f42c1;
    color: #6f42c1;
    background-color: transparent;
}

.btn-group .btn:hover {
    background-color: #6f42c1;
    border-color: #6f42c1;
    color: white;
}

.btn-group .btn.active {
    background-color: #6f42c1;
    border-color: #6f42c1;
    color: white;
}

/* Comparison toggle styling */
.btn-comparison {
    border-color: #6f42c1 !important;
    color: #6f42c1 !important;
    background-color: transparent !important;
}

.btn-comparison:hover {
    background-color: #6f42c1 !important;
    border-color: #6f42c1 !important;
    color: white !important;
}

.btn-comparison.active {
    background-color: #6f42c1 !important;
    border-color: #6f42c1 !important;
    color: white !important;
}

.gif-container {
    transition: all 0.3s ease;
}

#dimensional-gif {
    transition: opacity 0.3s ease;
    border: 2px solid #e9ecef;
    border-radius: 10px;
}



/* PC Mode gif sizing and grid layouts */
.pc-grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
    width: 100%;
    justify-items: center;
}

.pc-grid-4 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    gap: 12px;
    width: 100%;
    justify-items: center;
}

.pc-grid-9 {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    gap: 10px;
    width: 100%;
    justify-items: center;
}

.pc-large, .pc-medium, .pc-small {
    width: 100px;
    height: auto;
    max-width: 100%;
    cursor: pointer;
    transition: transform 0.2s ease;
}

.pc-large:hover, .pc-medium:hover, .pc-small:hover {
    transform: scale(1.05);
}

#pc-modes-container {
    background-color: white;
    border-radius: 10px;
    padding: 15px;
    border: 2px solid #e9ecef;
}

#pc-modes-grid {
    align-content: flex-start;
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

    const buttons = document.querySelectorAll('[data-dims]');
    const gif = document.getElementById('dimensional-gif');
    
    // Define base paths outside functions to ensure Jekyll processes them
    const birdGifsPath = '{{ "/assets/img/bird_gifs/" | relative_url }}';
    const pcGifsPath = '{{ "/assets/img/bird_gifs/PCs_plain/" | relative_url }}';
    
    const dimensionData = {
        'full': {
            gif: 'right_turn_fulldims.gif',
            compare: 'right_turn_fulldims.gif', // Same for original
            pcs: [], // No individual PCs for original
            percentage: 100
        },
        '9': {
            gif: 'right_turn_9dims.gif',
            compare: 'right_turn_9dims_compare.gif',
            pcs: ['PC01_cropped', 'PC02_cropped', 'PC03_cropped', 'PC04_cropped', 'PC05_cropped', 'PC06_cropped', 'PC07_cropped', 'PC08_cropped', 'PC09_cropped'],
            percentage: 99
        },
        '4': {
            gif: 'right_turn_4dims.gif',
            compare: 'right_turn_4dims_compare.gif',
            pcs: ['PC01_cropped', 'PC02_cropped', 'PC03_cropped', 'PC04_cropped'],
            percentage: 96
        },
        '2': {
            gif: 'right_turn_2dims.gif',
            compare: 'right_turn_2dims_compare.gif',
            pcs: ['PC01_cropped', 'PC02_cropped'],
            percentage: 92
        },
        '1': {
            gif: 'right_turn_1dims.gif',
            compare: 'right_turn_1dims_compare.gif',
            pcs: ['PC01_cropped'],
            percentage: 66
        }
    };
    
    // PC mode descriptions
    const pcDescriptions = {
        'PC01_cropped': '(1) Wing lifting',
        'PC02_cropped': '(2) Wing folding',
        'PC03_cropped': '(3) Tail spreading',
        'PC04_cropped': '(4) Body pitch',
        'PC05_cropped': '(5) Wing sweeping',
        'PC06_cropped': '(6) Tail twisting',
        'PC07_cropped': '(7) Wing extension',
        'PC08_cropped': '(8) Body roll',
        'PC09_cropped': '(9) Fine tail control'
    };
    
    // Track current state
    let currentDims = '2';
    let showComparison = true;
    
    function updateMainGif() {
        const data = dimensionData[currentDims];
        const gifToShow = showComparison ? data.compare : data.gif;
        
        gif.style.opacity = '0.3';
        setTimeout(() => {
            gif.src = birdGifsPath + gifToShow;
            gif.style.opacity = '1';
        }, 150);
    }
    
    function updateAccuracyDisplay() {
        const data = dimensionData[currentDims];
        const percentageElement = document.getElementById('accuracy-percentage');
        const barElement = document.getElementById('accuracy-bar');
        
        // Update percentage text
        percentageElement.textContent = data.percentage + '%';
        
        // Update progress bar
        barElement.style.width = data.percentage + '%';
        barElement.setAttribute('aria-valuenow', data.percentage);
    }
    
    function updatePCModes(pcs) {
        const container = document.getElementById('pc-modes-grid');
        const pcModesContainer = document.getElementById('pc-modes-container');
        container.innerHTML = '';
        
        console.log('Updating PC modes with:', pcs); // Debug log
        
        if (pcs.length === 0) {
            container.className = 'd-flex flex-wrap justify-content-center align-items-start';
            pcModesContainer.style.visibility = 'hidden'; // Hide but keep space
            return; // Just show empty container for original
        } else {
            pcModesContainer.style.visibility = 'visible'; // Show for other modes
        }
        
        // Determine grid layout and size based on number of PCs
        let gridClass = '';
        let sizeClass = '';
        if (pcs.length <= 2) {
            gridClass = 'pc-grid-2';
            sizeClass = 'pc-large';
        } else if (pcs.length <= 4) {
            gridClass = 'pc-grid-4';
            sizeClass = 'pc-medium';
        } else {
            gridClass = 'pc-grid-9';
            sizeClass = 'pc-small';
        }
        
        // Set the grid class on the container
        container.className = gridClass;
        
        pcs.forEach(pc => {
            const pcImg = document.createElement('img');
            
            // Use static PNG by default
            const staticSrc = pcGifsPath + pc.replace('_cropped', '_static') + '.png';
            const animatedSrc = pcGifsPath + pc + '.gif';
            
            pcImg.src = staticSrc;
            pcImg.className = `${sizeClass} rounded`;
            pcImg.alt = `${pc} morphing pattern`;
            // pcImg.title = `${pc} morphing pattern - hover to animate`;
            
            // Store both src paths for hover functionality
            pcImg.dataset.staticSrc = staticSrc;
            pcImg.dataset.animatedSrc = animatedSrc;
            
            const descriptionElement = document.getElementById('pc-description');
            const descriptionSpan = descriptionElement.querySelector('span');
            
            // Add hover functionality to swap between static and animated, and show description
            pcImg.addEventListener('mouseenter', function() {
                this.src = this.dataset.animatedSrc;
                // Show description
                const description = pcDescriptions[pc] || '';
                descriptionSpan.textContent = description;
                descriptionElement.style.opacity = '1';
            });
            
            pcImg.addEventListener('mouseleave', function() {
                this.src = this.dataset.staticSrc;
                // Hide description
                descriptionElement.style.opacity = '0';
            });
            
            console.log('Creating PC image with static src:', pcImg.src); // Debug log
            
            const pcContainer = document.createElement('div');
            pcContainer.className = 'text-center';
            pcContainer.appendChild(pcImg);
            
            container.appendChild(pcContainer);
        });
    }
    
    buttons.forEach(button => {
        button.addEventListener('click', function() {
            // Update active button
            buttons.forEach(btn => btn.classList.remove('active'));
            this.classList.add('active');
            
            // Get dimension data
            currentDims = this.dataset.dims;
            const data = dimensionData[currentDims];
            
            console.log('Button clicked:', currentDims, data); // Debug log
            
            // Update GIF, PC modes, and accuracy display
            updateMainGif();
            updatePCModes(data.pcs);
            updateAccuracyDisplay();
        });
    });
    
    // Handle comparison toggle - single button that toggles on/off
    const compareToggle = document.getElementById('compare-toggle');
    
    compareToggle.addEventListener('click', function() {
        showComparison = !showComparison;
        if (showComparison) {
            this.classList.add('active');
        } else {
            this.classList.remove('active');
        }
        updateMainGif();
    });
    
    // Initialize with 2 modes view and comparison on
    updatePCModes(dimensionData['2'].pcs);
    updateAccuracyDisplay();
    updateMainGif(); // Ensure the gif matches the initial comparison state
});
</script>
