.. _overview:

Package overview
================

Description
-----------

This manual provides instruction and background for the **H3DTD** program library for the forward modelling and inversion of time domain electromagnetic survey data. The program library provides codes to do the following:

    - Construct models on tensor meshes.
    - Forward model time domain electromagnetic responses to a 3D volume of contrasting conductivity and/or magnetic susceptibility.
    - Invert of surface, borehole and/or airborne EM data to recover 3D conductivity models:

The equations are discretized in time using backward Euler method and discretized in space by using a finite volume technique on a staggered grid. The sources can be grounded dipoles or loop currents that reside in the air, on the surface, or inside the earth. The responses can be any combination of components of E, H, or dB/dt. As of October, 2021, the code is capable of modeling SAM data. The transmitter waveform is user-defined and there are no restrictions on the length or shape of the waveform. Data can be simulated in the “on-time” or “off-time”. The earth model is an arbitrary 3D conductivity defined on a structured rectangular mesh. The earth can also have an arbitrary 3D magnetic susceptibility. The solutions are achieved by factorizing the forward modelling matrix and hence it is possible to simulate data from many sources. This is one of the major benefits of this approach.

The inversion is solved as an optimization problem with the simultaneous goals of (i)
minimizing an objective function dependent on the model and (ii) generating synthetic
data that match observations to within a degree of misfit consistent with the statistics
of those data. To counteract the inherent lack of information, the formulation incorporates reference
model and regularization.

Capacity for the user to directionally weight smoothing and reference model influence
as well as overall influence of regularization on objective function minimization. Explicit
prior information may also take the form of upper and lower bounds on the conductivity
contrast in any cell.

The regularization parameter (controlling relative importance of objective function and
misfit terms). The initial research underlying this program library was funded principally by the mineral industry
consortium “Joint and Cooperative Inversion of Geophysical and Geological Data” (1991 -
1997) which was sponsored by NSERC and the following 11 companies: BHP Minerals, CRA Exploration,
Cominco Exploration, Falconbridge, Hudson Bay Exploration and Development, INCO
Exploration & Technical Services, Kennecott Exploration Company, Newmont Gold Company,
Noranda Exploration, Placer Dome, and WMC.


Program Library Content
-----------------------

The main executable programs within the H3DTD program library are:

    - **h3dtd:** used to forward model TEM data for a conductivity (and a susceptibility) model
    - **h3dtdinv:** used to invert TEM data to recover a conductivity model

Also useful are the following utility programs:

    - **blk3cell:** creates block models directly on tensor meshes

Licensing
---------

Licensing for commercial use is managed by distributors, not by the UBC-GIF research group.
Details are in the `Licensing policy document <http://gif.eos.ubc.ca/software/licensing>`__.


Installing H3DTD
----------------

H3DTD Executables
^^^^^^^^^^^^^^^^^

There is no automatic installer currently available for H3DTD. Please follow the following steps in
order to use the software:

    1. Extract all files provided from the given zip-based archive and place them all together in a new folder.
    2. Add this directory as new path to your environment variables.
    3. Make sure to create a separate directory for each new inversion, where all the associated files will be stored. Do not store anything in the bin directory other than executable applications and Graphical User Interface applications (GUIs).




