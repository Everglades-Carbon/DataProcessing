# DataProcessing
Processing steps for eddy covariance tower sites:

This code follows the protocol. In r set your working directory to the location of the raw files. There should a separate directory for each file type (Files: MET, TOA, TOB1, HOBO, .ghg). There should be nothing else in these directories.  

## Scripts to build MET files:

1. Always run the timestamp script first. This file produces a timestamp that can be merged with the files to add a timestamp where data is mising. 
2. Run the MET file script.
3. Run the TOA file script.
4. Fill gaps in the pressure data.
5. Process HOBO waterlevel.
6. Import HOBO water level and apply any necessary corrections. 
7. Process TOB1 files in EddyPro. 

## End of the year final files:
1. Gapfill fluxes.
2. Create flux and met files for Ameriflux. 
