# Griflan Hover Effect

A stunning hover animation project utilizing Vite, GSAP, and Matter.js. This project transforms a simple text list into an interactive visual experience where related tags dynamically fall and interact with physics when hovered.

## Features
- **Dynamic Physics Engine**: Tags fall from above using Matter.js and interact with the service container as physical bodies.
- **Smooth Animations**: GSAP handles smooth transitions for color, height, and image reveals on hover.
- **Vite Setup**: Converted to a modern Vite setup for lightning-fast HMR and optimized builds.
- **Local Fonts**: Fonts are now downloaded and served locally rather than via Google Fonts API.

## Installation

Make sure you have [Node.js](https://nodejs.org/) installed, then run the following in the terminal:

```bash
npm install
```

## Running the Development Server

To start the Vite development server, run:

```bash
npm run dev
```

Then, open your browser to the URL provided in your terminal (usually `http://localhost:5173/`).

## Building for Production

To create an optimized production build:

```bash
npm run build
```

The generated application files will be inside the `dist` folder.

## How It Works
- **HTML/CSS**: Each row is an interactive container that initially hides relevant images and tags.
- **JS (GSAP + Matter.js)**: When you hover over a container (`.service`), GSAP smoothly modifies the layout. At the same time, Matter.js spawns tags that drop in and bounce within predefined boundaries.

## Note on Images
Images have been intentionally left out. You will need to drop appropriate images into the project folder (`service_1_img_1.jpg`, etc.) to see the full aesthetic in action as per the structure defined in `index.html`.
