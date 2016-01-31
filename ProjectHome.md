**PSOPT** is an open source optimal control package written in C++ that uses direct collocation methods, which include pseudospectral as well as local discretizations. These methods solve optimal control problems by approximatimg the time-dependent variables using polynomials, which allows to discretize the differential equations and continuous constraints over a grid of nodes, and to compute any integrals associated with the problem using well known quadrature formulas.
Nonlinear programming then is used to find local optimal
solutions. **PSOPT** is able to deal with problems with the following characteristics:


  * Single or multiphase problems

  * Continuous time nonlinear dynamics

  * General endpoint constraints

  * Nonlinear path constraints

  * Integral constraints

  * Interior point constraints

  * Bounds on controls and state variables

  * General cost function with Lagrange and Mayer terms.

  * Free or fixed initial and final conditions

  * Linear or nonlinear linkages between phases

  * Fixed or free initial time

  * Fixed or free final time

  * Optimisation of static parameters

  * Parameter estimation based on sampled observations

For further information, see the [Wiki page](http://code.google.com/p/psopt/wiki/Introduction?ts=1242407138&updated=Introduction), visit the [project home page](https://sites.google.com/a/psopt.org/psopt/Home) or download the [software documentation](http://psopt.googlecode.com/files/PSOPT_Manual_R3.pdf).
You can also join the [PSOPT user's group](http://groups.google.com/group/psopt-users-group).

Project logo is courtesy of nasaimages.org