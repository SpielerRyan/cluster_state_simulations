# A Tale of Two Cluster Magnet Simulations
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/19dMEl-0xLvvKI2J9Zaz1RNY8_9QehoEa#scrollTo=Dpm6WASVzIvj)

The cluster magnet is a generalization of the transverse field Ising model that interpolates between a trivial gapped phase and the nontrivial $\mathbb{Z}_2 \times \mathbb{Z}_2$ symmetry protected topological phase (SPT).  Deep in the SPT, the model's ground state is the cluster state, which serves as a resource for measurement based quantum computation.  

This repository probes the phase diagram of the cluster magnet with two different simulations - a variational quantum eigensolver (VQE) and a density matrix renormalization group (DMRG) simulation.  It examines the expectation value of twisted sector "string" order parameter to determine whether the model is in a nontrivial SPT phase. 

---

## Technical Highlights

* **Variational Quantum Eigensolver:** Implements a VQE with ansatz inspired by the circuit that prepares a cluster state.  Extracts expectation value of the string order parameter for a variety of transverse field strengths and plots them to examine phase diagram.
* **Density Matrix Renormalization Group Simulation:** Implements two site DMRG with a matrix product state ansatz.  Extracts expectation value of the string order parameter for a variety of transverse field strengths and plots them to examine phase diagram.  Compares to VQE output, finding the latter to overestimate ground state energy and artificially give a vanishing expectation value for the string order parameter in the disordered phase.

---

## How to Run

This project is completely self-contained and designed to run directly in the cloud via Google Colab. 

1. Click the **Open in Colab** badge at the top of this file.
2. Execute the cells from top to bottom.
