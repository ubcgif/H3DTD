.. _example:

Examples
========

dB/dt for Coincident Loop Airborne
----------------------------------

Here, the program libraries for H3DTD will be used to forward model and invert simple airborne TDEM data
for a coincident loop system. In this tutorial, we learn to:

    - create block models on tensor meshes
    - predict TEM data for a synthetic model
    - invert TEM data created using our synthetic model

Zip folders containing all necessary files can be downloaded here:

    - `Standard airborne TDEM example <https://github.com/ubcgif/H3DTD/raw/main/assets/h3dtd_example_dbzdt.zip>`__

The full example is parsed into 3 sections:

.. toctree::
    :maxdepth: 2

    Create tensor model <example_dbdt/create_model>
    Forward modeling <example_dbdt/fwd>
    Inversion <example_dbdt/inv>

