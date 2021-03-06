.. _weightsFile:

Model Weights File
==================

The structure and ordering of the weights file is identical to that of a model file, i.e.:


|
| :math:`w_{1,1,1}`
| :math:`w_{1,1,2}`
| :math:`\;\vdots`
| :math:`w_{1,1,nz}`
| :math:`w_{1,2,1}`
| :math:`\;\vdots`
| :math:`w_{1,nx,nz}`
| :math:`w_{2,1,1}`
| :math:`\;\vdots`
| :math:`w_{i,j,k}`
| :math:`\;\vdots`
| :math:`w_{ny,nx,nz}`
|
|

where :math:`N=nx \times ny \times nz` is the total number of cells in the corresponding tensor mesh. Cells in the x and y directions are organized E to W and S to N, respectively, while cells are organized top to bottom in the vertical. Thus :math:`w_{1,1,1}` is the weight for the top southwesternmost cell and :math:`w_{ny,nx,nz}` is the weight for the bottom northeastermost cell. For sensitivity weighting, only relative values matter. Regions where cells have smaller weights will have more structure. For example, assigning weights of surface cells to a value of unity, and deeper cells to values between 0 and 1 will force structure to occur at greater depths. 

.. note:: Weights for inactive cells, including the air, do not play a role in the solution and so they can be assigned any number.














