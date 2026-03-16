# Griflan Hover Effect

A stunning, fully responsive hover animation project utilizing Vite, GSAP, and Matter.js. This project transforms a static layout into an interactive visual experience where related tags dynamically fall and interact with physics bounded within their service containers when hovered over.

![Features & Interactions](https://img.shields.io/badge/Vite-Ready-brightgreen.svg)
![Mobile Responsive](https://img.shields.io/badge/Responsive-Mobile%20%26%20Tablet-blue)

## Features
- **Dynamic Physics Engine**: Tags fall from above using Matter.js and physically interact with the boundaries of the service containers.
- **Smooth GSAP Animations**: Handling of smooth transitions for color, dynamic container height expansion/collapse, and staggered image trail reveals upon hover.
- **Vite Setup**: Fully modernized with a Vite configuration ensuring lightning-fast Hot Module Replacement (HMR) and optimized, minified production builds.
- **Local Custom Fonts**: Serves `Barlow Condensed`, `Instrument Serif`, and `TANMEMORIES` entirely locally, maintaining perfect visual fidelity and rapid loading.
- **Mobile Responsive**: The layout and physical boundaries natively adapt across Desktop, Tablet, and Mobile views. The physics boundaries intelligently re-calculate according to the screen size.
- **Interactive Micro-Animations**: Features custom CSS interactions such as the right-to-left swift color-invert animation on the `.btn` component.
- **Optimized Media**: Makes use of the modern `.avif` image format for efficient payload delivery.

## Installation

Ensure that you have [Node.js](https://nodejs.org/) installed, then run the corresponding install command located inside the root repository:

```bash
npm install
```

## Running the Development Server

To start up the Vite development server with HMR, type:

```bash
npm run dev
```

Then, open your browser to the URL provided in your terminal (usually `http://localhost:5173/`).

## Building for Production

To create an optimized production build for deployment:

```bash
npm run build
```

The generated application files will be packaged directly into a local `dist` folder, making it super easy to deploy to hosting services like Vercel or Netlify.

## Core Architecture
- **HTML/CSS**: The layout relies on flexbox architecture and absolute positioning to stack initially hidden images and physical boundaries safely. Advanced media queries adjust the root sizes and gaps to keep things fluid.
- **JS Integration**: 
  - GSAP observes the `mouseenter` and `mouseleave` behaviors, orchestrating height tweening and translation.
  - Matter.js coordinates body physics. Invisible walls (left, right, floor) are algorithmically computed for the specific container the user is actively hovering over, letting tags drop naturally like dice.

## Project Assets
The repository contains 8 high-quality `.avif` image assets mapped onto the three major service categories (`BRANDING`, `DIGITAL`, `MOTION`). Fonts and icons are managed locally within their respective folders.
