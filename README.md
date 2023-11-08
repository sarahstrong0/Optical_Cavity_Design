## Overview

This lab project involved the design and simulation of a bow-tie optical cavity. Python code was written to compute the optimal parameters for the cavity, considering the constraints imposed by the available laboratory equipment.

## 3.2 Optical Cavities

### 3.2.1 Design a Bow-Tie Cavity

#### Goals Achieved

- Designed the cavity with the provided equipment.
- Ensured the cavity was stable and optimizes the modes of interest.

#### Design Considerations

- **Mirror Angle**: Mirrors  used at a perpendicular angle of incidence. 
- **Cavity Dimensions**: The cavity length exceeds its width for the best angle of incidence.
- **Breadboards**: Used honeycomb breadboards to dampen vibrations, which would significantly affect the performance.
- **Mirror Selection**: Chose from available planar and concave mirrors, considering their back-side polish quality for input/output coupling.
- **Cavity Linewidth**: Opted for a larger free spectral range by making the cavity as short as possible while staying within the stability range.

#### Tasks

(a) Decided on the mirror types and their spacing.  
(b) Used ABCD matrices to ensure the cavity is stable.  
(c) Calculated the cavity waist (`wo`), and its location relative to the input mirror.  
(d) Calculated the cavity's Free Spectral Range (FSR).  
(e) Using the manufacturer’s specifications, calculated the cavity finesse, quality, bounce number, and linewidth.

### 3.2.2 Mode Matching into The Cavity

To maximize the amount of light in the TEM<sub>0,0</sub> mode, 'mode-matching' is crucial. This process involves configuring the input laser beam to match the mode of the optical cavity.

#### Goal Achieved

Designed an optical system, potentially using a two-lens telescope, to match the q-parameter of your beam as closely as possible to the q-parameter of your cavity at the cavity waist.

#### Steps

- Developed Python code to define general ABCD matrices for lenses and free space to propagate your q’s.
- Iteratively tried different lens configurations to approach the optimal solution.

#### Additional Info

- Considered the problem as underconstrained optimization.
- Accounted for the effect of cavity mirrors on the laser beam towards the cavity waist.
- Assumed our laser beam has a waist (`wo`) of 1 mm at a distance of 1 m from the cavity's input mirror.

