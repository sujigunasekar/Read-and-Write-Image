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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('download.jpeg',1)
cv2.imshow('212222230152_suji',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('download.jpeg',1)
w=cv2.imwrite('1.jpeg',color_img)
cv2.imshow('212222230152_suji',color_img)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('download.jpeg',1)
print(color_img.shape)



```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('download.jpeg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222230152',color_img)
cv2.waitKey(0)


```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('download.jpeg',-1)
tag=color_image[20:80,20:80]
color_image[90:150,90:150]=tag
cv2.imshow('212222230152_suji',color_image)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

![1d](https://user-images.githubusercontent.com/119559822/225263448-def05fd5-2921-4a5d-a000-a70397b2db17.png)


### ii)Write the image

![2d](https://user-images.githubusercontent.com/119559822/225263518-82a46560-05be-4dd8-a332-2f5e88190ea3.png)

### iii)Shape of the Image

![3d](https://user-images.githubusercontent.com/119559822/225263560-10b51931-02ac-463e-b620-65eafec099d1.png)

### iv)Access rows and columns

![4d](https://user-images.githubusercontent.com/119559822/225263682-b25de9b4-dc7a-4fbd-a116-698a8f5c255b.png)

### v)Cut and paste portion of image

![5d](https://user-images.githubusercontent.com/119559822/225263715-8d14b7e3-c14b-42f3-9219-2fa7c41c1edd.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


