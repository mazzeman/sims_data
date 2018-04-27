This directory contains data used for unit tests of our Zernike Polynomial
fit to the LSST optical model.

PhoSimData/ and CatSimData/ contain PhoSim-realized and predicted pixel
positions of objects simulated on a grid.  This is to be used when testing the
map between pupil position (which is known in predicted_positions.txt) and final
position on the LSST focal plane.

FullUnitTest/ contains PhoSim data for sources along with the full astrometric
data on those sources (mean position, proper motion, etc.).  This is to be used
when testing the map between astrometric position and final position on the LSST
focal plane.
