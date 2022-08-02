Hello everyone

In this repository you can find a basic and simple Object Measurement project that is work with **aruco marker**.
While i don't have any camera with laser to measure the distance of the objects, I find out that i can use ArUco markers as a main measure and then use it to measure other objects in the camera. 
Here in the photo blow, the green line is the aruco marker and the blue line is a detected object. Also the red dot is the center of the blue box. So we can calculate the **height** and **width** of a detected box-object from there.

![](https://github.com/Ali619/Object-Detection-Size-Measurement/blob/master/aruco_pic.jpg?raw=true)


# Requirements: 

**Important Note:** **For this project I used `opencv-contrib-python` package. If you just and only install `opencv`, you will get error.**
If you still getting error after installing `opencv-contrib-python` package, you can find the solution [here](https://stackoverflow.com/questions/45972357/python-opencv-aruco-no-module-named-cv2-aruco/56867817).

I put `5x5_aruco-10.svg` file to print it. But be sure that you print it by 5x5 centimiter size if you want to use the exact code that I write. If you print it with other sizes, you should change the code as well. (The part that pixels will convert to centimiters)

# About the project: 

The program will first detect *ArUco* and draw a green line around it. Then it will calculate how many pixels that the green line have. Next it will convert the amount of pixels to Centimeter and in this way the program can measure the objects in camera. 

The size of ArUco (the one that i used in this project) is 5x5 centimeter. So we can divide the amount of Pixels that the camera detect by 20 and calculate the size. 

# How to run the project:
* You should run `measure_object_size_camera.py` file

I hope you guys enjoy it 👍
