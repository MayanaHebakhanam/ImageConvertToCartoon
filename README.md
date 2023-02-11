# ImageConvertToCartoon
This python project illustrates the conversion of given image in to a cartoon.
Library cv2 is used to capture video using OpenCV,designed to solve computer vision problems, NL and Image processing app's.
cv2.imread() Loads an image from specified file.
cv2.cvtColor is used to convert an image from one color space to another.
Second parameter in cv2.medianBlur() indicates size of kernel,Median blur is similar to other averaging methods, processes the edges and removes noise

cv2.adaptiveThreshold:
A global value of threshold was used which remained constant throughout.So, a constant threshold value won’t help in the case of variable lighting conditions in different areas. Adaptive thresholding is the method where the threshold value is calculated for smaller regions.
This leads to different threshold values for different regions with respect to the change in lighting
Syntax: cv2.adaptiveThreshold(source, maxVal, adaptiveMethod, thresholdType, blocksize, constant)
cv2.ADAPTIVE_THRESH_MEAN_C: Threshold Value = (Mean of the neighbourhood area values – constant value). 
In other words, it is the mean of the blockSize×blockSize neighborhood of a point minus constant.
cv2.THRESH_BINARY: If pixel intensity is greater than the set threshold, value set to 255, else set to 0 (black).

A bilateral filter is used for smoothening images and reducing noise, while preserving edges.
parameters:source,Diameter of each pixel neighborhood,sigmaColor,sigmaSpace

Bit-wise conjunction of input array elements.
Masking is a common technique to extract the Region of Interest (ROI).

cv2.waitKey(0):
It takes time in milliseconds as a parameter and waits for the given time to destroy the window,if 0 is passed in the argument it waits till any key is pressed

Python Opencv destroyAllWindows() function allows users to destroy or close all windows at any time after exiting the script

