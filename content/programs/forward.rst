.. _h3dtd_fwd:

Forward Modeling Program
========================

The forward problem is solved using the **h3dtd_v2.exe** executable program and an input file that MUST be name **h3dtd.inp**. To run the executable, open a command window and type the following:

.. figure:: images/run_h3dtd.png
     :align: center
     :width: 500


Units
^^^^^

    - **Electric field data:** *Ex*, *Ey* and *Ez* in units V/m
    - **Magnetic field data:** *Hx*, *Hy* and *Hz* in units A/m. 
    - **Magnetic field data:** *dBx/dt*, *dBy/dt* and *-dBz/dt* in units T/s. The vertical component of dB/dt is represented using -dBz/dt due to a long-standing plotting convention 
    - **SAM data:** The projection of the anomalous H-field along the direction of the Earth's magnetic field in units A/m
    - **Conductivity model:** S/m
    - **Susceptibility model:** SI
    - **Reference/starting conductivity model:** S/m 
    - **Model/interface weights:** unitless



Output Files
^^^^^^^^^^^^

The program **h3dtd_v2.exe** creates the following output files:

    - **recv_h3dtd.txt:** E, H and dB/dt data predicted using H3DTD

    - **h3dtd_v2.log:** A log file for H3DTD

    - **mumps.log:** A log file for the MUMPS solver





