# Finite elements methods for partial differential equations

This thesis presents an interesting approach for numerically solving elliptic
boundary value problems, namely the finite element method (FEM). We first
have a brief look at ordinary differential equations and how to solve them
numerically. This shows by example how numerical solutions are inherently
always approximations of the true solution and the importance of convergence of
such methods. After introducing the basics in this setting, we move on to partial
differential equations (PDEs). First we look at the definition of a PDE and some
examples, as well as a small demonstration of explicitly solving a PDE. Then we
move on to the main subject of the thesis, the numerical treatment of PDEs. As
a preparation step, we introduce the idea of finite difference schemes by example
of the 5-point formula for the Poisson equation. After this we begin our work
towards the finite element method. Before we can talk about the core ideas of
FEM, we first need to establish some mathematical tools that will later enable
us to introduce the weak or integral form of elliptic boundary value problems
(BVP). We make our way towards the Lax-Milgram theorem, which guarantees
that the weak form of an elliptic BVP is a well posed problem. At this point
we can now give the recipe for the finite element method and illustrate its key
concepts with a 1D example. In the last chapter we model airflow around an
aircraft wing via the FEM. Throughout the section the model is developed and a
concrete finite element scheme is derived. After presenting the numerical results
computed with the Python implementation of the scheme, a few error bounds
and estimates are stated. In the appendix the full source code is provided
