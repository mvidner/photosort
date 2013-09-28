photosort
=========

Move photos to individual directories according to date taken.

Requirements:

- [exifr](https://github.com/remvee/exifr)

Example
-------

    $ cd /media/SMENA/DCIM/100SMENA
    $ photosort --verbose --target=/data/photos *
    ..............
    /data/photos/2012/2012-11-11
     100_1374.JPG
     100_1375.JPG
     100_1376.JPG
     100_1377.JPG
     100_1378.JPG
     100_1379.JPG
    mkdir -p /data/photos/2012/2012-11-11
    mv 100_1374.JPG 100_1375.JPG 100_1376.JPG 100_1377.JPG 100_1378.JPG 100_1379.JPG /data/photos/2012/2012-11-11
    
    /data/photos/2012/2012-11-17
     100_1380.JPG
     Not moving, too few.
    
    /data/photos/2012/2012-11-30
     100_1381.JPG
     Not moving, too few.
    
    /data/photos/2012/2012-12-22
     100_1382.JPG
     100_1383.JPG
     100_1384.JPG
     100_1385.JPG
     100_1386.JPG
     100_1387.JPG
    mkdir -p /data/photos/2012/2012-12-22
    mv 100_1382.JPG 100_1383.JPG 100_1384.JPG 100_1385.JPG 100_1386.JPG 100_1387.JPG /data/photos/2012/2012-12-22
