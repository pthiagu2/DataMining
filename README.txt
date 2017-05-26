File Generated: 02-Feb-2012 01:27:31
Dataset Collection: Colonial Era Weather Archive
Type: TMAX - Monthly
Version: LATEST
Number of Records: 1018
Number of Locations: 1018
Number of Data Points: 336016
Dataset Hash: d4007075d4018cc53e3edc08ca9a3e6a

------------------------------------

This is the dataset description for the "Colonial Era Weather Archive" dataset 
as represented in the Berkeley Earth Surface Temperature Analysis data 
archive.

Colonial Era Weather Archive RAW DATA

This dataset is a representation of the land surface temperature component of 
the Colonial Era Weather Archive.  The official dataset was collected by NOAA’s 
National Climatic Data Center (NCDC; http://www.ncdc.noaa.gov/).

The original data files are not publicly available.

The Berkeley Earth Surface Temperature project imported these reports and 
produced a new representation of the temperature data in the standard format 
used by the Berkeley project.

This dataset should contain all of the air temperature data in the original 
dataset.  It will also contain metadata for station names, locations, and other 
identifiers.  In some cases, the original source may provide additional 
metadata that is not included here.

------------------------------------

Data Formats

The Berkeley project collects temperature data and metadata from a variety of 
sources and attempts to represent it in a common format.  This information is 
primarily managed via a series of customized Matlab classes, and the data and 
source code to use this system has been made available by Berkeley Earth 
(though the proprietary restrictions on Matlab may limit its availability for 
some users).

To accommodate other users and formats, we have designed a system to represent 
all of our information via a series of text files.  The data is distributed 
across a variety of files.  A minimal user wishing to inspect temperature and 
location data will need to examine only two of these files.  However, to 
accommodate advanced users we provide additional files including a variety of 
quality control, sourcing, and additional metadata.

The most important files for new and casual users are highlighted with the 
indicator “***”.


General dataset files:

	***	README.txt: An overview file describing the nature of the dataset and the 
way the data is distributed across other files.  The current file you are 
reading is the README file.

	***	site_detail.txt: An accounting of the metadata associated with each site.  
This file is suitable for most users but omits certain metadata only available 
in the complete file.

		site_complete_detail.txt: Comprehensive collection of site metadata.  This 
file provides all available metadata including historical and conflicting 
values.  In order to represent all of the possible information, the format of 
this data file is the most complicated, and consequently this file is probably 
not of interest to casual data users.

		site_summary.txt: A brief summary file providing geolocation metadata in a 
simple tab delimited format.  This is entirely redundant with the more 
comprehensive site metadata files; however, it is provided as a simple easy to 
use alternative that may be convenient for some users.

		site_flags.txt: A variable length set of integer flags attached to each site 
indicating specifying additional characteristics of the site and the data 
attached to it.

		site_flag_descriptions.txt: Plain text descriptions of the site flags.

		data_flag_descriptions.txt: Plain text descriptions of the per datum flags.

		source_flag_descriptions.txt: Plain text descriptions of the source codes.

		station_changes.txt: A file highlighting the times at which changes in 
station metadata have occurred.

		data_characterization.txt: A file providing summary statistics for each each 
station's record.



Per data type files:

	***	data.txt: File containing the temperature time series associated with this 
dataset.  This file also contains a limited amount of per datum metadata.

		flags.txt: File containing a variable length array of per datum quality 
control, diagnostic, and data history flags.  

		sources.txt: File containing a variable length array of per datum source 
archive indicator flags.
