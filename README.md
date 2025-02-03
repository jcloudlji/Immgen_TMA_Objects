# Immgen_TMA_Objects
An overview of the simplistic approach to creating AnnData objects from the Tissue Microarray.

This script firstly walks through a straightforward method of creating an object in the AnnData format given outputs from the Xenium Prime 5K experiment conducted on the Tissue Microarray (TMA). Additionally, there are steps to subset the TMA to produce AnnData objects for any given region of interest on the panel.

The subsetting portion of the code depends upon the use of the labelme package. If you are running into issues using labelme while running this pipeline remotely, I would recommend installing labelme on your local computer (also using 'pip install labelme'), performing polygon creation in the same manner, and uploading the resulting json file back to your remote directory.

I must note that the subsetting process draws heavily from the Tissue Removal process used for the following paper, just with inverse logic: https://github.com/Goldrathlab/Spatial-TRM-paper.git.
