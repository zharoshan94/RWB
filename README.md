# Master thesis

The goal of this master thesis is to provide tools that allow the identification of Rossby wave breaking events by analyzing contour lines of for example potential or absolute vorticity. 

### Contour Extracting algorithm

![ pv_pole](https://user-images.githubusercontent.com/94976842/143453121-2e76e796-274d-4ed9-a120-b5b3181843d3.jpg)


The input of many existing Rossby wave breaking algorithms a (closed) contour line of a certain variable such as PV. In a first step, a contour extracting algorithm based on the "find_contours" function of "measure" by "skimage" was created. The algorithm, written in Python, is provided in a Jupyter Notebook. A first version including a detailed description can be found [here](https://github.com/skaderli/Master_thesis/blob/main/extract_contour_description.ipynb).

### Wave breaking algorithms

Based on the output of the contour extracting algorithm, different wave brekaing algorithms will be implemented. These algorithms are based and inspired by the work of [Wernli and Sprenger (2007)](https://doi.org/10.1175/JAS3912.1) and [Barnes (2012)](https://doi.org/10.1029/2012JD017469).
