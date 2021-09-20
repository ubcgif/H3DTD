.. _example_fwd:

Forward Modeling
================

Here, the code **h3dtd.exe** and the input file **h3dtd.inp** (:ref:`see format <h3dtd_input_fwd>`) are used to forward model TEM data for a synthetic airborne survey. We are interested in the vertical dB/dt response for a coincident loop system. Files relevant to this part of the example are in the sub-folder *fwd*. For this example, we use the model that was created in the example ":ref:`create model<example_model>`". Before running this example, you may want to do the following:

	- `Download and open the zip folder containing the entire H3DTD example <https://github.com/ubcgif/H3DTD/raw/main/assets/h3dtd_example_dbzdt.zip>`__ (if not done already)
	- :ref:`Learn how to run code from command line <h3dtd_fwd>`
	- :ref:`Learn the format of the input file <h3dtd_input_fwd>`

To forward model the data, the following input file was used:

.. figure:: ../inputfiles/images/fwd_input.png
     :align: center
     :width: 700

H3DTD forward models the Cartesian components of the electric field, magnetic field and the time derivative of the magnetic flux density. Below, we show dBz/dt at 0.0001 s, 0.001 s and 0.01 due to step-off excitation.

.. figure:: images/fwd.png
     :align: center
     :width: 700



