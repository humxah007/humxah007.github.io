---
layout: post
title: 2D CFD of Wedge Airfoil for Hypersonic Regime Using ANSYS at Mach 3.5
description: Simulated 2D flow over a wedge-shaped airfoil at Mach 3.5 using ANSYS Fluent to study shock formation and high-temperature effects.
skills: 
  - Compressible flow analysis
  - Hypersonic shockwave modeling
  - 2D mesh generation
  - ANSYS Fluent high-speed flow setup
main-image: /profile.jpg
---

# Detailed Description
In this CFD project, a wedge airfoil was simulated under hypersonic conditions at Mach 3.5. The simulation focused on analyzing oblique shockwave behavior, pressure rise across the shock, and temperature variation. Inviscid and viscous models were compared. Boundary conditions were defined precisely with freestream pressure at 101325 Pa and temperature at 300 K. The mesh contained 250,000 quadrilateral elements with boundary layer refinement (y+ < 1). Results were validated against theoretical shock angles using θ-β-Mach relations and demonstrated close correlation with Prandtl-Meyer expansion theory.

# Analysis
## Flow Field Visualization
{% include image-gallery.html images="/mach.jpg, /press.jpg, /vel.jpg, /stream.jpg" height="400"%}
<span style="font-size: 10px">Top-left: Mach number contour • Top-right: Pressure distribution • Bottom-left: Velocity vectors • Bottom-right: Streamline pattern</span>  

## Key Observations:

 Oblique shock angle measured at 32.4° (theoretical: 31.8°)

 Post-shock temperature reached 1200K at leading edge

 Pressure ratio across shock: 12.8 (vs theoretical 12.3)

 Boundary layer separation observed at 15° deflection angle

# Conclusion
The project reinforced understanding of hypersonic aerodynamics, including thermal loads and shockwave patterns associated with wedge-shaped leading edges. The ANSYS Fluent simulation successfully captured complex phenomena like shock-boundary layer interactions and expansion fans. Results demonstrated that wedge geometries produce more predictable shock patterns than blunt bodies at Mach 3.5, though thermal management remains critical due to stagnation temperatures exceeding 1000K.

## Aerofoil Concept Demonstration
{% include youtube-video.html id="6wgrDBa-AXo" autoplay="false" %}

> "In hypersonic flight, the air doesn't whisper—it roars in compressed fire."
> — Aerospace CFD Specialist

## External Links
[NASA Hypersonics Research](https://www.nasa.gov/topics/aeronautics/features/hypersonic.html)  
[ANSYS Academic CFD](https://www.ansys.com/academic)
