# Obstruction of Absolute Concentration Robustness by Conservation Laws in Non-Redundant Zero-One Networks

This repository contains the code and data accompanying the paper:
"Obstruction of Absolute Concentration Robustness by Conservation Laws in Non-Redundant Zero-One Networks"
by Xinyi Si and Xiaoxian Tang.

1. SOFTWARE REQUIREMENTS
------------------------
- Software: Maplesoft Maple
- Version: Maple 2024 (Compatible with Maple 2020+)
- Platform: Windows 64-bit (Code is platform-independent)

Note: The code relies on symbolic computation capabilities available in Maple 2024. 
While it should work on older versions (e.g., Maple 2020+), specific syntax for polynomial solving or Groebner bases might require minor adjustments.

2. FILE DESCRIPTION & EXECUTION GUIDE
-------------------------------------
The supplementary code consists of three Maple Worksheets (.mw). Please follow the steps below to reproduce the results in the manuscript.

(1) ACR Detection Algorithm (Corresponds to Fig. 2)
File: Algorithm_1.mw
https://github.com/Cynthia-091225/Test-for-ACR/blob/main/Algorithm\_1.mw
Function: Implements the structural verification algorithm to determine if a given network admits Absolute Concentration Robustness (ACR).
Instructions:
- Open the file in Maple.
- Manually input the Stoichiometric Matrix, Reactant Matrix, and the Index of the species to be tested in the designated input section.
- Note: The matrices for all networks analyzed in Fig. 2 are provided in Table_1.mw of the manuscript for your reference.
- Execute the worksheet to obtain the verification result.

(2) Computational Efficiency Analysis (Corresponds to Table 1)
    File: Table_1.mw
    https://github.com/Cynthia-091225/Test-for-ACR/blob/main/Table\_1.mw
    Function: Reproduces the computational performance results presented in Table 1.
    Instructions:
    - Note: Running this file requires the text file for Algorithm_1.mw, which is provided as "Algorithm_1.mpl" along with this file (https://github.com/Cynthia-091225/Test-for-ACR/blob/main/Algorithm\_1.mpl).
    - Run this worksheet to generate the running time statistics for the classification algorithm across different network dimensions.

(3) Positive Steady State Analysis (Corresponds to Table 2)
    File: computation_of_Table_2.mw
    https://github.com/Cynthia-091225/Detect-for-ACR/blob/main/computation_of_Table_2.mw
    Function: Computes the positive steady states for the network topologies listed in Table 2.
    Purpose: These calculations provide numerical evidence supporting the theoretical existence criteria for ACR derived in the paper.
    Instructions:
    -Note: When rerunning  the code, please unassign the definited values for each stoichiometric matrix.
    - Execute the worksheet to view the solved steady state concentrations.

3. COMPUTATIONAL NOTES
----------------------
- Some symbolic computation steps (e.g., computing resultants for high-dimensional networks) may take about 1 minutes depending on your CPU.
- If you encounter memory issues, please increase the kernel memory limit in Maple preferences.

