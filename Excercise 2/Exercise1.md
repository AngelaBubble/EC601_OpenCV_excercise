# Question 1:
ColorImage.cpp is a program that takes a look at colorspace conversions in
OpenCV. Run the code in ColorImage.cpp and comment on the outputs.
Implement the same thing in Python and save each image.

## Answer:
The outputs are 10 images:

The first image is the orginial image.

The 2nd to the 4th images show the intensity of the colors, red, green and blue, in the orginal image.

The 5th image shows the luma  component of the image.

The 6th and 7th images show The blue-difference and red-difference chroma components of the image.

The 8th image shows the degree to which a stimulus can be described as similar to or different from stimuli

The 9th image shows the saturation of a color which is determined by a combination of light intensity and how much it is distributed across the spectrum of different wavelengths. 

The 10th images shows the brightness of the image.

# Question 2:
Print out the values of the pixel at (20,25) in the RGB, YCbCr and HSV
versions of the image. What are the ranges of pixel values in each channel
of each of the above mentioned colorspaces?

## Answer:
### The value of pixel at (20,25) of Lenna image

```
('RGB [20,25] : ', array([106, 122, 225], dtype=uint8))
('YCbCr [20,25] : ', array([151, 181, 103], dtype=uint8))
('HSV [20,25] : ', array([  4, 135, 225], dtype=uint8))
```

### The ranges of pixel values:
```
RGB: 
R : 0 ~ 255
G : 0 ~ 255
B : 0 ~ 255
```
```
YCbCr with Sub sampling ratio 4:2:0
Luma Y : 16 ~ 235
Chorma Cb : 16 ~ 240
Chorma Cr : 16 ~ 240

YCbCr with Sub sampling ratio 4:4:4
Luma Y : 0 ~ 255
Chorma Cb : 0 ~ 255
Chorma Cr : 0 ~ 255
```
```
HSV:
H : 0 ~ 180
S : 0 ~ 255
V : 0 ~ 255
```
