.. _elements:

Elements of the H3DTD v2 package
================================

This section provides a brief description of each program in the H3DTD v2 package. In addition, we describe the file formats for all input and supporting files used by the coding library.

Program Library
---------------

The main executable programs within the H3DTD v2 program library are:

    - **h3dtd_v2:** used to forward model TEM data for a conductivity (and a susceptibility) model
    - **h3dtdinv_v2:** used to invert TEM data to recover a conductivity model

Also useful are the following utility programs:

    - **blk3cell:** creates block models directly on tensor meshes

Main Input Files
----------------

Here, we describe the main input files for executables contained with the H3DTD coding package.

.. tOcTree::
    :maxdepth: 1

    Create tensor model <inputfiles/createModel>
    Forward modeling <inputfiles/forward>
    Inversion <inputfiles/inversion>


Supporting Files
----------------

Here, we describe the formats of supporting files used to run H3DTD v2 executable files. The input files for each executable program are described in the :ref:`running the programs<running>` section.

.. toctree::
    :maxdepth: 1

    Locations File <files/surveyFile>
    Time Gates File <files/gatesFile>
    Predicted Data File <files/preFile>
    Observations File <files/obsFile>
    Topography File <files/topoFile>
    Tensor Mesh File <files/tensor_mesh>
    Model File <files/model>
    Weights File <files/weights>
    Wave File <files/waveFile>
    Bounds File <files/bounds>












