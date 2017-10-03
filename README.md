# DataProcessing
Processing steps for eddy covariance tower sites in the Everglades Tower Network:

This code follows the protocol. In r set your working directory to the location of the raw files. There is a separate directory for each file type (Files: MET, TOA, TOB1, HOBO, .ghg). There should be nothing else in these directories.

# Work FLow:

1. Met file development (MET and TOA).
  1a. Concactanate files.
  1b. Format timestamp.
  1c. Add in all missing time periods and remove duplicates.
  1d. Filter all erroneous data.
  
 2. Water Level (MET, HOBO) 
  2a. Pressure file for HOBO.
  2b. Upload Water Level and create dynamic Met file.
 
3. Flux file development (post-edire TOB1)
  1a. Concactanate files.
  1b. Format timestamp.
  1c. Add in all missing time periods and remove duplicates.
  
4. Merge Met, Flux, and Water Level Data
  4a. PAR correction and fill missing par.
  4b. Air temperature correction and fill missing par.
  
5. Pressure correct and gapfill CO2 flux data.

6. Ameriflux format
