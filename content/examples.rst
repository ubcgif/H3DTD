.. _example:

Examples
========

dB/dt for Coincident Loop Airborne
----------------------------------

Here, the program libraries for H3DTD v2 will be used to forward model and transient dB/dt data
for a coincident loop system. In this tutorial, we learn to:

    - create block models on tensor meshes
    - predict TEM data for a synthetic model
    - invert TEM data created using our synthetic model

Zip folders containing all necessary files can be downloaded here:

    - `Standard airborne TDEM example <https://github.com/ubcgif/H3DTD/raw/h3dtd_v2/assets/h3dtd_example_dbzdt.zip>`__

The full example is parsed into 3 sections:

.. toctree::
    :maxdepth: 2

    Create tensor model <example_dbdt/create_model>
    Forward modeling <example_dbdt/fwd>
    Inversion <example_dbdt/inv>


SAM Data for a Large Surface Loop
---------------------------------

Here, the program libraries for H3DTD v2 will be used to forward model and invert SAM data for a large
loop transmitter on the surface. In this tutorial, we learn to:

    - create block models on tensor meshes
    - predict SAM data for a synthetic model
    - invert SAM data created using our synthetic model

Zip folders containing all necessary files can be downloaded here:

    - `Large ground loop SAM example <https://github.com/ubcgif/h3dtd/raw/h3dtd_v2/assets/h3dtd_example_sam.zip>`__

The full example is parsed into 3 sections:

.. toctree::
    :maxdepth: 2

    Create tensor model <example_sam/create_model>
    Forward modeling <example_sam/fwd>
    Inversion <example_sam/inv>

