# ICSM transformation grids

National Transformation version 2 (NTv2) files for transforming between Australian national datums AGD66 / AGD84 and GDA94
	
	AGD66 (EPSG CRS code : 4202) and GDA94 (EPSG CRS code : 4283)
	AGD84 (EPSG CRS code : 4203) and GDA94 (EPSG CRS code : 4283)
	
Detailed information on Australian datums and transformation between these datums is available at http://www.icsm.gov.au/gda/tech.html 
in particular Chapter 7 descibes the transformation methods including background to and area of application of the transmformation files (extracts below)

The coordinates of a point will change depending on which datum the coordinates are referred to. 

To change a coordinate from one datum to another, a mathematical process known as transformation is used. This may be done in two or three dimensions and requires a number of points with positions known in terms of both datums ('common' points).  

The accuracy of the transformation depends on the method chosen and the accuracy, number and distribution of the 'common points'. For transforming AGD66 or AGD84 coordinates to GDA94 the NTv2 grid transformation process is the most accurate. For the sake of consistency it is recommended for all transformations in Australia. The files are two way, which means that they may be applied to and from GDA94.


The AGD66/AGD84 to GDA94 transformation grids are files of coordinate shifts that compensate for distortions in the original data, as well as transforming between datums.  

The complex mathematical processing, based on many common points, is done prior to the production of the files of coordinate shifts (Collier, Argeseanu et al. 1998) and the user only has to perform a simple interpolation to obtain the required shifts, followed by a simple addition to perform the transformation.

The files of coordinate shifts are provided in the Canadian format known as National Transformation version 2 (NTv2).

The Australian NTv2 transformation files are provided in the binary format, but software provided by ICSM jurisdictions can readily convert them to ASCII format.

An in-depth explanation of the format can be found in Appendix C of the "GDAit" User Guide and the GDAit Software Documentation available from 
www.dtpli.vic.gov.au/geodesy > Geocentric Datum of Australia 1994 (GDA94) > GDA94 useful tools.
## Transformation files
### AGD66 <> GDA94

Full national coverage two-way transformation file - see http://www.icsm.gov.au/gda/tech.html for details

| File        | EPSG Transformation Code
|-|-
|`A66_National_13_09_01.gsb`|1803 [AGD66 to GDA94 (11)]
    

	A66_National_13_09_01.gsb	EPSG Transformation Code : 1803 [AGD66 to GDA94 (11)]
	
### AGD84 <> GDA94

Full coverage two-way transformation file in those states that origianlly adopted AGD84 - West Australia, South Australia, Queensland see http://www.icsm.gov.au/gda/tech.html for details

| File        | EPSG Transformation Code
|-|-
|`National_84_02_07_01.gsb`|1804 [AGD66 to GDA94 (11)]
	

