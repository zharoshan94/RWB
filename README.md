<p align="center">
  <img src="https://user-images.githubusercontent.com/94976842/186669732-8590c915-6812-4a90-b852-ef250d107bf6.jpeg" width=40% height=40%>
</p>

# Rossby Wave Breaking (RWB) detection tool

This Python tool can detect, classify, and track RWB in two-dimensional gridded data. The detection is based on contour lines respresenting the dynamical tropopause. Prefered input variables are Potential Vorticity (PV) or Absolute Vorticity (AV). The algorithm features two different RWB indices: The streamer index developed by [Wernli and Sprenger (2007)](https://doi.org/10.1175/JAS3912.1) and the overturning index developed by [Barnes and Hartmann (2012)](https://doi.org/10.1029/2012JD017469). The algorithm is embedded in a technical consisting of five parts, each including several subroutines. Besides routines that handle the input and output of data, there is the extraction of the contour line, calculation of the RWB indices, and classification (stratospheric, tropospheric, cyclonic, and anticyclonic) of the RWB events. The tool was developed as part of a master thesis at the Oeschger Centre for Climate Change Research at the University of Bern. 

<p align="center">
  <img src="https://user-images.githubusercontent.com/94976842/186668848-c91327c9-ec74-4314-9732-d26bea41870c.jpg" width=60% height=60%>
</p>

## Contour Extracting Algorithm

<p align="center">
  <img src="https://user-images.githubusercontent.com/94976842/186919920-a67625cf-102c-43a6-af1d-2032fcd432b0.png" width=75% height=75%>
</p>

The Rossby wave indices are based on a closed contour line representing the dynamical tropopause. Therefore, we first need to extract a suitable contour line from a two-dimensional field. This algorithm is based on the "find_contours" function of "measure" by "skimage". A first description of the implemented subroutines can be found [here](https://github.com/skaderli/RWB/blob/main/Contour_Extraction_Algorithm.ipynb).

## RWB Index Algorithm

<p align="center">
  <img src="https://user-images.githubusercontent.com/94976842/186933876-44ebe9fa-adb7-41c8-a714-cf45c9a9fbd3.png" width=80% height=80%>
</p>

Calculation of the RWB Indices. 
