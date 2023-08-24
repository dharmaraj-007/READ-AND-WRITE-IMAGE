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
### Developed By:Dharmaraj S
### Register Number: 212222240025
i) #To Read,display the image
```
  import cv2
img = cv2.imread('flower.png', 0)
resized_img = cv2.resize(img, None, fx=0.8, fy=0.8)
cv2.imshow('212222240025', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image
```

import cv2
img=cv2.imread('flower.png',0)
cv2.imwrite('writed_walt.png',img)

```
iii) #Find the shape of the Image
```python3

import cv2
img=cv2.imread('flower.png',0)
print(img.shape)

```
iv) #To access rows and columns

```python3

import cv2
img = cv2.imread('flower.png', 0)
resized_img = cv2.resize(img, None, fx=0.8, fy=0.8)
for i in range(100, 250):
    for j in range(10, 50):
        resized_img[i][j] = 255  
cv2.imshow('212222240025', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
v) #To cut and paste portion of image
```python3

import cv2
img = cv2.imread('flower.png', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222240025', img)
cv2.waitKey(0)


```

## Output:
### i) Read and display the image

![dip flower](https://github.com/dharmaraj-007/READ-AND-WRITE-IMAGE/assets/119560386/fd690494-a649-4279-bb74-9d472d460983)

### ii)Write the image
![dip image](https://github.com/dharmaraj-007/READ-AND-WRITE-IMAGE/assets/119560386/00564374-fcee-4121-b0e4-6a63521f0d16)


### iii)Shape of the Image

![dip shape of the image](https://github.com/dharmaraj-007/READ-AND-WRITE-IMAGE/assets/119560386/272ac8e4-b6ed-4010-bda7-fed557363be9)


### iv)Access rows and columns
![dip row and col](https://github.com/dharmaraj-007/READ-AND-WRITE-IMAGE/assets/119560386/4c255cd4-8880-4a8a-87f2-502bbeb5d49b)


### v)Cut and paste portion of image
![cut and copy](https://github.com/dharmaraj-007/READ-AND-WRITE-IMAGE/assets/119560386/62d0f832-7c49-47d0-92a3-3e561a8ff1f6)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
