# GEOMETRY_OLOID.md
**Mathematical Construction & Parameters for ORECO Core**

---

## 1. The Oloid Definition
The ORECO core is based on the convex hull of two interlocking circles in perpendicular planes, where the center of each circle lies on the edge of the other.

### Core Parameters:
*   **Radius ($R$):** The primary dimension (typically 12mm - 15mm for automotive cooling lines).
*   **Center Distance ($d$):** Fixed at $d = R$.
*   **Surface Area ($A$):** $A = 4\pi R^2$ (Identical to a sphere of the same radius).
*   **Volume ($V$):** $V \approx 3.052418 \cdot R^3$.

---
## 2. Parametric Equations (for CAD Implementation)
To generate the Oloid surface in CAD software (OpenSCAD, Rhino, SolidWorks), use the following segments based on the angle $\phi$:

*   **Segment 1:** $x = R \cos \phi, \quad y = R \sin \phi, \quad z = 0$
*   **Segment 2:** $x = R - R \cos \phi, \quad y = 0, \quad z = R \sin \phi$

The convex hull of these two circles defines the rolling surface.

---
## 3. The 2-5° Magnetic Tilt Integration
In the ORECO V1.4 design, the gimbal suspension is calibrated with a fixed offset $\alpha$:
*   **$\alpha$ (Pre-Tilt):** $3^{\circ}$ (Nominal).
*   **Function:** Ensures the "Angle of Attack" for the incoming fluid stream ($v_{flow}$) is non-zero at $t=0$, initiating immediate torque.

---
## 4. Internal Ball Path
The internal capsule wall must maintain a constant clearance $c$ to the magnetic sphere:
*   **Internal Radius ($r_{int}$):** $R - t_{wall}$ (where $t$ is wall thickness).
*   **Ball Diameter ($D_{ball}$):** $0.7 \cdot (2R - 2t_{wall})$.

---
