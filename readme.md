
## GDB raster

Here is an example ESRI Geodatabase (GDB) data source with a raster. 

http://frap.fire.ca.gov/data/frapgisdata-sw-fveg_download

Direct download: http://frap.fire.ca.gov/data/statewide/fveg15_1.zip

This was converted to GeoTIFF using ArcGIS, the resulting files are in **arc-tif/arc_fveg15_1.tif.zip**.  (184Mb)

A selection of the gdalinfo output follows, full output is in **gdalinfo_fveg15_1.tif.txt** (4Mb). 


```
Driver: GTiff/GeoTIFF
Files: fveg15_1.tif
       fveg15_1.tif.ovr
       fveg15_1.tif.aux.xml
Size is 39623, 38094
Coordinate System is:
PROJCS["NAD_1983_California_Teale_Albers",
    GEOGCS["NAD83",
        DATUM["North_American_Datum_1983",
            SPHEROID["GRS 1980",6378137,298.2572221010042,
                AUTHORITY["EPSG","7019"]],
            AUTHORITY["EPSG","6269"]],
        PRIMEM["Greenwich",0],
        UNIT["degree",0.0174532925199433],
        AUTHORITY["EPSG","4269"]],
    PROJECTION["Albers_Conic_Equal_Area"],
    PARAMETER["standard_parallel_1",34],
    PARAMETER["standard_parallel_2",40.5],
    PARAMETER["latitude_of_center",0],
    PARAMETER["longitude_of_center",-120],
    PARAMETER["false_easting",0],
    PARAMETER["false_northing",-4000000],
    UNIT["metre",1,
        AUTHORITY["EPSG","9001"]]]
Origin = (-636269.999999998137355,530310.000000000000000)
Pixel Size = (30.000000000000000,-30.000000000000000)
Metadata:
  AREA_OR_POINT=Area
Image Structure Metadata:
  COMPRESSION=LZW
  INTERLEAVE=BAND
Corner Coordinates:
Upper Left  ( -636270.000,  530310.000) (127d44' 2.84"W, 42d33'31.44"N)
Lower Left  ( -636270.000, -612510.000) (126d44'50.64"W, 32d17'39.60"N)
Upper Right (  552420.000,  530310.000) (113d16'53.19"W, 42d36'58.97"N)
Lower Right (  552420.000, -612510.000) (114d 8'21.71"W, 32d20'40.82"N)
Center      (  -41925.000,  -41100.000) (120d28'32.91"W, 37d38'44.53"N)
Band 1 Block=128x128 Type=Int32, ColorInterp=Gray
  Min=1.000 Max=14352.000 
  Minimum=1.000, Maximum=14352.000, Mean=6561.787, StdDev=4312.845
  NoData Value=2147483647
  Overviews: 19812x19047, 9906x9524, 4953x4762, 2477x2381, 1239x1191, 620x596, 310x298, 155x149
  Metadata:
    STATISTICS_COVARIANCES=18600628.16071996
    STATISTICS_MAXIMUM=14352
    STATISTICS_MEAN=6561.7870424573
    STATISTICS_MINIMUM=1
    STATISTICS_SKIPFACTORX=1
    STATISTICS_SKIPFACTORY=1
    STATISTICS_STDDEV=4312.8445555944
<GDALRasterAttributeTable>
  <FieldDefn index="0">
    <Name>OBJECTID</Name>
...


```

This repos exists in support of https://github.com/r-barnes/ArcRasterRescue/issues/2

