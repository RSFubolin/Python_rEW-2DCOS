# Python_rEW-2DCOS
This file provides the core code of the rEW-2COS method. By integrating reflectance intensity data and spectral morphology data, the recognition ability of this method for sensitive bands is enhanced. Based on the 2DCOS equation, the autocorrelation peak is identified and further correlation elimination is carried out to obtain the sensitive band.
# Getting Started
To set the absolute pathname of input data and output data and running follow these simple example steps.
# Prerequisites
The method is built with Python based on Pycharm. You need some basic Python packages: numpy, pandas, scikit-learn, os, and pywt.
# Input data
We have provided a sample dataset. The file is located in the "data_original" folder. Among the data, 350–2500 represents reflectance, and Target represents the target value. In fact, the input data is not limited to measured vegetation leaf spectra.
# Description
Based on the data (in the "data_original" folder), the spectral reflectance intensity of the continuous wavelet decomposition was obtained via "CWT.py", and the spectral morphological features were calculated using "Morphology.py". The multi-scale spectral reflectance intensity data and spectral morphological data were additively fused. The fused data were then normalized and grouped according to the target values using the K-means method in SPSS software, resulting in the input data for 2DCOS analysis (in the "data" folder). Notably, to save running memory, the example only uses partial data. Subsequently, based on "main.py" and "calculations.py", the synchronous spectral data (in the "result" folder) were generated. We extract the autocorrelation peaks via “Autocorrelation peak.py”. The top 3% autocorrelation peaks of the synchronous spectra were selected and subjected to correlation-based elimination, ultimately identifying the sensitive bands.
This file provides the core code of the rEW-2COS method, which can identify sensitive bands for different vegetation parameters.
# Statement
These codes in this project cannot be used for any commercial purposes without the author's consent.
# Contact
Bolin Fu: fubolin@glut.edu.cn; Yawei ZHU: 1020232080@glut.edu.cn
