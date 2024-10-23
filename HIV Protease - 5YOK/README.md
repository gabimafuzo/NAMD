# HIV-1 Protease Simulation (PDB ID: 5YOK)

<div style="display: flex; justify-content: space-between; align-items: center;">
  <div>
    <img src="https://github.com/gabimafuzo/NAMD/blob/eef890ad992f9ba255e50af4400bad1947774a50/HIV%20Protease%20-%205YOK/proteinacomp.gif" alt="HIV Protease Simulation GIF" width="400px">
  </div>
  <div>
    <img src="https://github.com/gabimafuzo/NAMD/blob/987a7b9b28c0516edb13f9d7413b9b50bf659157/HIV%20Protease%20-%205YOK/doc/prot_img.jpg" alt="HIV Protease Simulation" width="350px">
  </div>
</div>


This repository contains the molecular dynamics (MD) simulation of the **HIV-1 protease** (PDB ID: 5YOK). The project focuses on studying the structural behavior of the HIV-1 protease in a **water solvent with NaCl ions**.

---

## **Key Steps**:
- **Input Generation**: CHARMM-GUI was used to prepare the simulation inputs, including parameter and topology files.

- **Equilibration and Production**: Both steps were conducted using the NAMD software.

- **Visualization**: Results were analyzed using VMD, including trajectory inspection and graph generation.

---

## **Methodology**:

### **System Preparation**:
- The **5YOK** structure was retrieved from the Protein Data Bank.
- The system was solvated in a **water box** and neutralized using **NaCl ions**.
- Input files were generated using **CHARMM-GUI**.

### **Simulation**:
- **Equilibration** and **production phases** were run in **NAMD**.
- The **production run** followed, gathering data for analysis.

### **Visualization**:
- **VMD** was used for visualizing the MD trajectory and generating movies and images.
- Analysis included **RMSD**, bond analysis, and temperature monitoring.

---

## **Results**:

### **1. RMSD Backbone Analysis**
The following plot represents the **RMSD** (Root Mean Square Deviation) of the backbone atoms, indicating structural stability over time:

<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b668d687668c926dec2971f26645039c4ca231fc/HIV%20Protease%20-%205YOK/rmsdvsframe.jpeg" alt="RMSD Backbone Analysis" width="500px">
</div>

---

### **2. Bond vs Time Step (TS) Analysis**
This graph shows the evolution of critical **bonds** over time steps (**TS**), reflecting the structural integrity of the protease:

<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b668d687668c926dec2971f26645039c4ca231fc/HIV%20Protease%20-%205YOK/bondvsts.jpeg" alt="Bond vs Time Step (TS) Analysis" width="500px">
</div>

---

### **3. Temperature and Energy Monitoring (TEM & TEMAVG vs TS)**
The following plot shows **temperature** and **energy** trends during the simulation. Stable temperature and energy profiles indicate a well-equilibrated system:

<div align="left">
  <img src="https://github.com/gabimafuzo/NAMD/blob/b668d687668c926dec2971f26645039c4ca231fc/HIV%20Protease%20-%205YOK/tempvsts.jpeg" alt="Temperature and Energy Monitoring" width="500px">
</div>

---

