# POPC Membrane Simulation

This file involves the molecular dynamics (MD) simulation of a **POPC membrane** (1-palmitoyl-2-oleoyl-sn-glycero-3-phosphocholine), a common phosphatidylcholine used in membrane studies.

## **Methodology**

### **System Preparation**:
- The membrane system was built using **CHARMM-GUI**.
- The system was solvated with a **water box**, and neutralized with **NaCl ions** for stability.
- Input files required for the simulation, including topology and parameter files, were generated using **CHARMM-GUI**.

### **Simulation**:
- **Equilibration**: The system underwent multiple equilibration steps (6.1 to 6.6) to stabilize the membrane environment.
- **Production**: After equilibration, a short production run was performed to gather data for analysis.

### **Visualization**:
- The simulation trajectories were analyzed using **VMD (Visual Molecular Dynamics)**.
- Key metrics such as **area per lipid**, **membrane thickness**, and **deformation** were extracted.

## **Results**:

### **1. Area per Lipid Fluctuation**:
The area per lipid fluctuated during the short simulation run.
<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b06a0c95c696e6de63cfd1dfebd188401fb0f771/POPC%20Bylayer%20Membrane/doc/areaperlipid.jpeg" alt="Area per Lipid Fluctuation" width="400px">
</div>

### **2. Membrane Thickness**:
Significant variations in the **membrane thickness** were observed, especially around the phosphorus atoms of the lipid heads. 
<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b06a0c95c696e6de63cfd1dfebd188401fb0f771/POPC%20Bylayer%20Membrane/doc/membrane_thickness.jpeg" alt="Membrane Thickness" width="400px">
</div>

### **3. Density Profile**:
The density profile at **Frame 1** showed a higher density of lipids, while by **Frame 30**, the membrane had expanded, resulting in lower peaks in the density profile. This suggests that the system was still adjusting to the conditions during the short simulation.
<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b06a0c95c696e6de63cfd1dfebd188401fb0f771/POPC%20Bylayer%20Membrane/doc/density1.jpeg" alt="Density Profile" width="400px">
</div>
<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b06a0c95c696e6de63cfd1dfebd188401fb0f771/POPC%20Bylayer%20Membrane/doc/density30.jpeg" alt="Density Profile" width="400px">
</div>

**Density Profile Tool**:
> Giorgino T. Computing 1-D atomic densities in macromolecular simulations: The density profile tool for VMD. *Computer Physics Communications*. 2014 Jan;185(1):317–22. Available from [doi:10.1016/j.cpc.2013.08.022](https://doi.org/10.1016/j.cpc.2013.08.022) or preprint at [arXiv:1308.5873](https://arxiv.org/abs/1308.5873).


## **Conclusion**:
The POPC membrane simulation provided valuable preliminary insights into the structural dynamics of the lipid bilayer. However, due to the short duration of the production run, more extended simulations are necessary to achieve equilibrium and gather conclusive data. Future studies will focus on longer simulations to stabilize the membrane's structural properties.
