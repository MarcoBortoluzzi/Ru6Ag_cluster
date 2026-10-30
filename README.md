# Ru6Ag_cluster
DFT calculations and AIM analysis on [AgRu6(CO)22]-

Marco Bortoluzzi, markos@unive.it

Università Ca’ Foscari Venezia, Via Torino 155, 30172 Mestre (VE), Italy

The excerise is taken from the data published in reference [1]. The structure of the heterometallic cluster [AgRu6(CO)22]- was optimized with DFT calculations using the PBEh-3c method [2]. The compound has 104 valence electrons, and according to the EAN (effective atomic number) it should have 11 metal-metal bonds.

The minimal input file (Ru6Ag.inp) was tested with ORCA 6, Linux version [3]. The calculation took less than 4 minutes on a desktop PC with 16-core AMD processor and 64 GByte RAM. The input can be edited to change the number of cores and the RAM available for each core. The software can be downloaded at https://orcaforum.kofo.mpg.de/.
If ORCA is installed in the ~/orca6 folder, the calculation can be launched from a terminal opened in the folder containing the input file: ~/orca6/orca Ru6Ag.inp > Ru6Ag.out

Once finished the calculation, a file in .molden format can be generated with the command: ~/orca6/orca_2mkl Ru6Ag -molden. The file generated must be renamed from Ru6Ag.molden.input to Ru6Ag.molden.
The file can be opened with Multiwfn 3.8, Linux version [4], available at http://sobereva.com/multiwfn/download.html. Once opened the Ru6Ag.molden file, the AIM analysis can be carried out by typing 2, then  2, 3 and 4. To visualize the structure and the critical points (Cp) type 0. Limit the visualization for clarity to the (3,-1) critical points and visualize the Cp labels. The numer of (3,-1) metal-metal critical points should agree with the EAN model. 
Annotate the Cp labels for the four Ru-Ag and the seven Ru-Ru bonds. Exit from the graphical interface and type 7 followed by the Cp number. Annotate the values relative to the electron density, potential energy density, energy density and Laplacian of electron density. Repeat the procedure for the 11 metal-metal (3,-1) critical points. Compare the values with those reported in reference [1]. Are the values in line with Bianchi’s definition [5] of metal-metal bonds? Finally, propose the strongest Ag-Ru and Ru-Ru bonds on the basis of the density and potential energy density values at critical points.

[1] C. Cesari, M. Bortoluzzi, F. Forti, L. Gubbels, C. Femoni, M.C. Iapalucci, S. Zacchini. 2-D Molecular Alloy Ru−M (M = Cu, Ag, and Au) Carbonyl Clusters: Synthesis, Molecular Structure,Catalysis, and Computational Studies. Inorg. Chem. 61 (2022) 14726-14741. https://doi.org/10.1021/acs.inorgchem.2c02099

[2] S. Grimme, J.G. Brandenburg, C. Bannwarth, A. Hansen. Consistent structures and interactions by density functional theory with small atomic orbital basis sets. J. Chem. Phys. 143 (2015) 054107. https://doi.org/10.1063/1.4927476

[3] F. Neese. Software Update: The ORCA Program System—Version 6.0. Wiley Interdiscip. Rev.: Comput. Mol. Sci. 15 (2025) e70019. https://doi.org/10.1002/wcms.70019

[4] T. Lu. A comprehensive electron wavefunction analysis toolbox for chemists, Multiwfn. J. Chem. Phys. 161 (2024) 082503. https://doi.org/10.1063/5.0216272

[5] C. Lepetit, P. Fau, K. Fajerwerg, M.L. Kahn, B. Silvi. Topological analysis of the metal-metal bond: A tutorial review. Coord. Chem. Rev. 345 (2017) 150-181. https://doi.org/10.1016/j.ccr.2017.04.009
