  ## Istanbul technical university GEM425E finite element analysis of marine structures final project / Eren Keskintaş
  ## Parametric Ship Midship Section FEM Model (ANSYS APDL)
This repository contains a fully parametric finite element model of a ship midship cross-section, developed using ANSYS APDL. The script automatically generates the structural geometry, assigns sections and materials, and creates the mesh, enabling fast structural modeling and analysis workflows.
  ## Project Overview
The model represents the midship section of a ship hull — one of the most structurally critical regions of a vessel. It includes:
Bottom plating
Inner bottom structure
Side shell regions
Deck plating
Transverse bulkheads
Longitudinal flat bar stiffeners
All structural components are modeled using SHELL181 elements, making the model suitable for global structural analysis, stiffness studies, and FEM-based design investigations.
  ## Fully Parametric Geometry
The geometry is controlled entirely by parameters at the beginning of the APDL script. Changing a few values automatically generates a new structural configuration.
  ## Adjustable Parameters
Parameter	Description
B	Ship breadth
H	Ship depth
Los	Section length
TP	Plate thickness
TW	Stiffener thickness
Nsb	Number of bottom stiffeners (per side)
Nsd	Number of deck stiffeners (per side)
Spacing values	Automatically computed
This allows rapid creation of alternative structural layouts without redrawing geometry.
  ## Stiffener Modeling
All longitudinal stiffeners are modeled as flat bar stiffeners (web-only shell elements). This provides:
Reduced modeling complexity
Efficient meshing
Faster solver performance
The approach is well suited for parametric studies and preliminary ship structural design.
   ## Workbench Integration
The APDL model can be exported as a .cdb file and imported into ANSYS Workbench using the External Model workflow. This enables:
Load and boundary condition definition in Mechanical
Post-processing with Workbench tools
Hybrid APDL–Workbench analysis setups
the script generates an entire family of structures by simply modifying parameters.

## final
This project is part of an ongoing learning and development process in ship structural modeling and parametric FEM design.
Suggestions for improvement, optimization ideas, or structural modeling feedback are highly appreciated. If you have recommendations regarding:
feel free to open an issue or share your thoughts.
<img width="928" height="707" alt="image" src="https://github.com/user-attachments/assets/9658f669-e1a0-48fc-9afe-5ca53e389e8c" />
