# DIPT_EXP-07
# Edge-Linking-using-Hough-Transform
## NAME : VARUN JC
## REG NO : 21224240179
## AIM:
To write a Python program to detect the lines using Hough Transform.

## SOFTWARE REQUIRED:
Anaconda - Python 3.7

## ALGORITHM:
### Step1:

Import all the necessary modules for the program.
### Step2:

Load a image using imread() from cv2 module.
### Step3:

Convert the image to grayscale.
### Step4:

Using Canny operator from cv2,detect the edges of the image.
### Step5:

Using the HoughLinesP(),detect line co-ordinates for every points in the images.Using For loop,draw the lines on the found co-ordinates.Display the image.


## PROGRAM:

```
DEVELOPED BY : HIBA NASREEN M
REG NO : 212224040117
```
### Input image and grayscale image
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt

gray = cv2.imread('nature.jpg', cv2.IMREAD_GRAYSCALE)
img_color = cv2.imread('nature.jpg', cv2.IMREAD_COLOR)
img_c = cv2.cvtColor(img_color, cv2.COLOR_BGR2RGB)
gray_rgb = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)

gray = cv2.GaussianBlur(gray, (3, 3), 0)
```
```python
plt.figure(figsize=(13, 13))
plt.subplot(1, 2, 1)
plt.imshow(img_c)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(gray_rgb, cmap='gray')
plt.title("Gray Image")
plt.axis("off")
plt.show()
```

### Canny Edge detector output
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt

gray = cv2.imread('nature.jpg', cv2.IMREAD_GRAYSCALE)
img_color = cv2.imread('nature.jpg', cv2.IMREAD_COLOR)
img_c = cv2.cvtColor(img_color, cv2.COLOR_BGR2RGB)
gray_rgb = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)

gray = cv2.GaussianBlur(gray, (3, 3), 0)
```
```python
plt.figure(figsize=(13, 13))
plt.subplot(1, 2, 1)
plt.imshow(img_c)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(gray_rgb, cmap='gray')
plt.title("Gray Image")
plt.axis("off")
plt.show()
```

### Display the result of Hough transform
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
```
```python
gray = cv2.imread('nature.jpg', cv2.IMREAD_GRAYSCALE)
img_color = cv2.imread('nature.jpg', cv2.IMREAD_COLOR)
img_c = cv2.cvtColor(img_color, cv2.COLOR_BGR2RGB)
gray_rgb = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)

gray = cv2.GaussianBlur(gray, (3, 3), 0)
```
```python
plt.figure(figsize=(13, 13))
plt.subplot(1, 2, 1)
plt.imshow(img_c)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(gray_rgb, cmap='gray')
plt.title("Gray Image")
plt.axis("off")
plt.show()
```

## OUTPUT:

### Input image and grayscale image

<img width="1002" height="651" alt="image" src="https://github.com/user-attachments/assets/0407bfac-ac18-43de-834b-faa2f574eb1b" />


### Canny Edge detector output

<img width="387" height="527" alt="image" src="https://github.com/user-attachments/assets/921398d3-3f74-4d6e-90fc-d30d4498da7f" />


### Display the result of Hough transform

<img width="368" height="523" alt="image" src="https://github.com/user-attachments/assets/6243bbcd-bfc0-4df7-a582-da118a170c29" />


## RESULT:

Thus, the image has been successfully converted.
