# DSHARPVII

This repository contains a tool to find putative planet mass from gap width in mm dust contiuum emission of protoplanetary disks.

## Credit
The fitting method is in [Zhang et al. 2018](https://doi.org/10.3847/2041-8213/aaf744). The method was used to fit DSHARP ([Andrews et al. 2018](https://doi.org/10.3847/2041-8213/aaf744)) samples but it can also be applied to other protoplanetary disks with gaps.

## Notebooks
To infer a planet mass, one needs to [measure the gap width](linearfit/measure_widths.ipynb).


Other quantities such as [aspect ratio h/r](linearfit/claculate_hr.ipynb),
[dust surface density (which is used to infer gas surface density)](linearfit/calculate_sigmad.ipynb), and
the [maximum gas surface density](linearfit/calculate_sigmagGI.ipynb) a disk can have to maintain gravitational instability are aslo needed. Their values can be estimated using these notebooks. If their values are known a priori (e.g., from other observational constraints), one can use [this](linearfit/find_planet_mass.ipynb) to estimate the planet mass. 


In calculating some previous values stellar properties are needed. They can be found in archival papers or relevant catalogs. Radial profiles are needed to measure the gap width and estimate the dust surface density around the gap.


The DSHARP data are public avaiable [here](https://almascience.eso.org/almadata/lp/DSHARP/).


This [notebook](linearfit/automated_DSHARPVII.ipynb) demonstrate the whole procedure. 
