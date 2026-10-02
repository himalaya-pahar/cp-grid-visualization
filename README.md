# CP Grid Visualizer

An interactive 2D coordinate grid and geometry visualization tool built for competitive programmers, algorithm enthusiasts, and problem solvers to quickly test, sketch, and inspect 2D geometry problems, Manhattan/Euclidean distances, and point-line configurations.

Live Demo: [https://himalaya-pahar.github.io/cp-grid-visualization/](https://himalaya-pahar.github.io/cp-grid-visualization/)

---

## Overview

Competitive programming problems often involve coordinate grids, Manhattan distances, point sets, and geometric paths. **CP Grid Visualizer** provides an instant, zero-setup interactive canvas where you can plot points, connect paths, paste test cases in bulk, and inspect distances in real time.

---

## Features

- **Interactive Canvas Plotting**
  - Click anywhere on the grid to drop a point.
  - Chain points into paths by selecting a point and clicking subsequent locations.
  - Temporary dashed indicator while extending chains.

- **Instant Distance Inspection**
  - Hover over any line segment to see both:
    - **Manhattan Distance ($M$)**: $|x_1 - x_2| + |y_1 - y_2|$
    - **Euclidean Distance ($E$)**: $\sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}$
  - Displayed in a high-contrast HUD tooltip with glowing highlight.

- **Bulk Input Mode**
  - Paste lists of coordinate pairs ($X\ Y$ separated by spaces or newlines) directly from problem statements or sample inputs to plot them simultaneously.

- **Smooth Pan & Adaptive Zoom**
  - Drag to pan across an infinite coordinate space.
  - Mouse wheel to zoom in/out with dynamically adjusting grid tick marks ($1, 2, 5, 10, 20$).

- **Read-Only / Inspection Mode**
  - Switch to Read-Only mode to inspect coordinates and explore complex graphs without accidentally adding points or lines.

- **Snap to Grid**
  - Toggle between strict integer coordinates (ideal for discrete CP grids) and 2-decimal floating point precision.

- **Full Undo & Redo**
  - Undo and redo history up to 50 operations (`Ctrl+Z`, `Ctrl+Shift+Z` / `Ctrl+Y`).

- **Contextual Deletion**
  - Right-click any point or line segment to instantly remove it.
  - Cancel selection with `Right-Click` or `Esc`.

- **Export to Image**
  - One-click export to PNG (`cp-grid-visualizer.png`) with crisp dark-themed styling and watermark.

- **Collapsible Sidebar & Modern Dark UI**
  - Toggleable sidebar for an unobstructed full-screen canvas view.
  - Built with high-contrast neon accents, JetBrains Mono, and Inter typography.

---

## Controls & Shortcuts

| Action | Control / Shortcut |
|---|---|
| **Add Point** | Click empty canvas or use **Quick Add** input |
| **Connect Points / Chain** | Click Point $A$ (selects it) $\rightarrow$ Click Point $B$ (or empty space) |
| **Inspect Line Distance** | Hover cursor over any connecting line |
| **Inspect Point** | Hover cursor over point or click in Read-Only mode |
| **Pan Canvas** | Left Click + Drag on empty space |
| **Zoom In / Out** | Mouse Wheel (`Scroll`) |
| **Cancel Selection** | `Right Click` on empty space or press `Esc` |
| **Delete Point / Line** | `Right Click` directly on the point or line |
| **Undo** | `Ctrl + Z` (or `Cmd + Z` on macOS) |
| **Redo** | `Ctrl + Shift + Z` / `Ctrl + Y` (or `Cmd + Shift + Z` on macOS) |
| **Toggle Sidebar** | Hamburger button on the top-right corner |

---

## Tech Stack

- **Core**: Vanilla HTML5, CSS3, JavaScript (Canvas 2D API)
- **Typography**: [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) & [Inter](https://fonts.google.com/specimen/Inter)
- **Zero Dependencies**: No libraries, build steps, or package installations required. Runs natively in any modern web browser.

---

## Getting Started

### Option 1: Direct File Open
Simply double-click `index.html` or open it with your favorite browser:
```bash
open index.html # On macOS
# or
xdg-open index.html # On Linux
# or
start index.html # On Windows
```

### Option 2: Local HTTP Server (Optional)
Using Python:
```bash
python3 -m http.server 8000
```
Or using Node `npx serve`:
```bash
npx serve .
```
Then navigate to `http://localhost:8000` in your browser.

---

## Author

**Nafis Shahriar**
- LinkedIn: [nafis-shahriar-687402287](https://www.linkedin.com/in/nafis-shahriar-687402287/)
- Codeforces: [Himalaya_](https://codeforces.com/profile/Himalaya_)
