# Design Rules & Style Guide

This document outlines the design system and UI patterns used for the **Rockies Itinerary** and related web pages.

## 1. Color Palette

| Name | Hex/RGBA | Usage |
| :--- | :--- | :--- |
| **Alpine Blue** | `#1a3a5f` | Primary background, navigation, and badges. |
| **Forest Green** | `#2d5a27` | Highlights and nature-themed elements. |
| **Sunset Orange** | `#e67e22` | Call-to-action buttons and accents. |
| **Glass Background** | `rgba(255, 255, 255, 0.7)` | Cards and overlays for a premium feel. |
| **Glass Border** | `rgba(255, 255, 255, 0.3)` | Subtle borders on cards. |

## 2. Typography

*   **Headings (H1 - H4)**: `Playfair Display`, serif. Used for titles to give a classic, cinematic look.
*   **Body Text**: `Inter`, sans-serif. Used for readability and modern feel.

## 3. Core Components

### 3.1 Glass Cards (`.glass-card`)
*   **Background**: Glassmorphism effect (`backdrop-filter: blur(12px)`).
*   **Border Radius**: `1.5rem` (24px).
*   **Hover Effect**: Translates `-5px` vertically with an enhanced shadow.

### 3.2 Stage Badges (`.stage-badge`)
*   **Background**: Linear gradient from `Alpine Blue` to `Blue-500`.
*   **Shape**: Pill-shaped (fully rounded).
*   **Typography**: 14px, Semi-bold.

### 3.3 Navigation (`.nav-sticky`)
*   **Background**: Semi-transparent `Alpine Blue` with blur.
*   **Link Animation**: Yellow underline expands from 0% to 100% width on hover.

### 3.4 Image Zoom (`.image-zoom`)
*   **Behavior**: Images scale up slightly (`1.08x`) within their container on hover.
*   **Transition**: `0.8s` cubic-bezier for a smooth, high-end feel.

## 4. Itinerary Patterns

### 4.1 Logistics Bar
A standardized horizontal bar for each day's logistics:
*   **Icons**: 🚗 (Driving), 🏠 (Stay), 🥾 (Distance), 🏔️ (Elevation), ⏱️ (Time).
*   **Styling**: 10-12px bold text, uppercase tracking, light border separator.

### 4.2 Alternating Layout
*   Two-column grid (`lg:grid-cols-2`).
*   **Rhythm**: Content on left / Image on right, followed by Image on left / Content on right.
*   **Mobile**: Always stacks to single column with image on top or proportional to importance.

## 5. Visual Standards
*   **Hero Image**: High-resolution, cinematic landscapes (`90vh` height).
*   **Video Integration**: Full-screen overlays for immersive travel footage.
*   **Shadows**: Use soft, layered shadows (`shadow-2xl`) for depth.

## 6. Deployment Process

The project is hosted on GitHub Pages. To deploy updates, follow these steps:

1.  **Stage Changes**: Ensure all modified HTML, CSS, and image assets are staged.
    ```bash
    git add .
    ```
2.  **Commit**: Use a descriptive commit message (e.g., `feat:`, `fix:`, `refactor:`).
    ```bash
    git commit -m "feat: [brief description of changes]"
    ```
3.  **Push**: Push to the `main` branch to trigger the automatic deployment.
    ```bash
    git push origin main
    ```
4.  **Verify**: Visit [scouting.tw](https://scouting.tw) or [scouting-tw.github.io](https://scouting-tw.github.io) to confirm the changes are live.
