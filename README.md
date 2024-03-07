# Histogram-of-an-images
&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;**
DATE: 07.03.2024
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;Developed By:SHALINI.K
### Step2:
Print the image using imshow().&emsp;&emsp;&emsp;&emsp;&emsp;Register Number: 212222240095
### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.
### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.
### Step5:
The Histogram of gray scale image and color image is shown.

## Program:

```python
# Developed By: SHALINI.K
# Register Number: 212222240095
```
### COLOR AND GRAY IMAGE:

```python
import cv2
import matplotlib.pyplot as plt
gray_image = cv2.imread("Gray_Mustang.jpg")
color_image = cv2.imread("Mustang.jpg",-1)
cv2.imshow("Gray Image",gray_image)
cv2.imshow("Colour Image",color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
### OUTPUT:


  </td>
  <td>

   </td>
  </tr>



  <tr>
    <td width=50%>







```
## Output:
### Input Grayscale Image and Color Image


### Histogram of Grayscale Image and any channel of Color Image



### Histogram Equalization of Grayscale Image.




## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
