---
title: "I am just leaving this here as a source of motivation"
excerpt: "Short description of portfolio item number 1<br/><img src='/images/500x300.png'>"
collection: portfolio
---
{% raw %}
    <div class="canvas-container">
        <span class="loading">Loading...</span>
        <canvas width="1024" height="1024" id="canvas"></canvas>
    </div>
    <div class="instructions">
        <p>Use <kbd>↑</kbd> <kbd>↓</kbd> <kbd>←</kbd> <kbd>→</kbd> to move the element in the canvas.</p>
    </div>
    <script src="/assets/js/coi-serviceworker.js"></script>
    <script>
        var Module = {
            // This is called when the Emscripten module is ready
            onRuntimeInitialized: () => {
                console.log("Emscripten module initialized");
                var loadingText = document.querySelector('.loading');
                loadingText.style.display = 'none';
            },
            canvas: (() => {
                var canvas = document.getElementById('canvas');
                canvas.addEventListener("webglcontextlost", function (e) {
                    alert('WebGL context lost. Reload the page.');
                    e.preventDefault();
                }, false);
                return canvas;
            })()
        };
    </script>
    <script src="/assets/js/demo.js"></script>
{% endraw %}
For now it's empty.
