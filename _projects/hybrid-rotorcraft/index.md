---
layout: post
title: Hybrid Rotorcraft-Bicycle Conversion System
description: |
    Engineered a dual-mode VTOL system that seamlessly transitions into a bicycle without disassembly. 
    Addressed battery limitations through a mechanical pedal-drive backup, enabling efficient urban mobility 
    both in the air and on the ground.
skills: 
  - CAD Modeling (CREO / Fusion 360)
  - FEA & CFD (ANSYS)
  - Aerodynamic Sizing & Performance Prediction
  - Kinematic Linkage Design
  - Material Selection (CFRP, Al 7075-T6)
  - Structural & System-Level Optimization
main-image: /_projects/hybrid-rotorcraft/pictures/profile.jpg
---

# Detailed Description
This project involved the design and development of a hybrid manned aerial vehicle that converts into a bicycle post-landing—ideal for last-mile transportation. The aircraft consists of four rotors mounted on telescopic arms that retract and rotate to function as wheels. A compact, high-efficiency chain-pedal mechanism powers the vehicle in ground mode.

Key innovations include a spring-loaded locking system with a safety factor of 4, vibration-damped motor mounts, and integrated battery casing optimized for center-of-gravity stability. ANSYS-based structural simulations confirmed impact resistance up to 3g, while aerodynamic profiling reduced drag by 18% compared to baseline drone models.

## Analysis
The propulsion system delivers 515 N of thrust per motor, ensuring more than twice the lift required for vertical takeoff and hover, thereby guaranteeing stable VTOL operation. The spring-loaded locking mechanism was engineered to withstand forces up to 2,500 N, achieving a safety factor of 4 based on static FEA results. Aerodynamic enhancements—including the use of blended fairings and streamlined frame geometry—contributed to an 18% reduction in drag. Power demands during flight were met using a 60V, 233Ah LiPo battery, with total power consumption measured at 41.95 kW. Additionally, the transformation from flight to bicycle mode was validated through ANSYS Motion simulations, completing the mechanical transition in just 0.5 seconds—critical for real-world urban use cases.

## Conclusion
The rotorcraft-bicycle concept delivers a 40% reduction in urban mobility accident risk compared to motorcycles and eliminates fuel and infrastructure dependencies. By addressing major eVTOL challenges—battery anxiety, ground mobility, and modularity—this design offers a sustainable alternative for future urban commuting.

## Additional Text
Project aligns with **UN SDGs 8, 9, and 17**, promoting sustainable innovation in transportation. Projected economic benefit includes up to **\$5,000 annual savings** per user from fuel, maintenance, and parking eliminations.

> *"The rotorcraft-bicycle doesn't just bridge air and ground – it connects engineering ingenuity to sustainable human mobility."*

## Design Visualizations
### Isometric Views
{% include image-gallery.html images="/_projects/hybrid-rotorcraft/pictures/bike-iso.jpg, /_projects/hybrid-rotorcraft/pictures/drone-iso.jpg" height="400"%}
<span style="font-size: 10px">Isometric views of bicycle and rotorcraft configurations</span>  

## Mechanism Demonstration
### Conversion Sequence
{% include local-video.html file="/_projects/hybrid-rotorcraft/images/conversion-mechanism.mp4" %}

<br>

## External Links
[Institute of Space Technology – Official Website](http://www.ist.edu.pk/)  
[Jetson One – Technical Specifications](https://www.jetsonaero.com/tech-specs)  
[T-Motor U15 – Datasheet](https://store.tmotor.com/goods.php?id=1083)

## Performance Specifications
| **Specification** | **Flight Mode**       | **Bicycle Mode**            |
| ----------------- | --------------------- | --------------------------- |
| Max Speed         | 102 km/h              | 25 km/h                     |
| Endurance         | 20 min (battery only) | Unlimited (pedal-drive)     |
| Payload Capacity  | 100 kg                | 100 kg                      |
| Frame Material    | CFRP (1.55 g/cm³)     | Al 7075-T6 joints           |
| Power Source      | 60V LiPo, 233Ah       | Human-powered chain (98% η) |
| Safety Rating     | 3g crash-survivable   | FoS = 4 structural locks    |
