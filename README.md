# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: Praneet S
Register NO: 212221230078
```
``` Python
# Import the necessary packages
import cv2
import numpy as np



# Create the Text using cv2.putText
img= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'PRANEET S',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()



# Create the structuring element
struct_ele= np.ones((9,9),np.uint8)



# Use Opening operation
opening = cv2.morphologyEx(img,cv2.MORPH_OPEN,struct_ele)
cv2.imshow('Opening',opening)
cv2.waitKey(0)
cv2.destroyAllWindows()




# Use Closing Operation
closing = cv2.morphologyEx(img,cv2.MORPH_CLOSE,struct_ele)
cv2.imshow('Closing',closing)
cv2.waitKey(0)
cv2.destroyAllWindows()




```
## Output:

### Display the input Image
![Screenshot 2023-11-08 084946](https://github.com/Praneet002/OPENING--CLOSING/assets/94308200/e24605f0-2e50-4f7a-91c3-e1deb813d8ee)



### Display the result of the Opening
![Screenshot 2023-11-08 085003](https://github.com/Praneet002/OPENING--CLOSING/assets/94308200/c7c4211e-6864-4aa9-8f0e-b30f7e1b7633)


### Display the result of Closing
![Screenshot 2023-11-08 085022](https://github.com/Praneet002/OPENING--CLOSING/assets/94308200/3dfbc7fc-29b0-443d-a204-2f9b7cd9bfa3)



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
