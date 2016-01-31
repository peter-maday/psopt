# Introduction #

**PSOPT** is an open source optimal control package written in C++ that uses direct collocation methods, which include pseudospectral as well as local discretisations.
These methods solve optimal control problems by approximatimg the time-dependent variables using polynomials, which allows to discretize the differential equations and continuous constraints
over a grid of nodes, and to compute the any integrals associated with the problem using well known quadrature formulas.
Nonlinear programming then is used to find local optimal
solutions. **PSOPT** is able to deal with problems with the following characteristics:


  * Single or multiphase problems

  * Continuous time nonlinear dynamics

  * General endpoint constraints

  * Nonlinear path constraints

  * Integral constraints

  * Interior point constraints

  * Bounds on controls and state variables

  * Delayed differential equations

  * General cost function with Lagrange and Mayer terms.

  * Free or fixed initial and final conditions

  * Linear or nonlinear linkages between phases

  * Fixed or free initial time

  * Fixed or free final time

  * Optimisation of static parameters

  * Parameter estimation based on sampled observations


# Features #
The implementation has the following features:

  * Choice between Legendre, Chebyshev, central differences, trapezoidal and Hermite-Simpson discretizations.

  * Automatic mesh refinement

  * Automatic scaling

  * Automatic differentiation using the [ADOL-C](http://www.math.tu-dresden.de/~adol-c/) library

  * Numerical differentiation by using sparse finite differences

  * Automatic identification of the sparsity pattern of derivative matrices.

  * DAE formulation, so that differential and algebraic constraints can be implemented in the same C++ function.

  * Easy to use interface to GNUplot to produce graphical output.

# Interfaces to NLP solvers #

PSOPT has interfaces to the following NLP solvers:

  * [IPOPT](http://www.coin-or.org/Ipopt/documentation/): an open source C++ implementation of an interior point method for large scale problems.

  * [SNOPT](http://www.sbsi-sol-optimize.com/asp/sol_product_snopt.htm): a well known and widely used proprietary large scale NLP solver.



# Why use PSOPT #

These are some reasons why users may wish to use PSOPT


  * Users who for any reason do not have access to commercial optimal control solvers and wish to employ a free open source package for optimal control which does not need a proprietary software environment to run on.

  * Users who need to link an optimal control solver from a C++ application.

  * Users who want to do research with the software, for instance by implementing their own problems, or by customising the code.


PSOPT does not require a commercial software environment to run on,
or to be compiled. PSOPT been developed under Ubuntu Linux, a free operating system and the GCC compiler. The software has also been ported to compile under Windows 7 using Microsoft Visual Studio 2010.
There is an optional interface to the nonlinear programming solver SNOPT.
Note also that the default NLP solver (IPOPT) requires a sparse linear solver
from a range of options, some of which are available at no cost. The author has personally used the linear solver MA27 (and MC19) from the Harwell Subroutine Library (HSL).

# More Details and Installation Instructions #

Further details about **PSOPT** including detailed installation instructions can be found in its [documentation](http://psopt.googlecode.com/files/PSOPT_Manual_R3.pdf). Also please ensure to read the [post release notes](http://code.google.com/p/psopt/wiki/Post_Release_Notes_3). You may also wish to visit the [PSOPT project home page](https://sites.google.com/a/psopt.org/psopt/Home). You may also wish to join the [PSOPT user's group](http://groups.google.com/group/psopt-users-group).

# How you can help #

You may help improve PSOPT in a number of ways.


  * Sending bug reports.

  * Sending corrections to the documentation.

  * Discussing with the author ways to improve the computational aspects or capabilities  of the software.

  * Sending to the author proposed modifications to the source code, for consideration  to be included in a future release of PSOPT.

  * Sending source code with new examples which may be included (with due acknowledgement) in future releases of PSOPT.

  * If you have had a good experience with PSOPT, tell your students or colleagues about it.

  * Quoting the use of PSOPT in your scientific publications.

# About the author #

[Victor M. Becerra](http://www.personal.reading.ac.uk/~shs99vmb) has been an academic at the School of Systems Engineering, University of Reading, United Kingdom,  since 2000, where he is currently a Reader. He obtained his PhD in optimal control from City University, London. in 1994.

# Contacting the author #
The author is open to discussing with users potential research collaboration
leading to publications, academic exchanges, or joint projects. He can be contacted at his email address: v.m.becerra@ieee.org.