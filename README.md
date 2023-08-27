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
### Developed By:S VAISHNAV NANDA
### Register Number: 212222240112
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('rdr.jpg',1)
cv2.imshow('212222240112_VAISHNAV',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```

import cv2
color_img=cv2.imread('rdrjpg',1)
w= cv2.imwrite('0.png',color_img)
cv2.imshow('0',color_img)
cv2.waitKey(0)




```
iii) #Find the shape of the Image
```python3
import cv2
import random
color_img=cv2.imread('rdr.jpg',1)
print(color_img.shape)


```
iv) #To access rows and columns

```python3
import cv2
import random
color_img=cv2.imread('rdr.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222240112_Vaishnav',color_img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```python3
import cv2
color_image=cv2.imread('rdr.jpg',1)
tag=color_image[20:80,20:80]
color_image[90:150,90:150]=tag
cv2.imshow("212222240112_vaishnav",color_image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image
![Screenshot from 2023-08-27 15-03-07](https://github.com/VaishnavNanda/READ-AND-WRITE-IMAGE/assets/118707051/0a305354-2547-4af8-b15e-4b3ab7c1e48d)

<br>
<br>

### ii)Write the image:
![Screenshot from 2023-08-27 15-03-07](https://github.com/VaishnavNanda/READ-AND-WRITE-IMAGE/assets/118707051/ce143736-b25c-4d53-a90c-28f74aa2e9f4)



<br>
<br>

### iii)Shape of the Image
![Screenshot from 2023-08-27 15-11-15](https://github.com/VaishnavNanda/READ-AND-WRITE-IMAGE/assets/118707051/0771c210-66ce-408c-be28-bdd09329ba40)


<br>
<br>

### iv)Access rows and columns
![Screenshot from 2023-08-27 15-13-37](https://github.com/VaishnavNanda/READ-AND-WRITE-IMAGE/assets/118707051/f618260b-3c23-4c9a-99bc-fcc2eaedb81e)


<br>
<br>

### v)Cut and paste portion of image
![Screenshot from 2023-08-27 15-18-33](https://github.com/VaishnavNanda/READ-AND-WRITE-IMAGE/assets/118707051/54afb3f4-b05a-47ee-9988-976a23bff381)

<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.
