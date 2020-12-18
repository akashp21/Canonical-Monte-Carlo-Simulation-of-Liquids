# Canonical-Monte-Carlo-Simulation-of-Liquids
A Monte Carlo simulation approach to model the self-assembly of particles in a liquid. 

Chemistry 404 Project

By Owen Kwok, Akash Panjabi and Sofia Mohamed

For our project, we decided to delve into the self-assembly of particles in a liquid. Our goal was to simulate stable, self-assembled states of a 
two-particle system using the Monte Carlo method and the Metropolis method as a propagation mechanism. The Metropolis Monte Carlo method generates 
trajectories in phase space that then samples from a chosen statistical ensemble. As for our computations, we have decided to sample from the canonical 
ensemble, where the number of atoms, the temperature and the volume are held constant. Further, in our system, the atom interactions are based off of the 
Lennard-Jones potential. Though, to make matters far simpler, we decided to use the reduced units. 


How to operate the code:

Begin by downloading the notebook file (ipynb) and uploading it to python. Create a new directory with the code in it, as this will help keep all of the files
generated in the same place. Note, if using the UBC provided platform syzygy, the code will not work as effectively. It is better to run the program using Jupyter on a 
local host.

1. Run Cell 1 and cell 2
2. Adjust initial parameters : n_atoms, T, rho, type2atoms(for V2), a, b, c, d, runs
   In line 30 in V1 (line 34 for V2), change how_to_initialize = “___” to your desired initialization parameters

	“lattice”
	Starting point. Generates lattice for simulation.

	“equilibrating”
	Resets trajectory at the last frame in the previous run, maintains the value of the maximum change in distance of the atoms. Used for equilibrating your simulation.

	“restart”
	Extend your trajectory file for more data.

3. Run cell 3 to start simulation

4. Run cell 4 to start analysis

5. Run cell 5 for thermodynamic quantities and averages+variance

6. Run cell 6 for pressure graph

7. Run cell 7 for potential energy graph

8. Run cell 8 for translational order parameter graph

9. Run cell 9 for radial distribution graph
