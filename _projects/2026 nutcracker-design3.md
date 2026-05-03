---
layout: project
title: Nutcracker design 3
description: HW 12- Design Problem 
image: /assets/images/beam1.jpg
---


## Homework 12- Design Problem Additional 2

For this assignment, I revisited my original macadamia nutcracker design from Homework 4. In the original design, the nutcracker handles were assumed to be rigid. For the updated design, the handles were instead modeled as elastic beams that bend under the combined transverse forces from the nut and the linear actuator.

## Assumptions:

To simplify the analysis, I made the following assumptions:

- The bottom handle of the nutcracker can be modeled as a simply supported beam.
- The pin connection acts as one support.
- The linear actuator acts like a roller support at the end of the handle.
- The force from the nut acts as a concentrated downward force on the beam.
- Only transverse forces were considered.
- The triangular jaw geometry was treated as an equilateral triangle.
- The nut was assumed to be at the instant of cracking.

![]({{'/assets/images/beam1.jpg'| relative_url}}) 

From my previous design, the required nut-cracking force was:


F_{nut} = 2570.5 N

The actuator force was:

F_{actuator} = 173.5 N

The beam length was:

L = 0.3336 m

Since the maximum allowed deflection was 2% of the beam length,

delta_{max} = 0.02(0.3336) = 0.006672 m

## Maximum Deflection Location



The nut force was located at:

a = 0.0273 m

from the pin support. The remaining beam length to the actuator support was:

b = 0.3063 m

Using the beam deflection equation from Appendix E for the case where (a < b), the location of maximum deflection is:

x_m= 0.192 m ( from the pin)


## Beam Design

To keep the vertical elastic deflection below 2% of the beam length, I used the maximum deflection equation:

I used polycarbonate as the beam material, with an elastic modulus of approximately:

E = 2.4*10^9  Pa
Solving for the required moment of inertia gave:

I = 0.03097*10^6 mm^4

Using a beam chart, the closest available cross-section was a polycarbonate C-channel with:


I_x = 0.677*10^6 { mm}^4

This value is greater than the required moment of inertia, so the selected beam should keep the elastic deflection below the 2% limit.

![]({{'/assets/images/beam2.jpg'| relative_url}}) 
## Final Design

My final design uses a polycarbonate C-channel beam for the nutcracker handle. The chosen cross-section has approximate dimensions:

75 { mm} times 8.9 \text{ mm}


The beam is supported by a pin on one side and the actuator on the other side. The nut force acts downward near the pin, while the actuator applies force near the end of the handle. The maximum deflection occurs about 0.192 m from the pin and is limited to 0.006672 m.

## Reflection

Considering the rigid handles as beams made the design more realistic because actual materials deform under load. Finding a beam material and cross-section with a searchable moment of inertia was challenging, and the final beam may be unrealistics for a handheld nutcracker. However, the redesign showed how beam deflection, material stiffness, and cross-sectional geometry all affect whether a structure can safely meet a design requirement.
