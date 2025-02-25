# TGA-Desorption-Simulations
This repository contains one of the latest versions of my Molecular Dynamics Code for my PhD Research (specifically, the Desorption version of the simulation). The latest version of the code, as well as all of the different test cases, are stored on the USC CARC Supercomputing Server. These files are just one example of the simulations, specifically the desorption of water-ice off of a gold spacecraft surface at 150 Kelvin, which simulate at reasonable real-world timescales via the PLUMED Plugin which implements Metadynamics with LAMMPS. I also included an example deposition file as well. 

The "SBATCH" slurm job script file allows the code to be run on the terminal via slurm with the USC CARC Supercomputer Clusters. However, if you have LAMMPS installed locally, the "./{LAMMPS FILE NAME}" command should work in order to run the code. However, this code ran on an optimized and customized version of LAMMPS, which included addiitonal libraries for some of the force fields included in the simulation, as well as for PLUMED itself, which many pre-compiled versions of LAMMPS unfortunately don't come with, so you'll also need those in order to run the code. 

Example XYZ Visualization Files are also included and can readily be visualized in OVITO (an MD visualization software), Paraview, or a number of any other visualizaiton software which can read xyz files with timestamps and atomic positions. 

<img width="767" alt="Deposition Visualization" src="https://github.com/user-attachments/assets/d6abbf49-832b-4d1d-b50e-969857f72d13" />

<img width="763" alt="Desorption Visualization Example" src="https://github.com/user-attachments/assets/81d0eb9a-64ad-4c01-a458-0b79f93cf1f0" />
