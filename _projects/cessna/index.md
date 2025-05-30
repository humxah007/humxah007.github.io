
---
layout: post
title: Aircraft Performance Analysis - Cessna 172 Skyhawk
description: Comprehensive analysis of the world's most-produced aircraft covering unaccelerated/accelerated flight regimes, thrust/power curves, climb/glide performance, and takeoff/landing metrics.
skills: 
  - Aerodynamic Parameter Estimation (CL/CD, L/D ratios)
  - MATLAB Programming & Data Visualization
  - Flight Performance Calculation (stall, climb, range)
  - Takeoff/Landing Distance Modeling
  - Energy Methods (V-n diagrams, Ps contours)
  - Error Analysis & Validation

main-image: /projects/cessna/pictures/profile.jpg
---

## Detailed Description
This project conducted a full-spectrum performance analysis of the Cessna 172S Skyhawk trainer aircraft:

1. **Unaccelerated Flight:**
   * Derived thrust/power required curves using drag polar $C_D = 0.0341 + 0.0292C_L^2$
   * Calculated max L/D ratio (17.47 @ 864 ft/s), stall speed (86.8 ft/s SL), and climb performance (24.2 ft/s ROC at SL)
   
2. **Accelerated Flight:**
   * Determined turn performance (679 ft min radius, 16°/s max rate)
   * Modeled range (1,185 km) and endurance (4.5 hrs) with specific fuel consumption
   
3. **Operational Analysis:**
   * Takeoff distance: 834 ft (ground roll + airborne)
   * Landing distance: 813 ft (approach-to-ground roll)
   
4. **Validation:** Compared results against factory specs, identifying error sources (e.g., 28% thrust deviation due to drag polar assumptions)

## Analysis
The performance metrics were benchmarked against actual aircraft data to validate computational methods.

### Key Findings and Observations:
* **Thrust Prediction:** Min required thrust was underestimated due to simplified induced drag modeling, resulting in a 28% error
* **Takeoff/Landing Performance:** Within a 13% margin of actual data, indicating acceptable accuracy using energy-based models
* **Stall Speed:** Closely aligned with published values (1.8% deviation), reflecting robust CLmax estimates
* **Turn Performance:** Showed distinct thrust and CLmax constraints across speed regimes
* **Ceiling Calculation:** Exactly matched actual specification, validating standard atmosphere methods

### Aircraft Diagrams
{% include image-gallery.html images="/projects/cessna/pictures/details.jpg, /projects/cessna/pictures/3views.jpg" height="400"%}
<span style="font-size: 10px">Aircraft systems diagram and three-view drawings</span>

### Wing Analysis
{% include image-gallery.html images="/projects/cessna/pictures/wing_iso.jpg, /projects/cessna/pictures/wing_side.jpg, /projects/cessna/pictures/wing_top.jpg" height="300"%}
<span style="font-size: 10px">Wing geometry analysis: Isometric, side and top views</span>

### Flight Demonstration
{% include youtube-video.html id="DvCv2SuKCE8" autoplay="false" %}

## Conclusion
The analysis confirmed the Cessna 172's exceptional training suitability—forgiving stall characteristics, stable low-speed handling, and predictable performance. Discrepancies versus factory data (≤28% error) stemmed from simplified drag modeling and constant-efficiency assumptions. Validated methodologies provide a framework for piston-aircraft performance optimization.

## Additional Text
*Methodological Notes:*
* Assumed constant propeller efficiency (η=0.7)
* Used $C_{L_{max}}$ = 1.63 (clean)/1.2 (flaps)
* Density model: ISA standard atmosphere
* Code appendix: 16 MATLAB scripts for parametric analysis

> *"The Cessna 172 taught the world to fly—not because it’s extraordinary, but because it makes the extraordinary achievable."*  
> **— Aviation Historian**

## External Links
* [Cessna 172S Specifications (Textron Aviation)](https://cessna.txtav.com/en/piston/cessna-172)
* [FAA Pilot’s Handbook (Performance Chapter)](https://www.faa.gov/regulations_policies/handbooks_manuals/aviation/phak)

## Performance Comparison
| **Parameter**        | **Calculated** | **Actual** | **Error** | **Insight**                    |
| -------------------- | -------------- | ---------- | --------- | ------------------------------ |
| **Min Thrust**       | 50 lb          | 70 lb      | 28%       | Underestimated induced drag    |
| **Takeoff Distance** | 834 ft         | 960 ft     | 13%       | Constant thrust assumption     |
| **Stall Speed (SL)** | 86.8 ft/s      | 85.3 ft/s  | 1.8%      | High-fidelity match            |
| **Max Velocity**     | 234 ft/s       | 275 ft/s   | 15%       | Propeller efficiency variation |
| **Service Ceiling**  | 14,000 ft      | 14,000 ft  | 0%        | Validated ceiling calculation  |

## Critical Metrics
| **Category**        | **Parameter**           | **Value**         |
| ------------------- | ----------------------- | ----------------- |
| **Aerodynamics**    | Max L/D Ratio           | 17.47 @ 864 ft/s  |
| **Climb**           | Service Ceiling         | 14,000 ft         |
|                     | Max Rate of Climb (SL)  | 24.2 ft/s         |
| **Range/Endurance** | Max Range               | 1,185 km (640 nm) |
|                     | Endurance               | 4.5 hours         |
| **Maneuvering**     | Min Turn Radius (SL)    | 679 ft            |
|                     | Max Turn Rate (SL)      | 16 deg/s          |
| **Operational**     | Takeoff Distance (MTOW) | 834 ft            |
|                     | Landing Distance        | 813 ft            |
