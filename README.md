# 🏡 Modern House 3D Exploration

[![Three.js](https://img.shields.io/badge/Three.js-r160-black?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![WebGL](https://img.shields.io/badge/WebGL-2.0-red?style=for-the-badge&logo=webgl)](https://www.khronos.org/webgl/)
[![AI Generated](https://img.shields.io/badge/Generated%20by-AI%20%2F%20Claude%20Artifacts-9cf?style=for-the-badge&logo=openai)](https://github.com/soheyltaheri/modern-house-3d)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Demo-Live%20Preview-blue?style=for-the-badge&logo=github)](https://soheyltaheri.github.io/modern-house-3d/)

> 🤖 **Note on Creation**: This entire 3D architectural exploration and interactive WebGL scene was **100% generated with AI** (Claude 3.5 Sonnet / AI Coding Artifacts) in a single standalone HTML file (~2,500 lines of procedural Three.js, shaders, dynamic physics, and HUD logic).

An immersive, interactive **3D Architectural Walkthrough Experience** built with **Three.js** and WebGL. Explore a modern interior villa in first-person with dynamic lighting, interactive elements, custom procedural geometries, and a futuristic HUD interface.

---

## ⚡ Live Demo
Experience the 3D walkthrough directly in your browser:
👉 **[https://soheyltaheri.github.io/modern-house-3d/](https://soheyltaheri.github.io/modern-house-3d/)**

---

## 📜 The Exact AI Generation Prompt
Below is the original system prompt that synthesized this entire interactive 3D game into a zero-dependency standalone `index.html`:

```text
Create a fully playable, realistic first-person 3D house exploration game that runs directly in the browser.

Use only:
- HTML
- CSS
- vanilla JavaScript
- Three.js r160 or later, loaded via ES module <script type="module"> with an importmap pointing to jsdelivr or unpkg (e.g. https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.module.js)
- PointerLockControls from three/addons/controls/PointerLockControls.js, imported through the same importmap

Do not use:
- npm, Vite, React, TypeScript, build tools
- external models, textures, images, audio files, fonts, or any asset that requires downloading (no Google Fonts, no @import, no external CSS)
- backend services
- placeholder comments or incomplete systems

Return only one complete index.html file containing all HTML, CSS, and JavaScript. The game must be immediately playable by opening the file in a modern browser. Do not explain anything. Do not provide setup instructions or partial code. Do not truncate or abbreviate any section — if the file is long, still return it in full, uncut.

Core requirements:
1. First-person perspective:
   - True first-person camera with mouse look via PointerLockControls
   - Smooth WASD movement + Sprint (Shift) + Jump (Space)
   - Eye height ~1.7m, base walking speed ~1.4 m/s, sprint ~2.8 m/s, with acceleration/friction and gravity ~9.8 m/s²
   - AABB collision detection against walls, floors, furniture, and door frames
   - Subtle realistic head bobbing while walking

2. The House:
   - Coherent multi-room layout (~100-150 m²): Living Room, Kitchen, Bedroom, Bathroom, Hallway
   - Interactive doors that open/close on proximity or pressing 'E'
   - Semi-transparent glass windows with incoming daylight
   - Procedural furniture: sofa, table, chairs, bed, kitchen counters, fridge, toilet, sink, shelves, lamps
   - Procedural materials (solid colors, PBR MeshStandardMaterial representing wood, fabric, metal, glass)

3. Realism and Polish:
   - Grounded gravity and smooth collision response
   - Realistic interior daytime lighting with soft shadows
   - Minimal HUD: crosshair, dynamic 'Press E' interaction prompts, room indicator badges
   - Pause menu (Escape) and restart option
```

---

## 🤖 AI Generation Breakdown & Architecture
- 🏗️ **Zero External 3D Models (.gltf/.obj)**: All structural components, furniture, lights, and architectural details are procedurally synthesized in code by the AI.
- 📐 **Complex Mathematics & Shaders**: Procedural canvas textures and custom PBR lighting calculations generated end-to-end.
- 🎮 **Full Game Loop**: Integrated input controller, collision detection, pointer-lock camera, and responsive mobile virtual joysticks in ~2.5k lines of pure code.

---

## 🕹️ Controls

| Action | Desktop (Keyboard & Mouse) | Mobile / Touch |
| :--- | :--- | :--- |
| **Move** | <kbd>W</kbd> <kbd>A</kbd> <kbd>S</kbd> <kbd>D</kbd> or Arrow Keys | Left Virtual Joystick |
| **Look Around** | Mouse Move (Click to Lock) | Right Drag Gesture |
| **Interact** | <kbd>E</kbd> or <kbd>Left Click</kbd> | Tap on Screen / Interact Button |
| **Sprint** | <kbd>Shift</kbd> | Double tap joystick |
| **Menu / Pause** | <kbd>Esc</kbd> | Settings Icon |

---

## 🚀 Quick Start (Local Run)

```bash
# Clone
git clone https://github.com/soheyltaheri/modern-house-3d.git
cd modern-house-3d

# Run locally using Python or any static server
python -m http.server 8000
```
Open [http://localhost:8000](http://localhost:8000) in your browser.

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).

---
*Curated & Published by [soheyltaheri](https://github.com/soheyltaheri)* ⚡
