# wrfout metadata overrides

This directory contains files that provide initial metadata information for the WRF `wrfout` hourly model output files.

## wrfout_wordmap.csv
The initial version of this file was auto-generated from a representative WRF model output file using notebooks. 
These initial versions were then updated as necessary to correct errors and improve the metadata descriptions. 
This wordmap is used to provide auto-generated `long_name` information for the metadata. 
The `wrfout_long_name_overrides.txt` file is used to selectively replace the auto-generated `long_name` values when
the automatic process does not provide a meaningful description.

## wrfout_flag_meanings_overrides.txt and wrfout_flag_values_overrides.txt
Flag meanings and values are not part of the original WRF model output files. They provide information about
the expected values and their meanings for select variables in the model output files. The meanings and values
were obtained from the WRF documentation.

## wrfout_long_name_overrides.txt
Sometimes the auto-generated `long_name` for the metadata is not as descriptive as it could be. In these cases this file 
can be used to override the `long_name` value with a more meaningful description.

## wrfout_notes_overrides.txt
Some variables such as `ACLWDNB` do not reflect the actual values without additional computation. The notes override file 
contains additional information about variables like this. The additional information was taken from the 
WRF documentation.

## wrfout_scale_factor_overrides.txt
The original WRF model output provides no `scale_factor` attribute for variables that are scaled. This file provides the 
`scale_factor` information for these variables. The scale factors were obtained from the WRF documentation and model 
output files.

## wrfout_units_overrides.txt
There are a number variables where either incorrect `units` were assigned or used the wrong format. When this
occurs the units override file can be used to correct the `units` attribute. Correct units were obtained from the 
WRF source code and discussions with NCAR staff.

## wrfout_valid_range_overrides.txt
A number of variables in the WRF model output files have a fixed range of values but no attribute was provided
to indicate this. The valid range override file contains the valid range information for these variables. The
information was obtained from the WRF documentation.
