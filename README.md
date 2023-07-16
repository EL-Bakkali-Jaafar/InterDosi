 
<b><h2>InterDosi papers</h2> </b> 
1. <p>Jaafar EL Bakkali, Abderrahim Doudouh, Tarek EL Bardouni, Omar Ait Sahel. Monte Carlo calculation of photon specific absorbed fractions in digimouse voxelized phantom using InterDosi code.Radiation Physics and Chemistry, Volume 182, 2021, 109360, ISSN 0969-806X. https://doi.org/10.1016/j.radphyschem.2021.109360 (http://www.sciencedirect.com/science/article/pii/S0969806X21000104)

2. Jaafar EL Bakkali, Abderrahim Doudouh, Tarek EL Bardouni. InterDosi simulations of photon and alpha specific absorbed fractions in zubal voxelized phantom. Applied Radiation and Isotopes,2021,109838,ISSN 0969-8043,https://doi.org/10.1016/j.apradiso.2021.109838. (https://www.sciencedirect.com/science/article/pii/S0969804321002402)
</p>

3. Jaafar El Bakkali, Emily Caffrey, Abderrahim Doudouh.InterDosi Monte Carlo simulations of photon and electron specific absorbed fractions in a voxel-based crab phantom. Radiat Environ Biophys 2021 Oct 17. https://link.springer.com/article/10.1007/s00411-021-00950-6

5. Jaafar EL Bakkali, Khalid Bouyakhlef, Abderrahim Doudouh, Tarek EL Bardouni.
Estimation of electron-specific absorbed fractions with the InterDosi code using ICRP adult female voxel-based phantom,
Applied Radiation and Isotopes,2022,110145,ISSN 0969-8043, https://doi.org/10.1016/j.apradiso.2022.110145.
(https://www.sciencedirect.com/science/article/pii/S0969804322000471)
6. EL Bakkali, J., Doudouh, A., EL Bardouni, T. et al. Intercomparison of S-Factor values calculated in Zubal voxelized phantom for eleven radionuclides commonly used in targeted prostate cancer therapy. Phys Eng Sci Med (2022). https://doi.org/10.1007/s13246-022-01191-7

7. BenDriss, H., Chakir, E., EL Bakkali, J. et al. InterDosi Monte Carlo study of radiation exposure of a reference crab phantom due to radioactive wastewater deposited in marine environment following the Fukushima nuclear accident. Radiat Environ Biophys (2022). https://doi.org/10.1007/s00411-022-00994-2
   
8. EL Bakkali, J., Doudouh, A. Comparison between InterDosi and MCNP in the estimation of photon SAFs on a series of ICRP pediatric voxelized phantoms. Jpn J Radiol (2023). https://doi.org/10.1007/s11604-023-01469-0



<b><h2> About InterDosi</h2> </b> 


![alt text](https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/InterDosi-LOgo.png)is a user-friendly open source code aimed at facilitating the use of Geant4 C++ toolkit for internal dosimetry on voxelized phantoms.
The word InterDosi stands for “Internal Dosimetry”, as its name implies, this code is about of a
Monte Carlo simulation tool especially oriented for performing internal dosimetry studies using
computational human and non-human biota voxel-based phantoms as well as estimating S-values
in spherical tumors of variable radii and chemical compositions. The code uses implicitly Geant4
Monte Carlo toolkit as dose calculation engine known to be the most famous, well-recognized
tool, powerful and widely used around the world for various applications involving the
simulation of ionizing radiation transport and its interaction with the matter.
With knowing that the learning of Geant4 code is not straightforward as the coding with is by
using C++ programming language and requires huge time to learn a such code, this reflects
negatively on the exorbitant effort required to build an advanced application based on the Geant4
C++ toolkit. To deal with this issue, at that point in particular, this open source code has saw the
light in order to provide to scientific researchers whom have a poor knowledge in Geant4/C++
programming, a user-friendly platform allowing them to perform internal dosimetric studies
 using voxelized phantoms as well as using spherical tumor models in an easy manner and in a
very short time too. The code offers a set of useful graphical tools helping user to quasi-
automatically perform all steps required for building a complete internal dosimetry study. The
philosophy of building the InterDosi code was based on the idea of providing an easy-to-use
Geant4-based code dealing without complication with other geometry files written in various file
formats, this through its well-developed converters allow user to import a 3D model of any
existing phantom having a common file format or a well-known structure like as GDML, STL,
OBJ and MCNP hexahedra lattice, and it converts them to a suitable voxel-based phantom file
format recognized by the code, this operation is done into few steps, almost automatically. The
involved dosimetric quantities as Absorbed Fraction (AF) Specific Absorbed Fraction (SAF) can
be calculated in a voxel-based phantom for a given configuration made up of three parameters,
namely: source organ, primary particle type and primary particle energy, this through the GUI
tab “SAFCals”. The code gives to user the opportunity to choice between the most particle types
emitted by radioactive substances used in nuclear medicine, including electron, positron, gamma,
alpha, neutron and proton. In addition, the code allows through the GUI tab “SValueCals”, an
auto calculation of S-values in all organs/regions as results of irradiation of a particular organ by
a selected radio-isotope. It can also be possible to calculate partial S-Value that account for a
specific particle or particle group. In order to speed up the simulation and reduce RAM usage,
parametrized volume approach was used and the G4PhantomParametrisation class was select to
build a parameterized volume representing the voxelized phantom. Additionally, InterDosi
provides a GUI tab “TPGSvalueCals”, a module serving to estimate S-value parameter in a
spherical tumor in which the user is free to set the size and chemical composition. Furthermore,
user can define an array of tumor configurations, each configuration is defined by three
parameters: tumor sphere radius, tumor chemical composition and radionuclide name. The code
allows to user through “VoxGeomVis”` GUI tab the visualization of phantom geometry in two or
three dimensions by implicitly calling Geant4 visualization system. Visualization of internal dose
heatmap for a given voxel-based phantom may be possible either in sagittal, coronal or
transversal view, which give to user a visual idea of how internal absorbed doses are two-
dimensionally distributed in different phantom organs for a particular slice from the phantom
whole volume. The code also includes a tool that allows user to plot SAF and S-value data by
using a data visualization named column chart.

Architecturally, InterDosi is a multithreaded tool that supports parallel calculations feature which
knows to be a good approach to reduce statistical errors associated to scored physics quantities as
well as reducing whole time spent by a given simulation. InterDosi can be run in sequential
mode that is means that one CPU is used, or in parallel mode where a multi-core architecture is
exploited. In order to enhance simulation statistics, a variance reduction technique known as
particle recycling method is also available in which each primary particle is repeated N times
determined.
The present open-source software has been coded by Jaafar EL Bakkali, professor in Nuclear
Physics and associated member to Radiation and Nuclear System Laboratory, U.A.E, Faculty of
Sciences of Tetuan, Morocco and distributed under GPL(General Public License) license.



 Here I provide some screenshots:
![alt text](https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/InterDosi1.20.png)

![alt text](https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/InterDosi-1.2.1.png)

![alt text](https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/InterDosi-1.2.2.png)

![alt text](https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/InterDosi-1.2.png)








<h2> Required dependencies for InterDosi C++ code</h2>
   <p>Geant4 toolkit, version 10.07 --> 11  </p>
   <p>gcc >= 5.4.0</p>
   <p>cmake >= 3.13.2</p>
   <p>HDF5 C++ API >= hdf5-1.10.4</p>
   <p>Valgrind</p>
<h2>Required dependencies for InterDosi.GUI Java-based application
</h2> </b> 
   <p>JRE 8</p>
   
<b><h2> Contribution in the developement of InterDosi open-source code
</h2> </b> 
<p> Anyone can contribute, even if they have a C++/Java programming skills.</p>

<b><h2> For further info</h2> </b> 
<p>Contact:
Jaafar EL Bakkali, at  <a href="mailto:bahmedj@gmail.com">bahmedj@gmail.com</a>  </p>
<h2> License</h2> 
<p>This software is free software; you can redistribute it and / or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version. For the complete text of the license see the GPL-web page.</p>


