# POPC Membrane Simulation

This project involves the molecular dynamics (MD) simulation of a **POPC membrane** (1-palmitoyl-2-oleoyl-sn-glycero-3-phosphocholine), a common phosphatidylcholine used in membrane studies.

## **Methodology**

### **System Preparation**:
- The membrane system was built using **CHARMM-GUI** to ensure proper lipid arrangement and system setup.
- The system was solvated with a **water box**, and neutralized with **NaCl ions** for stability.
- Input files required for the simulation, including topology and parameter files, were generated using **CHARMM-GUI**.

### **Simulation**:
- **Equilibration**: The system underwent multiple equilibration steps (6.1 to 6.6) to stabilize the membrane environment.
- **Production**: After equilibration, a short production run was performed to gather data for analysis.

### **Visualization**:
- The simulation trajectories were analyzed using **VMD (Visual Molecular Dynamics)**.
- Key metrics such as **area per lipid**, **membrane thickness**, and **deformation** were extracted for interpretation.

## **Results**:

### **1. Area per Lipid Fluctuation**:
The area per lipid fluctuated during the short simulation run, indicating that the system had not yet reached equilibrium. Longer simulations will be required to obtain stable values for this property.

### **2. Membrane Thickness**:
Significant variations in the **membrane thickness** were observed, especially around the phosphorus atoms of the lipid heads. These fluctuations suggest that the system might need more time to stabilize.

### **3. Deformation Dynamics**:
Deformation analysis of the membrane structure revealed how the bilayer responded to the simulated conditions. The membrane exhibited noticeable changes, particularly in its density profile at different time frames.

### **4. Density Profile**:
The density profile at **Frame 1** showed a higher density of lipids, while by **Frame 30**, the membrane had expanded, resulting in lower peaks in the density profile. This suggests that the system was still adjusting to the conditions during the short simulation.

## **Conclusion**:
The POPC membrane simulation provided valuable preliminary insights into the structural dynamics of the lipid bilayer. However, due to the short duration of the production run, more extended simulations are necessary to achieve equilibrium and gather conclusive data. Future studies will focus on longer simulations to stabilize the membrane's structural properties.
