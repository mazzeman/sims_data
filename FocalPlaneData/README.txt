This directory contains data used by sims_coordUtils to fit the filter-dependent
component of the FIELD_ANGLE to FOCAL_PLANE coordinate transformation.

The PhoSimData directory contains centroid files from a series of PhoSim runs
done on InstanceCatalogs that differed only in the filter being used.  PhoSim
was run with the following physics commands

clearclouds
backgroundmode 0
cameraconfig 7
opticsonlymode 1
centroidfile 1
rotationjitter 0.0
elevationjitter 0.0
azimuthjitter 0.0
perturbationmode 1

so as to eliminate the effects of atmospheric refraction and physical
perturbations due to the pointing of the telescope.  The PhoSim version used
was 3.7.9

The CatSimData directory contains a text file which includes the
CatSim-predicted positions of the sources from PhoSimData/.
It also contains the InstanceCataog used to generate PhoSimData/.
Note: because the optical model in obs_lsstSim will eventually be updated to
include a better model of refraction through the r filter, only the RA, Dec
columns from this catalog should be used.  These RA, Dec columns are the RA,
Dec directly passed into PhoSim (so: they are "observed" RA, Dec, which
differs from ICRS RA, Dec by terms which represent the motion of the Earth).
