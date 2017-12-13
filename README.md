# ICSM transformation grids

National Transformation version 2 (NTv2) files for transforming between Australian national datums AGD66 / AGD84 and GDA94
	
	AGD66 (EPSG 2D CRS code: 4202) and GDA94 (EPSG 2D CRS code: 4283)
	AGD84 (EPSG 3D CRS code: 4203) and GDA94 (EPSG 2D CRS code: 4283)
	GDA94 (EPSG 2D CRS code: 4283) and GDA2020 (EPSG 2D CRS code: 7844)

To change a coordinate from one datum to another, a mathematical process that models the relationship between coordinates on the two datums is used. This is known as a coordinate transformation. Ideally, this relationship model is defined empirically using common points that have ‘known’ coordinates on the source and target datum. Once defined, the relationship can be applied to transform all other coordinates in a dataset.

Transformation grids provide users of spatial data with a simple and nationally consistent method to transform coordinates between datums and potentially allow for a large number of common points to be used in developing the relationship model.

Australian grids of 2D coordinate shifts are provided in the Canadian National Transformation version 2 (NTv2) format as binary files (.gsb) but software provided by ICSM jurisdictions can readily convert them to ASCII format (.gsa). An in-depth explanation of the format can be found in Appendix C of the "GDAit" User Guide and the GDAit Software Documentation available from [www.dtpli.vic.gov.au/geodesy](www.dtpli.vic.gov.au/geodesy) > Geocentric Datum of Australia 1994 (GDA94) > GDA94 useful tools.

Detailed information on Australian datums and transformations between them is available in the GDA2020 Technical Manual available at [http://www.icsm.gov.au/gda/tech.html](http://www.icsm.gov.au/gda/tech.html) - in particular Chapter 3 and Appendix B describe the transformation methods including background to and area of application of the transformation files.

## Description of the Transformation Grids
### AGD66 <> GDA94

Full national coverage two-way transformation file – see Appendix B in the GDA2020 Technical Manual available at [http://www.icsm.gov.au/gda/tech.html](http://www.icsm.gov.au/gda/tech.html) for details.

| File        | EPSG Transformation Code
|-|-
|`A66_National_13_09_01.gsb`|1803 [AGD66 to GDA94 (11)]
    
	
### AGD84 <> GDA94

Full coverage two-way transformation file in those states that originally adopted AGD84 - West Australia, South Australia, Queensland - see Appendix B in the GDA2020 Technical Manual available at [http://www.icsm.gov.au/gda/tech.html](http://www.icsm.gov.au/gda/tech.html) for details.

| File        | EPSG Transformation Code
|-|-
|`National_84_02_07_01.gsb`|1804 [AGD66 to GDA94 (5)]
	

### GDA94 <> GDA2020
Full national coverage two-way transformation files – See Sections 3.2 and 3.7 in the GDA2020 Technical Manual available at [http://www.icsm.gov.au/gda/tech.html](http://www.icsm.gov.au/gda/tech.html) for details.
Two types of GDA94 – GDA2020 transformation grids have been developed:

•	Conformal: predominantly plate tectonic motion (~1.8 m NNE)

•	Conformal + Distortion: includes regional distortion.

The difference between GDA94 and GDA2020 coordinates is comprised of a conformal transformation component primarily due to plate tectonic motion and an irregular (non-conformal) distortion component. The conformal component accounts for the primary coordinate movement between GDA94 and GDA2020 and replicates a seven-parameter similarity transformation.
The distortion component is attributable to several second-order effects, such as an improved realisation of the global reference frame over time; irregular ground movement since GDA94 was established; and improvements in computation methods since GDA94. These effects vary in magnitude and direction around the country and can be as large as ~0.5 m.
Advice on choosing which grid to use is included in Table 3.4 in in the GDA2020 Technical Manual available at [http://www.icsm.gov.au/gda/tech.html]

| File        | EPSG Transformation Code
|-|-
|GDA94_GDA2020_conformal.gsb|Not yet available
|GDA94_GDA2020_conformal_and_distortion.gsb|Not yet available



## Direct Download of Transformation grids
The transformation grids can be accessed by downloading from this project on GitHub, or as a direct download from a bucket on Amazon's S3 service under the licence terms found in this folder. Direct links to the files are here (for use in production applications):

 * A66_National_13_09_01.gsb: https://s3-ap-southeast-2.amazonaws.com/transformation-grids/A66_National_13_09_01.gsb
 * National_84_02_07_01.gsb: https://s3-ap-southeast-2.amazonaws.com/transformation-grids/National_84_02_07_01.gsb
 * GDA94_GDA2020_conformal.gsb: https://s3-ap-southeast-2.amazonaws.com/transformation-grids/GDA94_GDA2020_conformal.gsb
 * GDA94_GDA2020_conformal_and_distortion.gsb:https://s3-ap-southeast-2.amazonaws.com/transformation-grids/GDA94_GDA2020_conformal_and_distortion.gsb
