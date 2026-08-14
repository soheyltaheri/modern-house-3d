# 🏡 Modern House 3D Exploration

[![Three.js](https://img.shields.io/badge/Three.js-r160-black?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![WebGL](https://img.shields.io/badge/WebGL-2.0-red?style=for-the-badge&logo=webgl)](https://www.khronos.org/webgl/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Demo-Live%20Preview-blue?style=for-the-badge&logo=github)](https://otka256.github.io/modern-house-3d/)

An immersive, interactive **3D Architectural Walkthrough Experience** built with **Three.js** and WebGL. Explore a modern interior villa in first-person with dynamic lighting, interactive elements, custom shaders, and a futuristic HUD interface.

---

## ✨ Features

- 🎮 **First-Person Walkthrough**: Smooth WASD movement, pointer-lock mouse look, and physics/collision handling.
- 💡 **Dynamic Lighting & Shadows**: Realistic ambient occlusion, soft directional shadows, and warm interior point lights.
- 🛋️ **Interactive Objects**: Inspect and toggle house appliances, lights, doors, and interactive triggers in real time.
- 🧭 **Heads-Up Display (HUD)**: Sleek glassmorphism room badges, dynamic reticle crosshair, mini-map / spatial location tags, and integrated control hints.
- 📱 **Mobile & Desktop Responsive**: Supports touch joysticks for mobile browsers as well as keyboard + mouse controls.
- ⚡ **Zero-Build Architecture**: Powered by native ES Modules and modern CDN imports (no bundler required).

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

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/otka256/modern-house-3d.git
cd modern-house-3d
```

### 2. Run locally
Since the project uses ES modules, serve it using any local HTTP server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve .
```

Open [http://localhost:8000](http://localhost:8000) in your browser.

---

## 🛠️ Tech Stack
- **Rendering Engine**: [Three.js](https://threejs.org/) (r160)
- **Styling**: Vanilla CSS3 (Glassmorphism & Backdrop Filters)
- **Deployment**: GitHub Pages (Automatic zero-config static hosting)

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).

---
*Created by [otka256](https://github.com/otka256)* ⚡
