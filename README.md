# External-Flow-Over-Truck-Geometry-CFD-Simulation-in-ANSYS-CFX
This repository documents a Computational Fluid Dynamics (CFD) simulation of airflow around a simplified truck model using ANSYS CFX. The analysis focuses on defining the fluid domain, applying appropriate meshing strategies, solver settings, and boundary conditions, and conducting a grid convergence study to validate numerical accuracy.

📄 Project Overview
The simulation explores the flow dynamics surrounding a truck body, focusing on drag prediction, pressure distribution, and wake structure formation. This setup is a foundational case in external aerodynamics and vehicle design evaluation.

🧩 Simulation Pipeline
Fluid Domain Definition
Fluid region sized to minimize boundary effects
Inlet and outlet positioned upstream/downstream of the truck
Symmetry planes used to reduce computational effort
Solid surfaces defined with no-slip conditions

Meshing Strategy
Hybrid mesh: unstructured for complex truck geometry
Boundary layer meshing near surfaces for viscous effects
Local mesh refinement in high-gradient regions (e.g., near the truck rear and wheel arches)
Mesh quality assessed using orthogonality and skewness metrics

CFD Solver Setup
Geometry imported into ANSYS CFX-Pre
Air as the working fluid with ideal gas properties
Turbulence model: SST k-ω or k-ε based on flow conditions
Solver settings include residual-based convergence checks and advanced discretization schemes

Boundary Conditions
Inlet: Velocity or pressure-based (depending on test case), representative of vehicle motion
Outlet: Pressure outlet at ambient conditions
Truck surface: No-slip wall condition

Symmetry: Applied across central plane of the domain
Solver Parameters
Residuals monitored for convergence
Second-order discretization schemes
Segregated solver or coupled AMG approach used for iterative solution
Robust under-relaxation and time step control for numerical stability

📊 Post-Processing & Flow Visualization
Contour plots of pressure, velocity, and turbulence quantities
Vector fields to examine recirculation zones and flow separation
Streamlines and pathlines to trace airflow patterns over and behind the truck
Iso-surfaces used to highlight regions of high vorticity or pressure gradients

📈 Grid Convergence Study
Mesh sensitivity analysis using 2–3 levels of refinement
Drag coefficients and flow features monitored across mesh variations
Error plotted against grid spacing
Ensures that results are mesh-independent and numerically reliable


📄 README.md: Summary documentation

💡 Key Takeaways
Accurate modeling of external vehicle aerodynamics
Importance of boundary layer resolution in drag prediction
Effects of mesh density on simulation fidelity
Understanding of turbulent wake behavior behind bluff bodies

🛠 Tools Used
ANSYS CFX and CFX-Pre
CFD-Post for visualization
Excel/Python for plotting and grid convergence analysis
