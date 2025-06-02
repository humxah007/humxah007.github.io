---
layout: post
title: High-Fidelity CFD Simulation of Cyclorotor Aerodynamics using Ansys Fluent
description: Performed transient CFD analysis of a cyclorotor system for UAV applications, focusing on vortex dynamics, pressure distribution, and performance characterization.
skills: 
  - CFD simulation with Ansys Fluent
  - Rotating machinery modeling (MRF/Sliding Mesh)
  - Transient turbulence analysis (Realizable k-ε)
  - Vortex dynamics visualization
  - Aerodynamic performance quantification
  - Python/Matlab post-processing

main-image: /profile.jpg
---

## Detailed Description
This project involved comprehensive CFD analysis of a cyclorotor system - a novel vertical takeoff and landing (VTOL) propulsion concept. The simulation modeled four rotating blades (NACA 0012 airfoils) at 600 RPM in a 5m x 5m domain. Key aspects included:
- Transient pressure-based solver with 2nd-order implicit time discretization
- Realizable k-epsilon turbulence model with enhanced wall treatment
- Dynamic mesh handling for blade rotation via Multiple Reference Frame (MRF) approach
- Boundary conditions: 15 m/s axial inflow, pressure outlet, and periodic boundaries
- Quantitative analysis of thrust generation and vortex shedding patterns

## Analysis
The solution revealed critical aerodynamic phenomena:
- Strong tip vortices developing during blade rotation (see pathline visualization)
- Pressure differential of up to 2.5 kPa between blade surfaces
- Velocity vectors showing accelerated flow through blade passages
- Achieved convergence with continuity residuals below 1e-5 after 5,000 iterations

## Conclusion
The cyclorotor configuration demonstrated viable VTOL capabilities with peak thrust of 850N at 600 RPM. Future work should investigate:
1. Blade-pitch modulation during rotation
2. Ground effect interactions
3. Aeroacoustic noise prediction

### Flow Visualization
{% include image-gallery.html images="/pathline.jpg, /static_pressure.jpg, /velocity_vector.jpg" height="400"%}
<span style="font-size: 10px">CFD results: Vortex pathlines, Static pressure distribution, Velocity vectors</span>  

## Pressure Field Dynamics (0.5x Speed)
<video autoplay loop muted playsinline controls width="100%" id="slowmoVideo">
  <source src="/static_pressure.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>
<script>
  document.getElementById('slowmoVideo').playbackRate = 0.5;
</script>

## Experimental Validation
<iframe width="100%" height="415" src="https://www.youtube.com/embed/Ub563Yc3xls" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<span style="font-size: 10px">University of Maryland cyclorotor wind tunnel test (reference)</span>

> "In cyclorotors, the true challenge lies not in achieving lift, but in mastering the vortex."
> — Dr. J. Gordon Leishman, Rotary Aerodynamics Expert

## External Links
- [Ansys Fluent Documentation](https://www.ansys.com/products/fluids/ansys-fluent)
- [Cyclorotor Research at University of Maryland](https://terpconnect.umd.edu/~leishman/Aero/cyclocopter.html)
- [NASA CFD Best Practices](https://turbmodels.larc.nasa.gov/)

## Simulation Parameters

| Category          | Specification |
|-------------------|---------------|
| **Solver Type**   | Pressure-Based, Transient |
| **Turbulence Model** | Realizable k-ε with EWT |
| **Time Step**     | 0.001 s |
| **Domain Size**   | 5m × 5m × 0.1m |
| **Mesh Elements** | 412,890 polyhedral |
| **Boundary Conditions** | Velocity Inlet (15 m/s), Pressure Outlet |
| **Rotation Speed** | 600 RPM |
| **Convergence**   | Residuals < 1e-5 |
| **Visualization** | Vorticity, Q-Criterion, Pressure Iso-surfaces |
