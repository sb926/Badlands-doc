Badlands
=====
[![DOI](https://zenodo.org/badge/16678/badlands-model/badlands.svg)](https://zenodo.org/badge/latestdoi/16678/badlands-model/badlands)

<div align="center">
    <img width=400 src="https://github.com/badlands-model/Badlands-doc/blob/master/figures/riseofthephoenix.png" alt="Rise of the Phoenix" title="Example of Landscape evolution with Badlands"</img>
</div>

## Overview

**Ba**sin an**d** **Lan**dscape **D**ynamic**s** (**Badlands**) is a parallel TIN-based landscape evolution model, built to simulate topography development at various space and time scales. The model is presently capable of simulating hillslope processes (**linear** diffusion), fluvial incision (*'modified'* **SPL**:  erosion/transport/deposition), spatially and temporally varying geodynamic (horizontal + vertical displacements) and climatic forces which can be used to simulate changes in base level, as well as effects of climate changes or sea-level fluctuations. 

The preferable way to use Badlands is to download the latest official release:
* <a href='https://github.com/badlands-model/badlands/releases'>Badlands v1.0<a/>

The latest Badlands version is the one that’s in our Git repository (our revision-control system). This is only for experienced users who want to try incoming changes and help identify bugs before an official release. Get it using this shell command, which requires Git:
* `git clone https://github.com/badlands-model/badlands.git`

## The specs...

The model is mainly written in fortran and is based on the following characteristics: 
* The finite volume approach from Tucker et al. (2001) based on the dual Delaunay-Voronoi framework is used to solve the continuity equation explicitly, 
* Node ordering is perform efficiently based on the work from Braun & Willett (2013),
* A Hilbert Space-Filling Curve method algorithm (Zoltan) is used to partition the TIN-based surface into subdomains,
* Drainage network partitioning is generated through METIS library. 

## Community driven

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public License along with this program.  If not, see <http://www.gnu.org/licenses/lgpl-3.0.en.html>.

The code is conceived as an open-source project, and is an ideal tool for both **Research** and **Learning** purposes.

### Reporting  

If you come accross a bug or if you need some help compiling or using the code [drop us a line](badlandsmodel@gmail.com).

## Read the doc!

Installation of the code requires several dependencies and it is more than encouraged to go through the <a href='https://cloudstor.aarnet.edu.au/plus/index.php/s/czcs134ykfUTW5F'>manual<a/> at first. 

## Hands-on examples

A compilation of examples can be found in this <a href='https://github.com/badlands-model/Badlands-doc'>Badlands-doc GitHub repository<a/>

| Planar surface with single outlet| Delta evolution under sea-level fluctuations | Climatic forcing on drainage evolution| 
| :-------------: |:-------------:|:-------------:| 
| <a href="http://www.youtube.com/watch?feature=player_embedded&v=lORa_EPs15Y" target="_blank"><img src="http://img.youtube.com/vi/lORa_EPs15Y/0.jpg" alt="Planar surface with single outlet" width="240" height="180" border="10" /></a> | <a href="http://www.youtube.com/watch?feature=player_embedded&v=nX0EDM2-oTc" target="_blank"><img src="http://img.youtube.com/vi/nX0EDM2-oTc/0.jpg" alt="Delta evolution under sea-level fluctuations" width="240" height="180" border="10" /></a> | <a href="http://www.youtube.com/watch?feature=player_embedded&v=2ibm8I1GvT8" target="_blank"><img src="http://img.youtube.com/vi/2ibm8I1GvT8/0.jpg" alt="Climatic forcing on drainage evolution" width="240" height="180" border="10" /></a> |
| execution 30s 2 CPUs |execution 240s 2 CPUs|execution 620s 2 CPUs|

| High-resolution depression filling model | 3D tectonic forcing and drainage evolution| Landscape evolution over continental scale | 
| :-------------: |:-------------:|:-------------:| 
| <a href="http://www.youtube.com/watch?feature=player_embedded&v=R16jZ2VT-ik" target="_blank"><img src="http://img.youtube.com/vi/R16jZ2VT-ik/0.jpg" alt="High-resolution depression filling model" width="240" height="180" border="10" /></a> | <a href="http://www.youtube.com/watch?feature=player_embedded&v=20Z92nnnpQY" target="_blank"><img src="http://img.youtube.com/vi/20Z92nnnpQY/0.jpg" alt="3D Tectonic forcing and drainage evolution" width="240" height="180" border="10" /></a> | <a href="http://www.youtube.com/watch?feature=player_embedded&v=ke2c9Ybb6LM" target="_blank"><img src="http://img.youtube.com/vi/ke2c9Ybb6LM/0.jpg" alt="Landscape evolution over continental scale" width="240" height="180" border="10" /></a> |
| execution 1h 2 CPUs |execution 22h 32 CPUs|execution 4h 16 CPUs|

## Getting the source code

The source code is available on github: <a href='https://github.com/badlands-model/Badlands'>here<a/>

## Stay tuned

News regarding simulations, internships, collaborations and developments associated to Badlands can be found on our [Jekyll Blog](http://badlands-model.github.io).
