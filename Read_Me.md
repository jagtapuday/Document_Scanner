# Document Scanner

In this project, I mainly use numpy and OpenCV. By using this project we can easily read images and convert them into the scanned images.
We can use both webcam or stored image for this project. There are two files utils.py and Main.py. In utiles.py I define
important functions that are necessary for Document Scan, these functions we will discuss later. In Main.py I import utils.py.
I would like to thank Murtaza's who helps me to complete this project.


steps->

1.Import Libraries

2.Import Image to scan #(cv2.imread() or cv2.VideoCapture(0))

3.Intialize Trackbars(utlis.initializeTrackbars())# let's considor as threshold min=200,max=200

4.Resize image #(cv2.resize())

5.Convert image into grayscale #(cv2.cvtColor(img,cv2.COLOR_BGR2GRAY))

6.Smoothing that grayscale image #(cv2.GaussianBlur())

7.Detecting edges #(cv2.Canny())

8.Dilation to increase white region #(cv2.dilate())

9.Erosion opposite to dilation #(cv2.erode())

10.Find all countours #(cv2.findContours())

11.Find biggest contour among all #(utilis.biggestContour())

12.Drow Border to contour

13.Warp the image with known contour

14.Apply adaptive threshold

15.Display Image Array with lables

16.By using Ctrl+S Save Image.
