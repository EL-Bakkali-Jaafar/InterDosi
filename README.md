 
<b><h2>InterDosi papers</h2> </b> 
<p>Jaafar EL Bakkali, Abderrahim Doudouh, Tarek EL Bardouni, Omar Ait Sahel. Monte Carlo calculation of photon specific absorbed fractions in digimouse voxelized phantom using InterDosi code.Radiation Physics and Chemistry, Volume 182, 2021, 109360, ISSN 0969-806X. https://doi.org/10.1016/j.radphyschem.2021.109360 (http://www.sciencedirect.com/science/article/pii/S0969806X21000104)

Jaafar EL Bakkali, Abderrahim Doudouh, Tarek EL Bardouni. InterDosi simulations of photon and alpha specific absorbed fractions in zubal voxelized phantom. Applied Radiation and Isotopes,2021,109838,ISSN 0969-8043,https://doi.org/10.1016/j.apradiso.2021.109838. (https://www.sciencedirect.com/science/article/pii/S0969804321002402)
</p>




<b><h2> About InterDosi</h2> </b> 
![alt text](https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/InterDosi-LOgo.png)is a user-friendly open source code aimed at facilitating the use of Geant4 C++ toolkit for internal dosimetry on voxelized phantoms.
 
The word InterDosi stands for “Internal Dosimetry”, as its name implies, this code is about of a Geant-based Monte Carlo modeling tool especially oriented for performing internal dosimetry studies on computational human and non-human biota voxel-based phantoms. Here I provide some screenshots:

With knowing that the learning of Geant4 code is not straightforward as the coding with is by using C++ programming language and requires huge time to learn a such code, this reflects negatively on the exorbitant effort required to build an advanced application based on Geant4 code. To deal with this issue, at that point in particular, this open source code has saw the light in order to provide to scientific researchers whom have a poor knowledge in Geant4/C++ programming, a user-friendly platform allowing them to perform internal dosimetric studies on voxelized phantoms in an easy manner and in a very short time too. The code offers a set of useful graphical tools helping user to quasi-automatically perform all steps required for building a complete internal dosimetry study. Briefly, this tool allows user to import a 3D model of any existing phantom having a common file format or a well-known structure like as GDML, STL, OBJ and MCNP hexahedra lattice, and it converts them to a suitable voxel-based phantom file format regnonized by the code, this operation is done into few steps, almost automatically. The involved dosimetric quantities as specific absorbed fraction and absorbed fraction can be calculated in a voxel-based phantom for a given configuration made up of three parameters, namely: source organ, primary particle type and primary particle energy. The code gives an opportunity to user to choice between the most particle types emitted by radioactive substances used in nuclear medicine, including  electron, positron, gamma, alpha, neutron and proton. In addition, code allows user to visualize phantom geometry in two or three dimensions by implicitly calling Geant4 visualization system. Visualization of internal dose heatmap for a given voxel-based phantom may be possible either in sagittal, coronal or transversal view, which give to user a visual idea of how internal absorbed doses are two-dimensionally distributed in different phantom organs for a particular slice from phantom whole volume. Architecturally, InterDosi is a multi threaded tool that supports parallel calculations feature which knows to be a good approach to reduce statistical errors associated to scored physics quantities as well as reducing whole time spent by a given simulation. InterDosi can be run in sequential mode that is means that one CPU is used, or in parallel mode where a multi-core architecture is exploited. In order to enhance simulation statistics, a variance reduction technique called PNTU (Particle Number of Times of Use) is also available in which each primary particle is repeated for a given times.

The present open-source software has been coded by Jaafar EL Bakkali, Assistant Professor in Nuclear Physics, Rabat-Morocco. Here I provide some screenshots:
![alt text](  https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/Screenshot1png)
<h2> Required dependencies for InterDosi C++ code</h2>https://github.com/EL-Bakkali-Jaafar/InterDosi/blob/master/Screenshot1png
   <p>Geant4 toolkit, version 10.05,10.06 or 10.07  </p>
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


