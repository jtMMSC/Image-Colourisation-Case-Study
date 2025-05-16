This repository contains all the MATLAB files and test data used in the MMSC Scientific Computing Case Study (University of Oxford) exploring Reproducing Kernel Hilbert Space (RKHS)-based image colourisation. The algorithm combines spatial and greyscale kernels and is optimised using the Nelder-Mead method (fminsearch) to achieve high-quality colour reconstruction across various image types.


-Test Images/
Contains the four test images used in the case study.

-minimiseE.mlx
Main script used for simulations in Section 4 of the case study. This runs the colourisation algorithm with the combined kernel (spatial + greyscale) and performs optimisation via fminsearch.

-extension_split.mlx
Main script used for simulations in Section 5, isolating and comparing spatial-only and greyscale-only kernels to evaluate the impact of each kernel component independently.

-Error.mlx
Error function for the combined kernel, used in the Nelder-Mead optimisation process.

-Error_greyscale.mlx
Error function used specifically when testing the greyscale-only kernel.

-Error_spatial.mlx
Error function used specifically when testing the spatial-only kernel.

-recolourise.mlx
Core interpolation function for the combined RKHS kernel (spatial + greyscale).

-recolourise_greyscale_only.mlx
Core interpolation function for the greyscale-only RKHS kernel.

-recolourise_spatial_only.mlx
Core interpolation function for the spatial-only RKHS kernel.

-image_colourisation_vJT.mlapp
MATLAB App Designer file for the GUI referenced in Section 4.1. Allows manual point selection and RGB input, enabling user-guided colour input for images with no pre-defined colour information.
