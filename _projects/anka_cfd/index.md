---
layout: post
title: CFD Aerodynamic Validation - ANKA-3 Flying Wing UAV
description: Performed high-accuracy CFD simulations on the stealth ANKA-3 UAV to analyze lift and drag performance at various angles of attack. The k-omega SST model was validated with <5% deviation from experimental data.
skills: 
  - ANSYS Fluent (CFD)
  - k-omega SST turbulence modeling
  - CATIA CAD modeling
  - Aerodynamic analysis
  - Contour visualization
  - Validation techniques
  - Technical documentation

main-image: /profile.jpg
---

# Detailed Description
This project involved conducting computational fluid dynamics (CFD) analysis of the ANKA-3 flying wing UAV to evaluate aerodynamic performance. Using CATIA, a radar-deflective geometry was modeled and meshed with 10 inflation layers to resolve the boundary layer accurately. Simulations were executed in ANSYS Fluent using the k-omega SST turbulence model at a cruise speed of 150 m/s and at angles of attack ranging from 0° to 12°.

The project focused on quantifying lift (Cl) and drag (Cd) coefficients, understanding flow behavior, and validating numerical accuracy through comparison with published experimental results. The CFD findings confirmed aerodynamic efficiency at lower AoAs and highlighted critical flow separation risks at higher AoAs.

## Analysis
The analysis revealed clear aerodynamic trends in the ANKA-3 UAV's behavior across the tested AoA spectrum.

 At **3° AoA**, the aircraft achieved peak aerodynamic efficiency with attached flow and minimal drag.
 As AoA increased beyond **6°**, significant flow separation was detected, particularly at the wingtips, leading to a 27% increase in drag.
 The k-omega SST model consistently delivered lift and drag values with high accuracy, maintaining deviation within ±5% compared to experimental data.

### Comparison of Simulated vs. Validated Aerodynamic Coefficients

| **Angle of Attack (AoA)** | **Lift Coefficient (Cl)** | **Cl Deviation** | **Drag Coefficient (Cd)** | **Cd Deviation** |
| ------------------------- | ------------------------- | ---------------- | ------------------------- | ---------------- |
| 0°                        | 0.08                      | +3.2%            | 0.022                     | -1.8%            |
| 3°                        | 0.42                      | +1.1%            | 0.041                     | +0.7%            |
| 6°                        | 0.61                      | -3.9%            | 0.098                     | -2.2%            |
| 12°                       | 0.38                      | +4.6%            | 0.157                     | +3.3%            |

### Conclusion
The validated CFD methodology successfully captured the aerodynamic behavior of the ANKA-3 UAV. The study supports its stability for low-AoA missions while indicating instability risks at higher AoA due to turbulent flow separation. These insights help guide future design optimization and reduce dependence on physical wind tunnel testing.

### Additional Text
This analysis sets the groundwork for enhanced aerodynamic control strategies such as vortex generators or active flow regulation. Future studies could explore unsteady-state behavior, gust response, and stall prediction models.

## CFD Results Visualization
### Pressure Contour and Flow Characteristics
{% include image-gallery.html images="/press.jpg, /vel_vect.jpg, /vel_proj.jpg, /stream.jpg" height="350"%}
<span style="font-size: 10px">From left: Surface pressure distribution, Velocity vectors, Velocity magnitude projection, Streamline visualization</span>  

## Flight Demonstration
### ANKA-3 UAV Flight Debut
{% include youtube-video.html id="fAnxwJk0h10" autoplay="false" %}
<span style="font-size: 10px">Official test footage of ANKA-3 UAV (Source: TUSAŞ)</span>  

## Quote
> *"In CFD, we don’t guess—we compute, validate, and conquer aerodynamic uncertainty."*  
> — Adapted from **John D. Anderson**, *Computational Fluid Dynamics Pioneer*

## References
- [ANKA-3 UAV Info - TUSAŞ](https://www.tusas.com/en/products/anka-3)
- [ANSYS k-omega SST Turbulence Model](https://www.ansys.com/products/fluids/ansys-fluent/turbulence-models)
- [Validation Source: AFASES 2016 Paper](https://doi.org/10.19062/2247-3173.2016.18.1.22)
