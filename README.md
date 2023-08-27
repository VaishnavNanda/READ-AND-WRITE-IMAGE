# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:JEEVAGOWTHAM S
### Register Number: 212222230053 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('123.jpg',1)
cv2.imshow('212222230053_jeeva',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```

import cv2
color_img=cv2.imread('123.jpg',1)
w= cv2.imwrite('0.png',color_img)
cv2.imshow('0',color_img)
cv2.waitKey(0)




```
iii) #Find the shape of the Image
```python3
import cv2
import random
color_img=cv2.imread('123.jpg',1)
print(color_img.shape)


```
iv) #To access rows and columns

```python3
import cv2
import random
color_img=cv2.imread('123.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230053_jeeva',color_img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```python3
import cv2
color_image=cv2.imread('123.jpg',1)
tag=color_image[20:80,20:80]
color_image[90:150,90:150]=tag
cv2.imshow("212222230053_JEEVA",color_image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image
![Screenshot 2023-08-23 090658](https://github.com/JeevaGowtham-S/READ-AND-WRITE-IMAGE/assets/118042624/f9db3c0b-f59f-46bf-9006-f672234e1398)

<br>
<br>

### ii)Write the image:
![Screenshot 2023-08-23 094610](https://github.com/JeevaGowtham-S/READ-AND-WRITE-IMAGE/assets/118042624/fe8d433f-e606-4786-a14a-55f13c137728)



<br>
<br>

### iii)Shape of the Image
![Screenshot 2023-08-23 091820](https://github.com/JeevaGowtham-S/READ-AND-WRITE-IMAGE/assets/118042624/b1eabeb4-0a1c-4070-be38-4285a7195179)

<br>
<br>

### iv)Access rows and columns


![Screenshot 2023-08-23 091914](https://github.com/JeevaGowtham-S/READ-AND-WRITE-IMAGE/assets/118042624/8e4edab5-4a28-4169-b4a1-3e0d3316942e)
<br>
<br>

### v)Cut and paste portion of image
 ![Screenshot 2023-08-23 115319](https://github.com/JeevaGowtham-S/READ-AND-WRITE-IMAGE/assets/118042624/de8e7bd0-557c-454b-9d07-d90db5d88c43)
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
