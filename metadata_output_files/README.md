# metadata_output_files

These are the final versions of the metadata output files for the CONUS404 model.

- wrfout_metadata.csv contains metadata for the variables in the WRF hourly model output files
- auxhist24_metadata.csv contains metadata for the variables in the WRF 15-minute model output files
- wrfxtrm_metadata.csv contains metadata for the variables in the WRF daily model output files

NOTE: The wrfout metadata file has been manually updated to fix errors in the description metadata 
for ACRUNSB and ACRUNSF that is not handled by the automated workflows. Generally the description variable 
values from the model output is left as-is to reflect the original WRF format. In some cases this may result
in confusing, incomplete, or incorrect descriptions. The wrfout metadata file is the most complete and accurate
representation of the model output metadata.
