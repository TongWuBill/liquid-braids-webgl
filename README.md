# Liquid Braids

A lightweight WebGL system that simulates fluid-like behavior through line fields, noise, and light diffusion — without heavy particle simulations.

Live Demo: https://tongwu.studio

---

## Overview

**Liquid Braids** is an exploration of *perceptual fluidity*.

Instead of simulating physically accurate fluids (e.g. Navier–Stokes),  
this project focuses on how motion, layering, and diffusion can create the *feeling* of fluid.

The goal:
> Design a system that feels alive — while remaining lightweight and accessible across devices.

This system is now used as the homepage background for my personal website.

---

## Concept

Traditional fluid simulations rely on complex physics and high computational cost.

This project takes a different approach:

- No particles
- No physics simulation
- No heavy GPU load

Instead, it builds fluid-like motion through:

- Layered line-based flow structures  
- Fractal noise (FBM) for organic variation  
- Shader-driven color diffusion and blending  

This creates a visual system that behaves like fluid — without actually simulating fluid.

> Not simulating physics — simulating perception of flow.

---

## Interaction Design

Interaction is modeled as a **“stirring force”**.

User input dynamically alters the flow field:

- Cursor / touch position acts as a center of influence  
- Movement velocity affects rotation and distortion  
- Presence controls intensity of interaction  
- Flow responds smoothly with temporal easing  

The result is a system that feels responsive, continuous, and tactile.

---

## Technical Approach

Built entirely with **WebGL (GLSL shaders)**.

### Core Techniques

- **Line-based flow fields**  
  Replaces particle systems with layered sine-driven streams  

- **FBM Noise (Fractal Brownian Motion)**  
  Generates organic motion and background variation  

- **Pigment Mixing (Non-linear blending)**  
  Uses sqrt-based color blending for more natural diffusion  

- **Full-screen quad rendering**  
  Minimal geometry → maximum efficiency  

- **Shader-only computation**  
  No CPU-heavy simulation loops  

---

## Performance

Designed to be **GPU-efficient and device-friendly**.

- No particle simulation overhead  
- Minimal draw calls  
- Resolution-aware rendering (DPR capped)  
- Stable performance across desktop and mobile  

This allows the system to run smoothly as a real-time background on a live website.

---

## Visual System

The visual language is inspired by:

- Fluid ink diffusion  
- Pigment interaction in water  
- Braided motion structures  

Color palettes transition dynamically, creating a continuous evolving system.

---

## Why This Approach

Most real-time fluid visuals prioritize physical accuracy.

This project explores an alternative direction:

> What if we design for perception instead of simulation?

By focusing on *how fluid feels*, rather than how it behaves physically,  
we can build systems that are:

- More efficient  
- More controllable  
- More expressive  

---

## Use Case

- Interactive website backgrounds  
- Generative visual systems  
- Real-time installations  
- Creative coding experiments  

---

## Future Directions

- Audio-reactive modulation  
- Multi-touch / gesture expansion  
- Integration with 3D spatial systems  
- WebGPU implementation  

---

## Author

Tong Wu  
Creative Technologist / Interactive Systems Designer  

Portfolio: https://tongwu.studio  

---

## License

MIT License
