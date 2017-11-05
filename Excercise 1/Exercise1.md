# Question 1:
How does a program read the cvMat object, in particular, what is the
order of the pixel structure?

# Answer:
Matrix elements are stored row by row. Element (i, j) (i - 0-based row index, j - 0-based column index) of a matrix can be retrieved or modified using CV_MAT_ELEM macro:

```
uchar pixval = CV_MAT_ELEM(grayimg, uchar, i, j)
CV_MAT_ELEM(cameraMatrix, float, 0, 2) = image.width*0.5f;
```
To access multiple-channel matrices, you can use CV_MAT_ELEM(matrix, type, i, j*nchannels + channel_idx).

The order of the pixel structure is:

For gray scale image:
![alt text](https://docs.opencv.org/2.4/_images/math/146857cf7bb2f26ce5ef0b4ddff686cf6f945204.png)

For RGB image:
![alt text](https://docs.opencv.org/2.4/_images/math/b6df115410caafea291ceb011f19cc4a19ae6c2c.png)
