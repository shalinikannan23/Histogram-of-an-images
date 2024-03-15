# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().

### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.

## Program:
### Colour and Gray Image
```python
# Developed By: SHALINI K
# Register Number: 212222240095


import cv2
import matplotlib.pyplot as plt
gray_image = cv2.imread("sea.jpg")
color_image = cv2.imread("grey.jpg",-1)
cv2.imshow("Gray Image",gray_image)
cv2.imshow("Colour Image",color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
### Histogram of Grayscale Image

```py

import numpy as np
import cv2
Gray_image = cv2.imread("grey.jpg")
Color_image = cv2.imread("sea.jpg")
import matplotlib.pyplot as plt
gray_hist = cv2.calcHist([Gray_image],[0],None,[256],[0,256])
color_hist = cv2.calcHist([Color_image],[0],None,[256],[0,256])
plt.figure()
plt.imshow(Gray_image)
plt.show()
plt.title("Histogram")
plt.xlabel("Grayscale Value")
plt.ylabel("Pixel Count")
plt.stem(gray_hist)
plt.show()

```
### Histogram of Green channel of colour Image

```py

plt.imshow(Color_image)
plt.show()
plt.title("Histogram of Color Image - Green Channel")
plt.xlabel("Intensity Value")
plt.ylabel("Pixel Count")
plt.stem(color_hist)
plt.show()
cv2.waitKey(0)
cv2.destroyAllWindows()
  ```


### Histogram Equalization of Grayscale Image

```py

import cv2
gray_image = cv2.imread("sea",0)
cv2.imshow('Grey Scale Image',gray_image)
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:
### Input Grayscale Image and Color Image
![image](https://github.com/shalinikannan23/Histogram-of-an-images/assets/118656529/54ccf726-ceef-438b-9d40-96af6ec094fc)



### Histogram of Grayscale Image

<img height=15% width=48% src="https://github.com/shalinikannan23/Histogram-of-an-images/assets/118656529/118e0518-4965-40e3-ac0c-1452acf91ae8">
<img height=15% width=48% src="https://github.com/shalinikannan23/Histogram-of-an-images/assets/118656529/27df6da9-028b-4bb7-acaa-a3f084627bde">




### Histogram of Green channel of Color Image
<img height=15% width=48% src="https://github.com/shalinikannan23/Histogram-of-an-images/assets/118656529/c8893082-ec01-4b33-8696-8d0ec950fda9">
<img height=15% width=48% src="https://github.com/shalinikannan23/Histogram-of-an-images/assets/118656529/eaa83d4b-60dc-4d71-86da-c2b3f3cf379e">





### Histogram Equalization of Grayscale Image.


![image](https://github.com/shalinikannan23/Histogram-of-an-images/assets/118656529/a356f6d0-00e0-480d-9cd2-7fd84f2c8403)



## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
