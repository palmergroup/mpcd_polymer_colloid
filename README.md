# mpcd_polymer_colloid

# Multi-particle collision dynamics simulations of polymer and colloid solutions with LAMMPS.
   

Updated: November 16, 2017

SRD_source:  Modified LAMMPS routines for performing multi-particle collision dynamics simulations of polymer and colloid solutions with LAMMPS.  The routines are based on the existing stochastic rotation dynamics (SRD) module in LAMMPS.  The original routines implement the standard SRD scheme and collision rules to handle solvent interactions with large mesoparticles such as colloids.  We have modified these routines to use a momentum conserving Andersen thermostat [MPCD-AT scheme described in Phys. Rev. E 91, 033309 (2015)] instead of the standard SRD algorithm. Additionally, we have implemented a collision scheme in which small mesoparticles (e.g., polymer beads) can exchange momentum with the solvent particles during the thermostatting step, as described in Macromolecules, 50, 8279-8289 (2017).

MPCD input files:   Sample input scripts for performing MPCD simulations of colloids suspended in a semi-dilute solution of bead-spring polymers using the routines in SRD_source. 

LD input files:   Sample input scripts for performing Langevin dynamics (LD) simulations of colloids suspended in a semi-dilute solution of bead-spring polymers using LAMMPS' standard LD integration scheme.  

All codes and input files were tested using lammps-5Nov16 and may need modification to work with other versions. 
