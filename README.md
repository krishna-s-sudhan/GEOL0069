## What is this project?

This repository contains the code and supporting documents used to classify sea ice and leads in remotely sensed altimetry data. We use Machine Learning methods, in particular the Gaussian Mixture Model.

The code is based on a jupyter notebook written by [Weibin Chen](https://www.ucl.ac.uk/earth-sciences/people/research-students/weibin-chen) and [Connor Nelson](https://www.ucl.ac.uk/earth-sciences/people/research-students/connor-nelson) for [Michel Tsamados's](https://www.ucl.ac.uk/earth-sciences/people/academic/dr-michel-tsamados) AI for Earth Observation Module

Gaussian Mixture Models are a machine learning method that use gaussian distributions to classify any number of groups. It works well for scaling. This is an example of it being applied to random data:

![GMM_random](https://github.com/user-attachments/assets/a32303d7-1152-426a-b36f-88a149b67c22)

This model can be applied to image data, but we apply it to data gathered by the Sentinel-3 satelite through its radar altimeter (SRAL). The data was classified and the mean and standard deviation of data in each class were calculated. The results are presented below:

![GMM_SRAL](https://github.com/user-attachments/assets/ee530f8d-4f73-4226-b3e1-766b26709c3f)

As expected, leads produce a sharper, narrower signal, owing to their flatness and high reflectivity. Sea ice on the other hand is rougher, and as a result produces a much more dispersed, spread out signal.
