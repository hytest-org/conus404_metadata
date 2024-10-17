# wrfxtrm_overrides
This directory contains files that provide initial metadata information for the WRF `wrfxtrm` daily model output files.

## wrfxtrm_wordmap.csv
The initial version of this file was auto-generated from a representative WRF model output file using notebooks. 
These initial versions were then updated as necessary to correct errors and improve the metadata descriptions. 
This wordmap is used to provide auto-generated `long_name` information for the metadata. 
The `wrfxtrm_long_name_overrides.txt` file is used to selectively replace the auto-generated `long_name` values when
the automatic process does not provide a meaningful description.

## wrfxtrm_long_name_overrides.txt
Sometimes the auto-generated `long_name` for the metadata is not as descriptive as it could be. In these cases this file 
can be used to override the `long_name` value with a more meaningful description.

## wrfxtrm_units_overrides.txt
There are a number variables where either incorrect `units` were assigned or used the wrong format. When this
occurs the units override file can be used to correct the `units` attribute. Correct units were obtained from the 
WRF source code and discussions with NCAR staff.
