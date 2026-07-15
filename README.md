# Cinematic VR Website

<p align="center">

![HTML](https://img.shields.io/badge/HTML5-100%25-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-Glassmorphism-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Canvas](https://img.shields.io/badge/HTML5-Canvas-black?style=for-the-badge)
![Performance](https://img.shields.io/badge/Optimized-60FPS-success?style=for-the-badge)

</p>

An Apple-inspired cinematic VR landing page built entirely with **HTML5, CSS3, and Vanilla JavaScript**, featuring scroll-driven frame animations, dual HTML5 canvas rendering, custom asset preloading, buttery-smooth interpolation (LERP), and high-performance rendering techniques.

Unlike traditional WebGL implementations, this project achieves a premium 3D visual experience using pre-rendered frame sequences, resulting in exceptional performance across desktop and mobile devices.

---

## Live Demo

**Website:** *(Add your deployed URL here)*

## Table of Contents

- [Overview](#overview)
- [Screenshots](#screenshots)
- [Architecture](#architecture)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [Core Features](#core-features)
- [Performance Optimizations](#performance-optimizations)
- [Animation Pipeline](#animation-pipeline)
- [Engineering Challenges](#engineering-challenges)
- [Lessons Learned](#lessons-learned)
- [Future Improvements](#future-improvements)
- [Contact](#contact)

## Overview

This project recreates the premium storytelling experience commonly found on Apple's product pages by combining scroll-driven animations, cinematic transitions, and responsive layouts into a lightweight web application.

Instead of rendering complex 3D models in real time, the application displays carefully pre-rendered image sequences synchronized with the user's scroll position. This approach delivers a high-end visual experience while maintaining excellent performance and browser compatibility.

The project was built completely from scratch without animation libraries or frontend frameworks, focusing on performance engineering, smooth user interactions, and clean architecture.

## Screenshots

### Hero Section

![HeroSection](assets/herosection.png)

## Architecture

### System Architecture

![Architecture](assets/architecture.png)

The application follows a lightweight client-side architecture where user interactions drive synchronized canvas rendering, animation timing, and asset management entirely within the browser.

Key architectural principles include:

- Dual HTML5 Canvas rendering pipeline
- Scroll-driven animation engine
- Asset preloading before initialization
- requestAnimationFrame rendering loop
- Linear interpolation (LERP) for smooth transitions
- Responsive layout with sticky scrolling sections

## Project Structure

```text
Cinematic-VR-Website
│
├── assets/
│   ├── dashboard.png
│   └── architecture.png
│
├── images/
│   ├── Hero Frame Sequence (90 Frames)
│   └── VR Rotation Sequence (90 Frames)
│
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
├── videos/
│   └── Background CTA Video
│
├── index.html
└── README.md
```

## Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | HTML5 |
| Styling | CSS3 (Glassmorphism, Flexbox, Grid) |
| Programming | Vanilla JavaScript (ES6+) |
| Rendering | HTML5 Canvas API |
| Animation | requestAnimationFrame |
| Performance | Passive Scroll Events, LERP, Asset Preloading |
| Media | Pre-rendered JPG Frame Sequences |
| Deployment | Static Hosting |

## Core Features

- Apple-inspired cinematic landing page experience
- Dual HTML5 Canvas rendering system
- 180 pre-rendered animation frames
- Scroll-driven frame synchronization
- Smooth LERP interpolation
- Asset preloader with loading progress
- Responsive desktop and mobile layouts
- Sticky scroll sections
- Glassmorphism design language
- Modular pricing section
- Testimonial section
- Video-based CTA section
- High-performance rendering pipeline

## Performance Optimizations

Performance was a primary focus throughout development.

### Rendering Optimizations

- HTML5 Canvas rendering
- GPU-friendly drawing pipeline
- `requestAnimationFrame` animation loop
- Passive scroll listeners
- Optimized canvas resizing

### Asset Management

- Complete asset preloading
- Progress-based loading screen
- Zero runtime image fetching
- Memory-efficient frame caching

### User Experience

- Smooth frame interpolation
- Responsive layout calculations
- Sticky scrolling choreography
- Minimal layout shifts
- Fast initial loading experience

## Animation Pipeline

The animation engine converts the user's scroll position into cinematic frame-based motion.

### Rendering Flow

```text
User Scroll
      │
      ▼
Scroll Percentage
      │
      ▼
Frame Calculation
      │
      ▼
LERP Smoothing
      │
      ▼
Canvas Rendering
      │
      ▼
Display Updated Frame
```

The application continuously updates animation frames using `requestAnimationFrame`, ensuring smooth rendering while avoiding unnecessary browser repaints.

Instead of jumping directly to the next frame, a Linear Interpolation (LERP) algorithm gradually moves toward the target frame, creating fluid motion similar to native applications.



