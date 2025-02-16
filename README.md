## What is this project?

This repository contains the code and supporting documents used to classify sea ice and leads in remotely sensed altimetry data. We use Machine Learning methods, in particular the Gaussian Mixture Model.

The code is based on a jupyter notebook written by [Weibin Chen](https://www.ucl.ac.uk/earth-sciences/people/research-students/weibin-chen) and [Connor Nelson](https://www.ucl.ac.uk/earth-sciences/people/research-students/connor-nelson) for [Michel Tsamados's](https://www.ucl.ac.uk/earth-sciences/people/academic/dr-michel-tsamados) AI for Earth Observation Module

Gaussian Mixture Models are a machine learning method that use gaussian distributions to classify any number of groups. It works well for scaling. This is an example of it being applied to random data:

![GMM_random](https://github.com/user-attachments/assets/a32303d7-1152-426a-b36f-88a149b67c22)

This model can be applied to image data, but we apply it to data gathered by the Sentinel-3 satelite through its radar altimeter (SRAL). The data was classified and the mean and standard deviation of data in each class were calculated. The results are presented below:

![GMM_SRAL](https://github.com/user-attachments/assets/ee530f8d-4f73-4226-b3e1-766b26709c3f)

As expected, leads produce a sharper, narrower signal, owing to their flatness and high reflectivity. Sea ice on the other hand is rougher, and as a result produces a much more dispersed, spread out signal.

We go on to produce a plot of all the signals in both classes, and in each seperate class. As well as producing scatter plots to compare their peakiness, sigma-0 values and standard deviation.

Finally we produce a confusion matrix to show the success of our classificiations.

![GMM_matrix](https://github.com/user-attachments/assets/a81b3374-3960-44e3-a0e9-b9f76a8179b1)

I hope you find this repository and the code useful, and a thanks to Weibin, Connor and Michel for producing the first jupyter notebook I used as reference.

## Contact

* krishna.sudhan.22@ucl.ac.uk
* This Project: https://github.com/krishna-s-sudhan/GEOL0069/

## Resources

* [Using GMMs in Python using Sci-kit Learn](https://scikit-learn.org/stable/modules/mixture.html)
* [The Copernicus Browser that can be used to access Sentinel-3 data](https://browser.dataspace.copernicus.eu/)


