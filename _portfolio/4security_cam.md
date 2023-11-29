---
title: "Python - Security Cam"
excerpt: "Implementation a simple security cam that records video feed only when a face or a body is detected in the current frame. <br/><img src='/images/sec_cam.jpg'>"
collection: portfolio
---

In this project I implemented a simple security cam.
As long as the progam has a video feed from the camera, it checks every frame in order to determine whether a face or a body is present or not. If a face or a body is detected it starts recording until there are no faces or bodies in the frame, at which moment starts a countdown of 3 seconds and then, if still no faces or bodies are in the frame, it stops recording and saves the file with the exact date as file name, otherwise it keeps recording.
It also recognizes the faces in the frame using [haarcascade](https://docs.opencv.org/4.x/db/d28/tutorial_cascade_classifier.html) to detect the face and [LBPH, Eigenfaces or Fisherfaces](https://docs.opencv.org/4.x/da/d60/tutorial_face_main.html) to recognize it. At the moment it only recognizes me, but you can add any folder containing several pictures of the person you want the program to identificate.
Check it out at my [github repo](https://github.com/GianFederico/SIDE-security_cam_v2).
