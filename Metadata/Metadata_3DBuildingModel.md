# 3-D Building Model
Filename: <br>Geometry Type: raster<br><br>![image](http://www1.nyc.gov/assets/doitt/images/content/pages/3d-buildings.png)

### Table of Contents<br><br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**1. Identification**](#1-identification)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**2. Data Quality and Specifications**](#2-data-quality-and-specifications)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[**3. Attribute Information**](#3-attribute-information)<br><br>
## 1. Identification
---------------------------------------------
|     |     |
| --- | --- |
**Purpose** |3-D Building Models were developed to supplement the most recent [planimetric](https://github.com/ekamptner/nyc-planimetrics/blob/master/Capture_Rules.md) update. Some examples of usage include wind or shadow simulations, urban design, and building volume determination.   <br><br> Examples of NYC 3-D Building Model usage include: <br> [CESIUM (Open Source 3D rendering library)](https://cesiumjs.org/NewYork/index.html?view=-74.01881302800248%2C40.69114333714821%2C753.2406554180401%2C21.27879878293835%2C-21.343905508724625%2C0.0716951918898415)<br> [NY Times Shadow Study](http://www.nytimes.com/interactive/2016/12/21/upshot/Mapping-the-Shadows-of-New-York-City.html)
**Description** |3-D Building Models representing every NYC building present in the 2014 aerial survey. Models are based on a hybrid of Level of Detail (LOD) 1 (simple/prismatic buildings with flat roof detail) and LOD 2 (includes roof structure details).  Highlights of the model include the differentiation of building components including roof, facades, and ground plane. 
**Source(s)** |Department of Information Technology & Telecommunications (DOITT)
**Publication Dates** |**Data**: 04/18/2016<br>**Last Update**: 04/18/2016<br>**Metadata**: 12/28/2016<br>**Update Frequency**: The 3-D model was a one-time capture. Updates and extensions may be considered in the future. 
**Available Formats** |3-D Model data is available in the following formats: <br> [CityGML](http://maps.nyc.gov/download/3dmodel/DA_WISE_GML.zip)<br>[Multipatch]( 
http://maps.nyc.gov/download/3dmodel/DA_WISE_Multipatch.zip)
**Use Limitations** |Open Data policies and restrictions apply. See [Terms of Use](http://www.nyc.gov/html/data/terms.html)
**Access Rights** |Public
**Contact Information** |**Name**: Colin Reilly, Director GIS Division, Department of Information Technology and Telecommunication (DOITT)<br>**Email**: creilly@doitt.nyc.gov
**Links** |https://data.cityofnewyork.us/City-Government/3-D-Building-Model/tnru-abg2
**Tags** |doitt, gis, 3d, buildings, model
## 2. Data Quality and Specifications
---------------------------------------------
|     |     |
| --- | --- |
**Horizontal Coordinate System** |New York State Plane Coordinates, Long Island East Zone, NAD83, US foot
**Resolution** |ASPRS CLASS 1.5 for 1"=100' scale maps
**Spatial Coverage** |New York City, NY
**Temporal Coverage** |Data is based on buildings present in 2014 aerial survey.
**Positional Accuracy** |3-D models are based on the planimetrics building footprint feature class. The horizontal accuracy (XY) of all planimetric feature classes captured is such that 95% of features are within (plus/minus) 1.25 ft of the actual horizontal location. The vertical accuracy (Z) of all planimetric feature classes with elevation values is such that 95% of features captured are within (plus/minus) 1.6 ft of the actual elevation.
**Features Captured** |Permanent structures (e.g. stairwells, towers, etc) with lengths greater than 10' on a side or minimum 100 sq. ft. were captured. Features that are less than 10' but also align with the building planimetric ouline are also included. 
**Features Excluded** |For LOD 1.5 buildings, domes and pitched roofs are not rendered.  All roof appendages, such as chimneys, parapets, spindles, and antenna are also not included. <br><br> For buildings with complex or multiple roof structures, a genearlized collection method was used. Small permanent strucutres (e.g. small towers, elevator shaft, stairs) with less than 10' on a side were not captured. 
**Capture and Update Notes** |3-D building models were created by stereo compilation with SocetSET GXP/Hexagon SSK software. Models are based on 2014 aerial photos and the recent [building footprints](https://github.com/CityOfNewYork/nyc-planimetrics/blob/master/Capture_Rules.md#building-footprint) from the [planimetric](https://github.com/CityOfNewYork/nyc-planimetrics/blob/master/Capture_Rules.md) update. Using the Open Geospatial Consortium's CityGML specification as the basis, the NYC 3-D Building Massing Model was developed to a hybrid specification combining elements from Level of Detail (LOD) 1 and 2. When possible, the elevation attributes (ground elevation and roof height) from the building footprint feature class was used for building base and top data collection to ensure vertical consistency. Since roof elevations from the building feature class are based on the highest point of the roof, there are some differences in elevation for the 3D roof infrastructure that is modeled. <br><br>Approximately 100 iconic buildings were created in LOD 2. <br><br>Building data was converted from DGN/ESRI multipatch file geodatabase formats to CityGML using Safe Software's Feature Manipulation Engine (FME). <br><br> The model was a one-time capture. If the model is useful, future updates and extensions will be considered. 
## 3. Attribute Information
---------------------------------------------
| Attribute | Description | Field Type | Sensitive Field (Y/N) | Notes| 
|------------ | ------------- | -------- | ----------- | ----------|
| BIN | Building identification number. Assigned by City Planning | numeric | No
| DOITT_ID | Unique identifier assigned by DOITT.  | numeric | No
| SOURCE_ID |  | numeric | No