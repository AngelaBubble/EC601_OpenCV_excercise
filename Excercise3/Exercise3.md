# Question 1:
Look at the code in Noise.cpp and implement the code in Python. Also,
print the results for different noise values in the Gaussian case, mean =
0, 5, 10, 20 and sigma = 0, 20, 50, 100 and for the salt-and-pepper case,
pa = 0.01, 0.03, 0.05, 0.4 and pb = 0.01, 0.03, 0.05, 0.4.

## Answer:
As the values increasing, there are more noise created.

# Question 2: Change the kernel sizes for all the filters with all different values for noises
and print the results for 3x3, 5x5 and 7x7 kernels. Comment on the results.
Which filter seems to work "better" for images with salt-and-pepper noise
and gaussian noise?

# Answer:
As the kernels sizes increase, the resulting image gets more blur.
I use the Gaussian Noise with mean = 0, sigma = 20 and Salt-and-pepper Noise with pa = 0.01, pb = 0.01 in the kernel changing cases.

## Gaussian Noise
For Gaussian Noise, Gaussian Filter works better

![alt tag](https://raw.githubusercontent.com/WeiXinqiao/EC601_OpenCV_excercise/master/Excercise3/output%20mean%3D0%20sigma%3D20%20pa%3D0.01%20pb%20%3D%200.01/GN_GaussianFilter.png)
![alt tag](https://raw.githubusercontent.com/WeiXinqiao/EC601_OpenCV_excercise/Excercise3/output 5x5/GN_GaussianFilter.png)
![alt tag](https://raw.githubusercontent.com/WeiXinqiao/EC601_OpenCV_excercise/master/Excercise3/output%207x7/GN_GaussianFilter.png)

## Salt-and-Pepper Noise
For Salt-and-Pepper Noise, Median filter works better

![alt tag](https://raw.githubusercontent.com/WeiXinqiao/EC601_OpenCV_excercise/master/Excercise3/output%20mean%3D0%20sigma%3D20%20pa%3D0.01%20pb%20%3D%200.01/SP_MedianFilter.png)
![alt tag](https://raw.githubusercontent.com/WeiXinqiao/EC601_OpenCV_excercise/master/Excercise3/output%205x5/SP_MedianFilter.png)
![alt tag](https://raw.githubusercontent.com/WeiXinqiao/EC601_OpenCV_excercise/master/Excercise3/output%207x7/SP_MedianFilter.png)

