# Question 1:
Look at Threshold.cpp and implement the code in Python, and observe
the results for different threshold values. Comment on the results.

## Answer:
In adaptive threshold, the algorithm calculate the threshold for a small regions of the image. So we get different thresholds for different regions of the same image and it gives us better results for images with varying illumination.

The band threshold take the upper band and lower band, which only shows limited range of color scalar of the images.

The binary threshold only shows black and white by deviding equally the range of colors.

The semi threshold takes the extreme value from the high value and low value.

# Qeustion 2:
What are the disadvantages of binary threshold?

## Answer:
The binary threshold takes one threshold value for the whole image and resulted in a black and white only. It may not suitable for all kind of image/condition. For example, if an image are concentrated on only certain range of gray scale, then it will show nothing after the binary threshold.

# Question 3:
When is Adaptive Threshold useful?

## Answer:
Adaptive binarization can be divided into three categories:

1) Global method: with this method first of the background of the image is estimated; after that a normalized image is generated with the help of the background information. Then global binarization method is employed.

2) Patch-based method: as the name indicates, patch-based method will perform binarization patch by patch. At each patch, a binarization is estimated with a global binarization method. After that, some post-processing is performed to make sue that binarization threshold in neighboring patches has smooth transition.

3) Moving-window method: with this method, binarization is done pixel by pixel. A moving window is set up to calculate the pixel statistics within the window, and based on the statistics the threshold for the central pixel within the window is calculated.
