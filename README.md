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
![WhatsApp Image 2024-05-07 at 6 07 53 PM (1)](https://github.com/karthickprabakaran/OPENING--AND-CLOSING/assets/166775653/eae08b89-181f-404f-9eba-37b13a42928b)


### Display the result of Opening
![WhatsApp Image 2024-05-07 at 6 07 53 PM (2)](https://github.com/karthickprabakaran/OPENING--AND-CLOSING/assets/166775653/709332e3-9cc0-4a0d-aba9-c911ad8e08a5)

### Display the result of Closing
![WhatsApp Image 2024-05-07 at 6 07 53 PM (3)](https://github.com/karthickprabakaran/OPENING--AND-CLOSING/assets/166775653/717a8b2e-0d8c-41c0-830d-c1fbb2bff4ab)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
