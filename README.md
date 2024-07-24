# Turing-foams

This repository contains supplementary simulation code for the project

**Deciphering the Interface Laws of Turing Mixtures and Foams**

by Henrik Weyer, Tobias Alexander Roth, and Erwin Frey.

The code is ordered with respect to the analyzed reaction--diffusion system:

_multispecies-2cMcRD-PAR_ multispecies mass-conserving reaction--diffusion systems with two components per species; associated with Figs. 1, 2, 3 and Movie 1

_Min-experiment_ Analysis of experimental data of the _E. coli_ Min protein system _in vitro_; associated with Fig.~4 and Data Figs.~1, 2 and Movie 5

_Min-simulation_ Model of the _E. coli_ Min protein system _in vitro_; associated with Figs. 4, 5, 6, and Movies 2, 3, 4

_FIS_ Model of the ferrocyanide--iodate--sulfite reaction; associated with Movie 5

## Comsol simulations
Large-scale simulations of the reaction--diffusion equations are performed in the finite-element software Comsol. Exemplary setup files are provided that contain the settings to perform the simulations in Comsol 6.1.

The simulation results are exported in txt files which are converted to hdf5 files and analyzed in the provided Mathematica notebooks (Comsol2Mathematica2hdf5.nb).

## Mathematica notebooks
The Mathematica notebooks are written for Mathematica version 13.1.
The Mathematica notebooks reference Comsol2Mathematica2hdf5.nb, which is assumed to be in the same folder as the referencing notebook.

Mathematica is used to analyze the Comsol simulations and the experimental data.
Moreover, it is used to perform pseudo-arclength continuation of the two-species PAR reaction--diffusion system. This is done using the implementation provided in the notebook continuation-setup.nb (fbrauns/2cMcRD-coarsening).
