Compilation of tests and documentation on the use of Badlands
=====

<div align="center">
    <img width=400 src="https://github.com/badlands-model/Badlands-doc/blob/master/riseofthephoenix.png" alt="Rise of the Phoenix" title="Example of Landscape evolution with Badlands"</img>
</div>

## Overview

**Ba**sin an**d** **lan**dscape **d**ynamic**s** (**Badlands**) is a parallel TIN-based landscape evolution model, built to simulate topography development at various space and time scales. The model is presently capable of simulating hillslope processes such as **linear** & **nonlinear** diffusion, fluvial incision (**detachment-limited** & **under-capacity** laws), spatially varying surface uplift which can be used to simulate changes in base level, as well as effects of climate changes and sea-level fluctuations. 

## The specs...

The model is mainly written in fortran and takes advantage of the Earth Surface Modelling Framework (**ESMF**). 
* The finite volume approach from Tucker et al. (2001) based on the dual Delaunay-Voronoi framework is used to solve the continuity equation explicitly, 
* Node ordering is perform efficiently based on the work from Braun & Willett (2013),
* A Hilbert Space-Filling Curve method algorithm (Zoltan) is used to partition the TIN-based surface into subdomains,
* Drainage network partitioning is generated through METIS library. 

## Community driven

The code is conceived as an open-source project, and is an ideal tool for both **Research** and **Learning** purposes.

## Getting the source code

The source code is available on github: <a href='https://github.com/badlands-model/Badlands'>here<a/>

## Read the doc!

Installation of the code requires several dependencies and it is more than encouraged to go through the <a href='https://github.com/badlands-model/Badlands-doc/blob/master/manual.pdf'>manual<a/> at first. 
