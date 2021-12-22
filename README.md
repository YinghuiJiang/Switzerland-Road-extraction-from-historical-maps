# Switzerland-Road-extraction-from-historical-maps
Project for the course "Foundations of Digital Humanities" contributed by Yinghui Jiang and Irina Serenko.
#### See our [Wiki page](http://fdh.epfl.ch/index.php/Switzerland_Road_extraction_from_historical_maps).

The files in this repository are:
* data - folder with input data for the dhSegment tool, it contains 2 folders: 'images' (contains 60 jpeg patches from different parts of the Dufour map 1000 by 1000 pixels) and 'labels' (contains 60 png binary labels with road annotations for the mentioned patches). Images from this folder were used as a training dataset for dhSegment.
* images_predict - folder with 9 overlapping patches of the Dufour map. These patches represent a small region of Switzerland containing Solothurn. This region was not presented in the training dataset.
* img - folder that contains the results of road segmentation, skeletonization, vectorization and georeferencing for the selected testing dataset:
    1) original_tiff_patch - folder with 9 original tiff patches downloaded from [GeoVITe](https://geovite.ethz.ch). They contain information about the geographic coordinates.
    2) Final_line.dbf
    3) Final_line.points
    4) Final_line.shp
    5) Final_line.shx
    6) Full_image.png - predictions of roads for the region combined from 9 selected patches (Solothurn).
    7) georeferenced_sk.tif - georeferenced vecorized map of predicted roads.
    8) sk_Full_image.png - result after skeletonization of the Full_image.png.
* dhSegment.ipynb.zip - compressed jupyter notebook with the results of road segmentation for images_predict. The code was taken from this [repository](https://github.com/dhlab-epfl/dhSegment-torch) and modified for the purpose of this project

**Notebooks of main coding parts:**
* vectorization.ipynb
* skeletonization.ipynb
* dhSegment.ipynb

**Image files:**
* Final lines
* Ground Control Points
* Skeletonized image
* Georeferenced image
* Image after training
* Original tiff patches 







