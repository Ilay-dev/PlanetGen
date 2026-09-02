# PlanetGen

<img width="1920" height="1080" alt="Planet_v2" src="https://github.com/user-attachments/assets/4d1142ac-9374-4c8c-aacc-ffa7fe4ff972" />


A professional, browser-based 3D planet generator. Create highly detailed, photorealistic planets procedurally and export them as `.glb` files for use in Blender, Unity, Unreal Engine, or web viewers.

## Features

- **100% Procedural:** Powered by GPU-accelerated WebGL shaders (FBM, Ridge Noise, Domain Warping).
- **Extreme Resolutions:** Supports texture generation from 512 up to an insane 32K (32768x16384).
- **Advanced Biomes:** Smooth biome blending, realistic climate zones (ice poles), and micro-details like winding rivers and sharp mountain ridges.
- **Weather System:** Dynamic, multi-layered cloud rendering with realistic shadows.
- **One-Click Export:** Instantly export your creation (including color, displacement, roughness, and transparent cloud layers) into a standard `.glb` 3D model.
- **State Management:** Save and load your custom planet configurations locally.

## Usage

No installation or build tools required.

1. Download or save the `index.html` file.
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari).
3. Tweak the sliders on the left panel to shape your world.
4. Click **Generate Textures** to apply your changes.
5. Click **Export GLB** to download the 3D model.

## UI Controls Overview

- **Global Settings:** Choose presets, adjust texture resolution, or save/load your current state.
- **Terrain Base:** Control land mass percentage, fragmentation (Pangea vs. Island archipelagos), and overall scale.
- **Micro Details:** Adjust how biomes blend into each other, generate mountain ridges, and add chaotic, meandering rivers.
- **Atmosphere:** Control the size of the polar ice caps and the density/turbulence of the cloud layer.
- **Biome Thresholds:** Set exact sea levels and height thresholds for sand, grass, and rock.
- **Colors:** Fully customizable color palette for oceans, landmasses, and weather.

## Performance Note

Generating textures at extremely high resolutions (16K, 32K) requires significant GPU memory (VRAM). When selecting these resolutions, your browser may freeze for a few seconds while the graphics card processes the shaders. If your browser crashes, lower the resolution before exporting.

## Tech Stack

- HTML5 / CSS3
- Vanilla JavaScript
- [Three.js](https://threejs.org/) (Loaded via ES modules)
- GLSL (Custom WebGL Shaders for real-time texture rendering)
