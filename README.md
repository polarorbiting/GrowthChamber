# GrowthChamber
Goal: Calculate germination rate of potato seeds in trays in a growth chamber environment.
The following has all been done using a combination of multiple programs (Python, ArcGIS, PCI Geomatica) 
but I would now like to automate/batch process using only python. Some steps must still be done in ArcGIS.

1. Camera Calibration (e.g. raspberry pi) 
2. Batch processing:
  a) image distortion removal 
  b) add custom local projection + scale image to make it measureable 
  c) convert jpeg to tiff so that invidivual bands can be accessed 
  d) create indices (e.g. Normalized Excess Green)
  e) create threshold; convert threshold pixels to vector 
  f) convert threshold pixels to vector
3. In ArcGIS:
  a) digitize seed trays in each image
  b) add a field in attribute table for cell # (multiple cells in each tray)
4. Overlay seed tray shapefile with threshold shapefile to get % veg in each cell. 
--> this should populate the field added in 3b -- ??? 
5. Export attribute table with newly populated field to text file



  

