# SIMULATION_PARAMETERS.md
**CFD & Electromagnetic Validation Setup for ORECO v1.4**

## 1. Fluid Dynamics Simulation (CFD)
To validate the passive cooling boost (~15%) and the torque generation, the following boundary conditions are recommended.

### A. Fluid Properties (Standard EV Coolant)
*   **Medium:** Water-Glycol Mixture (50/50).
*   **Density ($\rho$):** $1050 \, \text{kg/m}^3$.
*   **Dynamic Viscosity ($\mu$):** $0.0025 \, \text{Pa}\cdot\text{s}$ (at $40^\circ\text{C}$).
*   **Thermal Conductivity ($\lambda$):** $0.40 \, \text{W/(m}\cdot\text{K)}$.

### B. Boundary Conditions
*   **Inlet Velocity ($v$):** $1.5 \, \text{m/s}$ to $2.5 \, \text{m/s}$ (Standard operational flow).
*   **Turbulence Model:** $k$-$\omega$ SST (Shear Stress Transport) to accurately capture the Dean-vortices and flow separation at the Oloid surface.
*   **Reference Pressure:** $2.5 \, \text{bar}$ (System pressure).

### C. Evaluation Metrics
*   **Nusselt Number ($Nu$):** Comparison between a standard pipe and the ORECO-diffuser section to verify heat transfer enhancement.
*   **Pressure Drop ($\Delta p$):** Maximum allowable $\Delta p < 0.1 \, \text{bar}$ per module at $2.0 \, \text{m/s}$.

## 2. Mechanical & Kinematic Parameters
*   **Pre-Tilt Angle ($\alpha$):** $3^\circ$ (Magnetic offset).
*   **Precession Frequency ($f$):** Target range $10\text{--}20 \, \text{Hz}$.
*   **Moment of Inertia:** To be calculated based on Oloid shell (PEEK) + Internal Sphere (Neodymium).

## 3. Electromagnetic Induction Setup
*   **Coil Topology:** Segmented Toroidal (8 segments).
*   **Magnetic Flux Density ($B$):** Based on N52 Neodymium Sphere ($1.43\text{--}1.48 \, \text{T}$).
*   **Air Gap:** $1.5\text{ mm}$ (Sum of Capsule wall + Annular gap + Housing wall).

---
## 4. Expected Validation Goals
1.  **Self-Starting:** Verification of torque generation at $v = 1.0 \, \text{m/s}$ with $3^\circ$ tilt.
2.  **Thermal Inversion:** Visualization of the "stretching and folding" of fluid filaments (Inversive Kinematics).
3.  **Efficiency:** Ratio of extracted electrical power to hydraulic head loss.
---
[← Back to Overview (README)](./README.md)
