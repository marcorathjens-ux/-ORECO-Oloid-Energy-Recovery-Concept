Technical Design & Prototyping Specifications for ORECO v1.4
1. Dimensional Constraints
To ensure seamless integration into existing EV cooling circuits (e.g., Tesla Model 3 / VW ID.4), dimensions are based on automotive standard hose connectors.
Interface Diameter (ID): 19mm / 25mm (Standard SAE J2044).
Total Housing Length: 120mm - 150mm (including diffuser transitions).
Max Outer Diameter: 60mm (at the widest point of the diffuser).
2. Component Design (3-Layer Architecture)
Layer 1: Outer Housing (Diffuser)
Geometry: Bi-directional diffuser with a 7° opening angle to prevent flow separation.
Features: Integrated winding chambers for toroidal coils and slots for Mu-metal shielding.
Material: PEEK or PPS-GF40 (high-temp resistant, coolant-proof, non-magnetic).
Layer 2: Inner Oloid-Core (Capsule)
Geometry: Mathematically precise oloid profile (based on two circles with radius 
 and center distance 
).
Wall Thickness: 0.8mm - 1.2mm (optimized for magnetic induction vs. 2.5 bar system pressure).
Sealing: Friction welding or laser welding after sphere insertion.
Layer 3: Actuator (The Ball)
Type: Neodymium Magnet (N52) with Ceramic Coating (Si3N4).
Diameter: 8mm - 10mm (occupying ~60-70% of the inner oloid cross-section for optimal momentum).
3. Tolerances & Clearances
Annular Gap (Flow Path): 3mm - 5mm between oloid core and housing wall (balancing torque vs. pressure drop).
Bearing Tolerance: < 0.1mm at polar pivot points to minimize mechanical noise and vibration.
4. Prototyping Strategy (3D Printing)
Method: SLS (Selective Laser Sintering) for structural integrity or SLA for smooth internal surfaces.
Material: PA12 (Nylon) or high-temp resins, epoxy-coated for liquid-tight sealing.
