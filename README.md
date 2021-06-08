- Hi, I’m Sean Harding, a PhD student at the University of Bristol
- I’m interested in the electronic structure of strongly correlated materials

A brief guide to the repositories listed on this account:

1.) SIAM TB solver
In quantum mechanics we are interested in the solution of eigenvalue problems pertaining to large Hermitian matrices. A given model is described by a matrix called the Hamiltonian, which is often the object of immediate interest. The Hamiltonian is typically too large for conventional methods to be applied to find its eigenvalues. In this package, I have implemented in Python an approach to finding the lowest eigenvalue and associated eigenvector, called the ground state, of a particular problem called the Single Impurity Anderson Model (SIAM). The method works by using physical intuition to identify a basis in which the ground state is 'compact' - that is, has only a small number of large components, and finds these dominant components through an iterative proceedure.

The eigenvectors with eigenvalues close to the ground state describe how a given system responds to a weak external stimulus. The spectral function is a measure of the density of eigenvectors at a given eigenvalue, and is here used as a signature of the ground state calcultion used to assess its accuracy. The function is computed by an expansion on Chebyshev polynomials, and in 'spectral.py' the weight of each polynomial is computed.

2.) Slave boson
The code in SIAM solver relies on a specific choice of basis for the computation of the SIAM spectral function. An important link that I have uncovered in the project is the link between this basis and the results of a class of methods known as slave boson methods. I have here implemented the slave boson method for the SIAM problem in order to improve upon, or understand on a formal level, the basis choice that has been employed in the SIAM solver code.

3.) TIAM solver
The SIAM model is the simplest impurity model that can be constructed. Here, I have extended the code to study the ‘next simplest’ problem, the two-impurity anderson model (TIAM). 

4.) Fluids
This code was written as example code for students undertaking a master’s level research project studying the properties of simple fluids. It computes the phase diagram (under which conditions is the fluid a liquid and which a gas), and density profile of a simple fluid. 

5.) Rocket orbits
This software is an example of using the Runge-Kutta 4th order technique to solve the problem of a rocketship in orbit around the earth and moon, written as example code for an undergraduate computing class that I am a demonstrator for. I have opted here for an object oriented approach, which allows generalization of the problem to include more than one object in motion.
