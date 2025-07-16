---
layout: page
title: Explore Obstacle Avoidance
description: Interact with the data to see how different wing morphing patterns are used in flights with an obstacle.
importance: 4
category: work
permalink: /projects/morphing-wings/page4/
---

The following heatmap shows how Toothless flew between two perches with and without an obstacle. Each row shows a different morphing shape mode, with the colours showing <span style="color: #dc3545; font-weight: bold;">positive</span> and <span style="color: #3682BA; font-weight: bold;">negative</span> scores. Scores are the binned averages from 30 flights with an obstacle and 67 without.   

Try hovering your mouse over the heatmap, move from left to right as the hawk approaches the obstacle and lands. The gif will show you the morphing shape changes shown by each row. You can directly compare flights with an obstacle (top of each row) to flights without an obstacle (underneath).
 

*Note, the animations are symmetrical, but not all shape changes in flight are the same on the left and right sides of the hawk.*

---

<div class="row mt-4">
    <div class="col-md-8">
        <div class="interactive-heatmap-container" style="position: relative;">
            <img src="{{ '/assets/img/project_images/heatmap.svg' | relative_url }}" 
                 class="img-fluid main-heatmap" 
                 alt="Heatmap showing usage of different morphing modes">
            
            <!-- Hover zones for each row -->
            <div class="hover-zone zone-1" data-gif="PC01.gif" style="position: absolute; top: 7.9%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-2" data-gif="PC02.gif" style="position: absolute; top: 17.4%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-3" data-gif="PC03.gif" style="position: absolute; top: 26.8%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-4" data-gif="PC04.gif" style="position: absolute; top: 36.2%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-5" data-gif="PC05.gif" style="position: absolute; top: 46.0%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-6" data-gif="PC08.gif" style="position: absolute; top: 56.0%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-7" data-gif="PC06.gif" style="position: absolute; top: 65%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-8" data-gif="PC07.gif" style="position: absolute; top: 74%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            <div class="hover-zone zone-9" data-gif="PC09.gif" style="position: absolute; top: 84%; left: 0%; width: 100%; height: 8.2%; cursor: pointer;"></div>
            
            <!-- Contextual hover zones -->
            <div class="context-zone" data-gif="PC01.gif" data-context="approach1" style="position: absolute; top: 7.9%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC02.gif" data-context="approach2" style="position: absolute; top: 17.4%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC03.gif" data-context="approach3" style="position: absolute; top: 26.8%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC04.gif" data-context="approach4" style="position: absolute; top: 36.2%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC05.gif" data-context="approach5" style="position: absolute; top: 46.0%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC08.gif" data-context="approach8" style="position: absolute; top: 56.0%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC06.gif" data-context="approach6" style="position: absolute; top: 65%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC07.gif" data-context="approach7" style="position: absolute; top: 74%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC09.gif" data-context="approach9" style="position: absolute; top: 84%; left: 10%; width: 40%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            
            <!-- At obstacle zones -->
            <div class="context-zone" data-gif="PC01.gif" data-context="atobstacle1" style="position: absolute; top: 7.9%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC02.gif" data-context="atobstacle2" style="position: absolute; top: 17.4%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC03.gif" data-context="atobstacle3" style="position: absolute; top: 26.8%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC04.gif" data-context="atobstacle4" style="position: absolute; top: 36.2%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC05.gif" data-context="atobstacle5" style="position: absolute; top: 46.0%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC08.gif" data-context="atobstacle8" style="position: absolute; top: 56.0%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC06.gif" data-context="atobstacle6" style="position: absolute; top: 65%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC07.gif" data-context="atobstacle7" style="position: absolute; top: 74%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC09.gif" data-context="atobstacle9" style="position: absolute; top: 84%; left: 50%; width: 10%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            
            <!-- After obstacle recovery zones -->
            <div class="context-zone" data-gif="PC01.gif" data-context="recovery1" style="position: absolute; top: 7.9%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC02.gif" data-context="recovery2" style="position: absolute; top: 17.4%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC03.gif" data-context="recovery3" style="position: absolute; top: 26.8%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC04.gif" data-context="recovery4" style="position: absolute; top: 36.2%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC05.gif" data-context="recovery5" style="position: absolute; top: 46.0%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC08.gif" data-context="recovery8" style="position: absolute; top: 56.0%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC06.gif" data-context="recovery6" style="position: absolute; top: 65%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC07.gif" data-context="recovery7" style="position: absolute; top: 74%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
            <div class="context-zone" data-gif="PC09.gif" data-context="recovery9" style="position: absolute; top: 84%; left: 60%; width: 30%; height: 8.2%; cursor: pointer; z-index: 10;"></div>
        </div>
    </div>
    
    <div class="col-md-4">
        <div class="gif-display-area" style="position: sticky; top: 120px;">
            <div id="gif-placeholder" class="text-center p-4" style="border: 2px dashed #ccc; border-radius: 10px; min-height: 200px; display: flex; align-items: center; justify-content: center;">
                <p class="text-muted">Hover over a row to see the wing morphing pattern</p>
            </div>
            <img id="active-gif" 
                 src="" 
                 class="img-fluid rounded z-depth-1" 
                 style="display: none;"
                 alt="Wing morphing pattern">
            <div id="gif-caption" class="caption text-center mt-2" style="display: none;">
                <small id="caption-text"></small>
            </div>
            
            <!-- New contextual text area -->
            <div id="context-text-area" class="mt-3 p-3" style="display: none; background-color: #f8f9fa; border-radius: 8px; border-left: 4px solid #007bff;">
                <div id="context-text" class="text-dark"></div>
            </div>
        </div>
    </div>
</div>

---

## Insights

By splitting the complexity of morphing flight into morphing shape modes it is far easier to see extremely subtle changes how the hawk flies. Usually in biomechanics we miss this detail. While nine morphing modes is a lot, this has lowered the *number of dimensions* for morphing flight considerably. 

The shape changes are combined together and don't exist in isolation. Also it's important to remember every hawk flies differently! 


- **Context-Dependent Control**: Different shape changes when accelerating, turning, gliding, and landing
- **Coordinated Patterns**: Multiple modes work together to achieve complex manoeuvers
- **Efficient Design**: Only a few fundamental patterns can generate the full range of bird flight behaviors

**Go to the next page to see how we can use the modes to simplify morphing flight.**

<!-- Progress Navigator -->
<div class="progress-navigator-container mt-5">
    <div class="progress-navigator-bar">
        <div class="step" data-page="index">
            <div class="step-number">1</div>
            <div class="step-title">The Problem</div>
        </div>
        <div class="step" data-page="page2">
            <div class="step-number">2</div>
            <div class="step-title">Hidden Patterns</div>
        </div>
        <div class="step" data-page="page3">
            <div class="step-number">3</div>
            <div class="step-title">Interactive Modes</div>
        </div>
        <div class="step active" data-page="page4">
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

.interactive-heatmap-container {
    transition: all 0.3s ease;
}

.hover-zone {
    transition: all 0.2s ease;
}

.hover-zone:hover {
    background-color: rgba(255, 255, 255, 0.0);
    border-left: 4px solid #007bff;
}

.context-zone {
    transition: all 0.2s ease;
}

#active-gif {
    transition: opacity 0.3s ease;
}

.gif-display-area {
    background: #f8f9fa;
    border-radius: 10px;
    padding: 15px;
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

    const hoverZones = document.querySelectorAll('.hover-zone');
    const contextZones = document.querySelectorAll('.context-zone');
    const activeGif = document.getElementById('active-gif');
    const placeholder = document.getElementById('gif-placeholder');
    const caption = document.getElementById('gif-caption');
    const captionText = document.getElementById('caption-text');
    const contextArea = document.getElementById('context-text-area');
    const contextText = document.getElementById('context-text');
    
    const modeNames = {
        'PC01.gif': '(1) Wing <span style="color: #dc3545; font-weight: bold;">lifting</span> & <span style="color: #3682BA; font-weight: bold;">lowering</span>',
        'PC02.gif': '(2) Wing <span style="color: #dc3545; font-weight: bold;">spreading</span> & <span style="color: #3682BA; font-weight: bold;">folding</span>', 
        'PC03.gif': '(3) Wing sweep <span style="color: #dc3545; font-weight: bold;">forwards</span> & <span style="color: #3682BA; font-weight: bold;">backwards</span>',
        'PC04.gif': '(4) Tail <span style="color: #dc3545; font-weight: bold;">spreading</span> & <span style="color: #3682BA; font-weight: bold;">contracting</span>',
        'PC05.gif': '(5) Leading edge and tail pitch <span style="color: #dc3545; font-weight: bold;">up</span> & <span style="color: #3682BA; font-weight: bold;">down</span>',
        'PC06.gif': '(6) Hand-wing <span style="color: #dc3545; font-weight: bold;">spreading</span> & <span style="color: #3682BA; font-weight: bold;">contracting</span>',
        'PC07.gif': '(7) <span style="color: #dc3545; font-weight: bold;">M-folding</span> & <span style="color: #3682BA; font-weight: bold;">W-folding</span>',
        'PC08.gif': '(8) Trailing edge and tail pitch <span style="color: #dc3545; font-weight: bold;">up</span> & <span style="color: #3682BA; font-weight: bold;">down</span>',
        'PC09.gif': '(9) Hand-wing sweep <span style="color: #dc3545; font-weight: bold;">forwards</span> & <span style="color: #3682BA; font-weight: bold;">backwards</span>'
    };
    
    const contextData = {
        'approach1': '<strong>Approaching the obstacle.</strong><br>Timing of wingbeats has changed. Wingtips are <span style="color: #dc3545; font-weight: bold;">raised higher</span> in the upstroke and <span style="color: #3682BA; font-weight: bold;">dropped lower</span> in the downstroke.',
        'approach2': '<strong>Approaching the obstacle.</strong><br>Wings more <span style="color: #dc3545; font-weight: bold;">spread</span> during flapping.',
        'approach3': '<strong>Approaching the obstacle.</strong><br>Swept <span style="color: #dc3545; font-weight: bold;">forwards</span> earlier in the wingbeat.',
        'approach4': '<strong>Approaching the obstacle.</strong><br>Tail <span style="color: #dc3545; font-weight: bold;">more spread</span> during flapping.',
        'approach5': '<strong>Approaching the obstacle.</strong><br>Tail and leading edge pitched <span style="color: #3682BA; font-weight: bold;">down</span> more (likely symmetrical).',
        'approach8': '<strong>Approaching the obstacle.</strong><br>Strong instance of tail <span style="color: #dc3545; font-weight: bold;">raised</span>.',
        'approach6': '<strong>Approaching the obstacle.</strong><br>Hand-wing more <span style="color: #dc3545; font-weight: bold;">spread</span> during flapping.',
        'approach7': '<strong>Approaching the obstacle.</strong><br>Different <span style="color: #dc3545; font-weight: bold;">m-folding</span> pattern in flapping.',
        'approach9': '<strong>Approaching the obstacle.</strong><br>Hand-wing sweeping <span style="color: #dc3545; font-weight: bold;">forwards</span> more in flapping.',
        'atobstacle1': '<strong>At obstacle.</strong><br>Unusual flap: wings <span style="color: #3682BA; font-weight: bold;">lowered</span> and contracted before <span style="color: #dc3545; font-weight: bold;">raised</span> and spread. Usually the reverse.',
        'atobstacle2': '<strong>At obstacle.</strong><br>Unusual flap: wings lowered and <span style="color: #3682BA; font-weight: bold;">contracted</span> before raised and <span style="color: #dc3545; font-weight: bold;">spread</span>. Usually the reverse.',
        'atobstacle3': '<strong>At obstacle.</strong><br>Wings swept <span style="color: #3682BA; font-weight: bold;">backwards</span> then <span style="color: #dc3545; font-weight: bold;">forwards</span>.',
        'atobstacle4': '<strong>At obstacle.</strong><br>Tail <span style="color: #dc3545; font-weight: bold;">spread</span> more.',
        'atobstacle5': '<strong>At obstacle.</strong><br>Tail and leading edge pitched <span style="color: #3682BA; font-weight: bold;">down</span> and then <span style="color: #dc3545; font-weight: bold;">up</span>.',
        'atobstacle8': '<strong>At obstacle.</strong><br>Tail <span style="color: #3682BA; font-weight: bold;">lowered</span> strongly (likely banking).',
        'atobstacle6': '<strong>At obstacle.</strong><br>Hand-wing <span style="color: #dc3545; font-weight: bold;">spread</span> just before, then neutral.',
        'atobstacle7': '<strong>At obstacle.</strong><br>Brief strong instance of <span style="color: #dc3545; font-weight: bold;">M-folding</span>.',
        'atobstacle9': '<strong>At obstacle.</strong><br>Handwing swept <span style="color: #3682BA; font-weight: bold;">backwards</span>.',
        'recovery1': '<strong>After obstacle recovery.</strong><br>Wings <span style="color: #dc3545; font-weight: bold;">raised</span> to gliding at neutral height.',
        'recovery2': '<strong>After obstacle recovery.</strong><br>Max span gliding immediately.',
        'recovery3': '<strong>After obstacle recovery.</strong><br>Wings swept <span style="color: #dc3545; font-weight: bold;">forwards</span> then <span style="color: #3682BA; font-weight: bold;">back</span> during glide.',
        'recovery4': '<strong>After obstacle recovery.</strong><br>Tail <span style="color: #3682BA; font-weight: bold;">contracted</span> then slightly more <span style="color: #dc3545; font-weight: bold;">spread</span> during glide.',
        'recovery5': '<strong>After obstacle recovery.</strong><br>Tail and leading edge pitched <span style="color: #3682BA; font-weight: bold;">down</span> slightly more during glide.',
        'recovery8': '<strong>After obstacle recovery.</strong><br>Neutral tail banking.',
        'recovery6': '<strong>After obstacle recovery.</strong><br>Hand-wing <span style="color: #3682BA; font-weight: bold;">contracts</span> for glide.',
        'recovery7': '<strong>After obstacle recovery.</strong><br>Slightly less <span style="color: #dc3545; font-weight: bold;">M-folding</span> in glide.',
        'recovery9': '<strong>After obstacle recovery.</strong><br>Hand-wing more swept <span style="color: #dc3545; font-weight: bold;">forwards</span> in glide.'
    };
    
    // Handle regular hover zones
    hoverZones.forEach(zone => {
        zone.addEventListener('mouseenter', function() {
            const gifName = this.dataset.gif;
            const gifPath = `{{ '/assets/img/bird_gifs/PCs/' | relative_url }}${gifName}`;
            
            activeGif.src = gifPath;
            activeGif.style.display = 'block';
            placeholder.style.display = 'none';
            caption.style.display = 'block';
            captionText.innerHTML = modeNames[gifName] || 'Wing morphing pattern';
            contextArea.style.display = 'none'; // Hide context for regular zones
        });
    });
    
    // Handle contextual hover zones
    contextZones.forEach(zone => {
        zone.addEventListener('mouseenter', function() {
            const gifName = this.dataset.gif;
            const contextKey = this.dataset.context;
            const gifPath = `{{ '/assets/img/bird_gifs/PCs/' | relative_url }}${gifName}`;
            
            activeGif.src = gifPath;
            activeGif.style.display = 'block';
            placeholder.style.display = 'none';
            caption.style.display = 'block';
            captionText.innerHTML = modeNames[gifName] || 'Wing morphing pattern';
            
            // Show contextual information
            if (contextData[contextKey]) {
                contextArea.style.display = 'block';
                contextText.innerHTML = contextData[contextKey];
            }
        });
    });
    
    // Optional: Hide gif when leaving the entire heatmap area
    document.querySelector('.interactive-heatmap-container').addEventListener('mouseleave', function() {
        activeGif.style.display = 'none';
        placeholder.style.display = 'flex';
        caption.style.display = 'none';
        contextArea.style.display = 'none';
    });
});
</script> 