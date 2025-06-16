<!doctype html>
<html lang="en">
  <head>
    <title>&lt;model-viewer&gt; Interactive 3D Model</title>
    <meta charset="utf-8" />
    <meta name="description" content="Interactive 3D model with annotations, variants, animations, and AR" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="./styles.css" />
    <style>
      body {
        margin: 0; 
        font-family: Arial, sans-serif;
      }
      model-viewer {
        width: 100vw;
        height: 90vh;
        background-color: #f0f0f0;
      }
      .HotspotAnnotation {
        background: rgba(0, 0, 0, 0.75);
        color: white;
        padding: 4px 8px;
        border-radius: 4px;
        font-size: 12px;
        pointer-events: none;
      }
      .controls {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 8px;
        padding: 8px;
        background: #fff;
        border-top: 1px solid #ccc;
      }
      .controls button {
        padding: 8px 14px;
        font-size: 14px;
        border-radius: 5px;
        border: 1px solid #666;
        cursor: pointer;
        background-color: #eee;
        transition: background-color 0.3s ease;
      }
      .controls button:hover {
        background-color: #ddd;
      }
      .controls button.play {
        background-color: #28a745;
        color: white;
        border-color: #1e7e34;
      }
      .controls button.pause {
        background-color: #dc3545;
        color: white;
        border-color: #a71d2a;
      }
    </style>
  </head>

  <body>
    <model-viewer
      id="modelViewer"
      src="variant1.glb"
      alt="Interactive 3D Model"
      camera-controls
      ar
      ar-modes="webxr scene-viewer quick-look"
      poster="poster.png"
      shadow-intensity="1"
      autoplay
      animation-name="grip remove"
      interaction-prompt="auto"
      exposure="1"
    >
      <!-- Hotspots -->
      <button
        slot="hotspot-1"
        class="Hotspot"
        data-position="0.335 0.04 0.51"
        data-normal="0.37 0.84 0.38"
        data-visibility-attribute="visible"
        onmouseenter="showAnnotation('hotspot1')"
        onmouseleave="hideAnnotation('hotspot1')"
      >
        <div class="HotspotAnnotation" id="hotspot1" style="visibility: hidden;">
          Container
        </div>
      </button>

      <button
        slot="hotspot-2"
        class="Hotspot"
        data-position="0.28 0.05 0.44"
        data-normal="0 1 0"
        data-visibility-attribute="visible"
        onmouseenter="showAnnotation('hotspot2')"
        onmouseleave="hideAnnotation('hotspot2')"
      >
        <div class="HotspotAnnotation" id="hotspot2" style="visibility: hidden;">
          Grip
        </div>
      </button>

      <button
        slot="hotspot-3"
        class="Hotspot"
        data-position="0.23 0.06 0.36"
        data-normal="0 1 0"
        data-visibility-attribute="visible"
        onmouseenter="showAnnotation('hotspot3')"
        onmouseleave="hideAnnotation('hotspot3')"
      >
        <div class="HotspotAnnotation" id="hotspot3" style="visibility: hidden;">
          Screen
        </div>
      </button>

      <!-- Progress bar and AR button -->
      <div class="progress-bar hide" slot="progress-bar">
        <div class="update-bar"></div>
      </div>

      <button slot="ar-button" id="ar-button">View in your space</button>
      <div id="ar-prompt">
        <img src="ar_hand_prompt.png" alt="AR prompt" />
      </div>
    </model-viewer>

    <!-- Controls -->
    <div class="controls">
      <!-- View angle buttons -->
      <button onclick="setView('front')">Front View</button>
      <button onclick="setView('left')">Left View</button>
      <button onclick="setView('top')">Top View</button>

      <!-- Material variant buttons -->
      <button onclick="changeModel('variant1.glb')">Variant 1</button>
      <button onclick="changeModel('variant2.glb')">Variant 2</button>

      <!-- Animation controls -->
      <button onclick="playAnimation('grip remove')" class="play">Play Animation 1</button>
      <button onclick="playAnimation('animation2')" class="play">Play Animation 2</button>
      <button onclick="pauseAnimation()" class="pause">Pause Animation</button>
    </div>

    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/4.0.0/model-viewer.min.js"></script>

    <script>
      const modelViewer = document.getElementById("modelViewer");

      // Annotation visibility handlers
      function showAnnotation(id) {
        document.getElementById(id).style.visibility = "visible";
      }
      function hideAnnotation(id) {
        document.getElementById(id).style.visibility = "hidden";
      }

      // Change model variant by switching GLB source
      function changeModel(src) {
        modelViewer.src = src;
        // Reset to default animation and play
        modelViewer.animationName = "grip remove";
        modelViewer.pause();
        modelViewer.addEventListener(
          "load",
          () => {
            modelViewer.play();
          },
          { once: true }
        );
      }

      // Play specific animation
      function playAnimation(animName) {
        modelViewer.animationName = animName;
        modelViewer.play();
      }

      // Pause animation playback
      function pauseAnimation() {
        modelViewer.pause();
      }

      // Camera views
      function setView(view) {
        switch (view) {
          case "front":
            modelViewer.cameraOrbit = "10.12deg 80.23deg 1.689m";
            modelViewer.fieldOfView = "30deg";
            break;
          case "left":
            modelViewer.cameraOrbit = "350deg 80deg 1.689m";
            modelViewer.fieldOfView = "30deg";
            break;
          case "top":
            modelViewer.cameraOrbit = "7.674deg 0.0000573deg 1.689m";
            modelViewer.fieldOfView = "30deg";
            break;
          default:
            // fallback
            modelViewer.cameraOrbit = "10.12deg 80.23deg 1.689m";
            modelViewer.fieldOfView = "30deg";
        }
        modelViewer.jumpCameraToGoal();
      }
    </script>
  </body>
</html>
