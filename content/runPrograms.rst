.. _running:

Running the programs
====================

This section provides describes how to run all executables pertaining to the H3DTD package.

.. note::

    All executable files, input files, output filenames and files specified within input files can be specified in the following manner:

    - as just the filename if contained within the current working directory (Example: *filename.txt*)
    - as a file path relative to the current working directory (Example: *sub_dir\\filename.txt*)
    - as the full path (Example: *C:\\Users\\Name\\Tests\\filename.txt*)

    Executable files should **not** be renamed. However, input file names can be specified by the user if desired.

The main executable programs within the H3DTD program library are:

    - **h3dtd:** used to forward model TEM data for a conductivity (and a susceptibility) model
    - **h3dtdinv:** used to invert TEM data to recover a conductivity model

Also useful are the following utility programs:

    - **blk3cell:** creates block models directly on tensor meshes

Contents
--------

To learn the specifics of running each executable, see the following sections:

  .. toctree::
    :maxdepth: 1

    Creating Tensor Models <programs/createModel>
    Forward Modeling <programs/forward>
    Additional Cell and Face Weights <programs/weightsFiles>
    Inversion <programs/inversion>

