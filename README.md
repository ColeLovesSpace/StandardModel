# StandardModel

This program aims to build all the Lagrangian terms built out of the fundamental fields from the symmetry groups and their representations. It is meant to recursevely create every combination and evaluate whether or not the built term respects all of the symmetries of the theory and is renormalizable. 

It begins by creating a curr variable which is a list of all the fields/operators in the current term. It will then loop through all the fields and add each and their respective conjugate or bar and check if it has created a valid term. It will then covariantly differentiate the term using the product rule and see if the new terms it has generated respect the symmetries of the therory. This repeats until the term has too large of a mass dimension to be renormalizable at which point the recursive function returns 0. 


