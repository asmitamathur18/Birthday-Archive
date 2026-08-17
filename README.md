# Birthday Archive

> An interactive pixel-art browser experience built with HTML5 Canvas, JavaScript, and CSS.

## Overview

**Birthday Archive** is an interactive browser-based experience designed around exploration, discovery, and progression.

The player navigates through a compact pixel-art environment, interacts with distinct locations, collects items, and progressively unlocks the final sequence. The project combines custom canvas rendering, grid-based movement, interactive states, responsive controls, and animated visual effects into a lightweight standalone web experience.

The entire application runs client-side and requires no backend infrastructure or external runtime dependencies.

---

## Experience

The experience is structured around exploration and progressive discovery.

Players begin in the central environment and navigate through three interactive locations:

* **Burrito** — an interactive menu-based encounter
* **Shawarma** — an item discovery interaction
* **Perfume** — an item discovery interaction

Each location contributes to the player's progression. Once all three locations have been completed, the final area becomes available.

The experience concludes at the birthday cake with a final animated celebration sequence.

---

## Core Features

### Interactive World

A custom grid-based environment rendered using HTML5 Canvas provides the foundation for navigation and interaction.

### Player Navigation

The player can move throughout the environment using:

* Arrow-key controls on desktop
* Touch-based directional controls on mobile devices

### Progressive Gameplay

The game maintains state for each interactive location and tracks the player's progress throughout the experience.

### Interactive Encounters

Different locations provide unique interactions, including selectable menu options, contextual messages, and collectible progress states.

### Final Sequence

After completing all required interactions, the player can reach the final area and trigger the concluding sequence.

### Visual Effects

The final sequence includes a dynamically generated confetti animation rendered on a separate canvas layer.

### Responsive Experience

The interface adapts its controls for touchscreen devices while maintaining keyboard-based navigation on desktop.

---

## Technical Architecture

Birthday Archive is intentionally implemented as a lightweight client-side application.

```text
┌───────────────────────────────┐
│         Browser UI            │
├───────────────────────────────┤
│        HTML Structure         │
├───────────────────────────────┤
│        CSS Styling            │
├───────────────────────────────┤
│      JavaScript Game Logic    │
├───────────────────────────────┤
│       Canvas Rendering        │
├───────────────────────────────┤
│     Game State Management     │
└───────────────────────────────┘
```

The game loop continuously handles input, updates player state, renders the environment, and manages interactions.

---

## Technology Stack

| Technology   | Purpose                                  |
| ------------ | ---------------------------------------- |
| HTML5        | Application structure                    |
| CSS3         | Layout, styling, and responsive controls |
| JavaScript   | Game logic and state management          |
| HTML5 Canvas | Environment and character rendering      |
| Google Fonts | Typography                               |

---

## Game Systems

### Movement System

The environment uses a tile-based coordinate system. Player movement occurs between grid positions while the rendering system provides smooth visual movement between tiles.

### Collision System

Solid tiles and furniture objects are registered as collision boundaries, preventing the player from moving through designated objects.

### Interaction System

The game detects when the player enters specific interaction zones and triggers the corresponding encounter.

### Progress System

Each location maintains its own visited state. The final objective checks the completion state of all required locations before allowing the ending sequence to begin.

### Animation System

Canvas-based animation is used for player movement, visual feedback, and the final confetti sequence.

---

## Project Structure

```text
birthday-archive/
│
└── index.html
```

The current implementation is intentionally self-contained. The HTML file contains the application structure, styling, rendering logic, interaction systems, and game state.

---

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/birthday-archive.git
cd birthday-archive
```

### Run

Open `index.html` in a modern web browser.

No package manager, build system, server, or additional dependencies are required.

---

## Controls

### Desktop

| Input       | Action     |
| ----------- | ---------- |
| Arrow Up    | Move Up    |
| Arrow Down  | Move Down  |
| Arrow Left  | Move Left  |
| Arrow Right | Move Right |

### Mobile

Use the on-screen directional controls provided below the game.

---

## Browser Support

The experience is designed for modern browsers supporting HTML5 Canvas and contemporary JavaScript APIs.

Recommended browsers:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Safari

---

## Design Direction

The visual language combines pixel-art aesthetics with a warm, retro-inspired interface.

The environment uses a tile-based layout, custom-rendered objects, interactive overlays, collectible indicators, and animated transitions to create a compact game-like experience entirely within the browser.

---

## Deployment

Because the project is entirely client-side, it can be deployed using any static hosting provider.

Compatible platforms include:

* Vercel
* GitHub Pages
* Netlify
* Cloudflare Pages
* AWS S3

No backend server is required.

---

## Future Improvements

Potential extensions include:

* Additional interactive locations
* Expanded environments
* Sound effects and background music
* Save and resume functionality
* Additional character animations
* Multiple maps or levels
* More complex interaction systems
* Expanded narrative progression

---

## Project Status

**Status:** Complete

The current version contains the core navigation, interaction, progression, responsive controls, and final celebration systems required for the experience.

---

## License

This project is a personal creative work. All rights reserved.
