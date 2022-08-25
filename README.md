<p align="center">
  <img src="https://user-images.githubusercontent.com/94976842/186669732-8590c915-6812-4a90-b852-ef250d107bf6.jpeg" width=40% height=40%>
</p>

# Rossby Wave Breaking (RWB) detection tool

This Python tool can detect, classify, and track RWB in two-dimensional gridded data. The detection is based on contour lines respresenting the dynamical tropopause. Prefered input variables are Potential Vorticity (PV) or Absolute Vorticity (AV). The algorithm features two different RWB indices: The streamer index developed by [Wernli and Sprenger (2007)](https://doi.org/10.1175/JAS3912.1) and the overturning index developed by [Barnes and Hartmann (2012)](https://doi.org/10.1029/2012JD017469). The algorithm is embedded in a technical consisting of five parts, each including several subroutines. Besides routines that handle the input and output of data, there is the extraction of the contour line, calculation of the RWB indices, and classification (stratospheric, tropospheric, cyclonic, and anticyclonic) of the RWB events.

<p align="center">
  <img src="https://user-images.githubusercontent.com/94976842/186668848-c91327c9-ec74-4314-9732-d26bea41870c.jpg" width=60% height=60%>
</p>

## Contour Extracting algorithm

![ pv_pole](https://user-images.githubusercontent.com/94976842/143453121-2e76e796-274d-4ed9-a120-b5b3181843d3.jpg)

The input of many existing Rossby wave breaking algorithms a (closed) contour line of a certain variable such as PV. In a first step, a contour extracting algorithm based on the "find_contours" function of "measure" by "skimage" was created. The algorithm, written in Python, is provided in a Jupyter Notebook. A first version including a detailed description can be found [here](https://github.com/skaderli/Master_thesis/blob/main/extract_contour_description.ipynb).

