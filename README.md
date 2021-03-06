# DJI-Tello-Face-Follower
A project made in python that enables a DJI Tello Drone to follow a face.
It uses a simple resnet10 model to identify faces in the video stream from the drone and follow the face with the highest confidence
by checking the position of the bounding box. It maintains the distance from the face by checking the euclidean distance of the bbox and keeping it between a threshold of 110 with ± 5% tolerance.

Run the ```telloai.py``` file (keep the .py file just outside the resnet10 folder) with following arguments : 

1. ```-s <flag, if set, will save video to output.avi with XVID encoding>```
2. ```-c <float confidence value, default is 0.5>```
3. ```-p <prototxt file, default is given>```
4. ```-m <model file, default is given>```

**Demo :**

![](demo.gif)
