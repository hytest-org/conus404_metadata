# auxhist24_overrides

This directory contains files that provide initial metadata information for the WRF `auxhist24` 15-minute model output files.

## auxhist24_wordmap.csv
The initial version of this file was auto-generated from a representative WRF model output file using notebooks. 
and were then updated as necessary to correct errors and improve the metadata descriptions. 
This wordmap is used to provide auto-generated `long_name` information for the metadata and when the auto-generated
`long_name` is not sufficient, the `auxhist24_long_name_overrides.txt` file is used to selectively replace the 
auto-generated `long_name` with a more meaningful description.

## auxhist24_long_name_overrides.txt
Sometimes the auto-generated `long_name` for the metadata is not as descriptive as it could be. In these cases this file 
can be used to override the `long_name` value with a more meaningful description.

## auxhist24_notes_overrides.txt
The notes attribute is used to provide additional information about a variable that is not provided in the WRF model
output files. This information was obtained from the WRF documentation and source code.

## auxhist24_scale_factor_overrides.txt
The original WRF model output provides no `scale_factor` attribute for variables that are scaled. This file provides the 
`scale_factor` information for these variables. The scale factors were obtained from the WRF documentation and model 
output files.

## auxhist24_units_overrides.txt
There are a number variables where `units` were missing, incorrectly assigned, or used the wrong format. When this
occurs the units override file can be used to correct the `units` attribute. Correct units were obtained from the 
WRF source code and discussions with NCAR staff.
