.. _h3dtd_fwd:

Forward Modeling Program
========================

The forward problem is solved using the **h3dtd.exe** executable program and an input file that MUST be name **h3dtd.inp**. To run the executable, open a command window and type the following:

.. figure:: images/run_h3dtd.png
     :align: center
     :width: 500

.. Setting Number of Threads with Open MPI
.. ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. Before running the executable, the number of threads used to carry out all simultaneous processes can be set with Open MPI. This is set in the command window **before** running the executable. To set the number of threads (*nThreads* ), use the following syntax:

..     - Windows computer: "set OMP_NUM_THREADS=nThreads"
..     - Linux (bash shell): "export OMP_NUM_THREADS=nThreads"
..     - Linux (csh shell): "setenv OMP_NUM_THREADS nThreads"

.. .. important:: The number of processes (*nFreq* ) times the number of threads (*nThreads* ) **cannot** exceed the total number of threads available from the computer.

Units
^^^^^

    - **Electric field data:** *Ex*, *Ey* and *Ez* in units V/m
    - **Magnetic field data:** *Hx*, *Hy* and *Hz* in units A/m. 
    - **Magnetic field data:** *dBx/dt*, *dBy/dt* and *-dBz/dt* in units T/s. The vertical component of dB/dt is represented using -dBz/dt due to a long-standing plotting convention 
    - **Conductivity model:** S/m
    - **Susceptibility model:** SI
    - **Reference/starting conductivity model:** S/m 
    - **Model/interface weights:** unitless


.. important:: Any combination of data, electric and or magnetic field components, can be be inverted. A specified flag at the start of the observations file can be used to omit columns or individual datums.



Output Files
^^^^^^^^^^^^

The program **h3dtd.exe** creates the following output files:

    - **recv_h3dtd.txt:** E, H and dB/dt data predicted using H3DTD

    - **h3dtd.log:** A log file for H3DTD

    - **mumps.log:** A log file for the MUMPS solver





