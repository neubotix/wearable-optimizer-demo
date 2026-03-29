# Wearable Optimizer Demo

An interactive 3D web application for analyzing electronics placement and pressure distribution in wearable frames. Built with Three.js, this engineering tool allows you to visualize and adjust frame parameters in real-time while monitoring comfort metrics and design performance.

## 🚀 Quick Start

Simply open **`index.html`** in your web browser — no server required. The entire app is self-contained in a single HTML file.

### Features

- **3D Frame Visualization**: Interactive 3D model of AR glasses with real-time rendering
- **Parameter Control**: Adjust frame dimensions, electronics placement, weight distribution
- **Comfort Analysis**: Real-time pressure mapping at contact points (nose pad, temple, ear hook)
- **Scenario Presets**: Pre-configured designs (camera-front, balanced-design, battery-rear)
- **Tour Guides**: Two interactive tutorials:
  - **Tour 1**: Overview of 9 major UI sections
  - **Tour 2**: Detailed parameter guide for left-panel controls
- **Electronics Module**: Visual representation of integrated electronics with adjustable position and weight
- **Multiple View Modes**: Solid, Mesh, and Wireframe rendering

## 📋 Login Credentials

- **Email**: (any text)
- **Password**: `ching12345678`

## 🎮 Controls

- **Drag to Rotate**: Click and drag the 3D model to rotate view
- **Scroll to Zoom**: Use scroll wheel to zoom in/out
- **Reset Button**: Restore default view angle
- **View Modes**: Toggle between Solid, Mesh, and Wireframe
- **Sliders**: Adjust frame parameters in real-time

## 📁 Project Files

- `index.html` — Complete, self-contained webapp (463 KB)
  - All 3D models, code, and assets are embedded
  - No external dependencies or build step required
  - Just open in a browser and it works!

## 🔧 Customization

The `index.html` file can be edited directly for minor changes like:
- Text, labels, and descriptions
- Colors and visual styling
- Default parameter values
- UI text and messages

For structural changes or 3D model modifications, contact the developer.

### Default Parameters

The app launches with these default slider values:

| Parameter | Default | Range | Unit |
|-----------|---------|-------|------|
| Position along temple | 0% | 0–100% | - |
| Electronics weight | 3g | 1–25g | grams |
| Lens width | 44.0 | 40–55 | mm |
| Temple length | 140 | 100–160 | mm |
| Bridge width | 17.5 | 10–25 | mm |
| Panto tilt | 0° | -15–15 | degrees |
| Frame Y position | -13 | -20–5 | mm |
| Frame Z offset | +2 | -5–10 | mm |

## 🎨 Customization

The HTML file can be edited directly for minor changes (text, colors, default values). For structural changes or mesh modifications, use the Python generator.

## 📱 Browser Compatibility

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Requires WebGL support

## 📊 Data Visualization

The app displays:

- **Comfort Score**: 0–100 index (green = excellent)
- **Pressure Heatmap**: Contact point pressure in kPa
- **CG Position**: Center of gravity relative to frame
- **Design Insights**: Engineering recommendations

## 📝 License

MIT License — Feel free to modify and share.

## 👤 Creator

Developed for wearable product engineering and comfort analysis.

---

**Questions?** Check the in-app tours or inspect the generator code for implementation details.
