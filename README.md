# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: Karthick P
Register Number: 212222100021
```
### Display the input Image
```python
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'Krishnaraj', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
### Create ths structured element
```python
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```python
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```python
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![create 10](https://github.com/KRISHNARAJ-D/OPENING--AND-CLOSING/assets/119559695/09f5071f-124c-455b-9c9b-a3fa7d71f0ff)


### Display the result of Opening

![open 101 ](https://github.com/KRISHNARAJ-D/OPENING--AND-CLOSING/assets/119559695/9765d8e7-ae01-42ab-8a1a-ea3a3a25171f)

### Display the result of Closing
![close 100 1](https://github.com/KRISHNARAJ-D/OPENING--AND-CLOSING/assets/119559695/815c5f11-b4b9-463d-9c1f-86a4cbad67bc)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
