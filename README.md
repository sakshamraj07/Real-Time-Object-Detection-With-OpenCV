# Real-Time-Object-Detection-With-OpenCV
Introduction
Real-Time Object Detection with OpenCV
This project demonstrates real-time object detection using a laptop camera or webcam with OpenCV and the MobileNetSSD deep learning model. It processes each frame of the video stream to detect and classify objects—such as people, chairs, dogs, etc.—and displays them with bounding boxes for easy visualization.
Getting Started
Clone the Repository
git clone https://github.com/Surya-Murali/Real-Time-Object-Detection-With-OpenCV.git
cd Real-Time-Object-Detection-With-OpenCV
Install Required Libraries
Ensure that you have the necessary libraries installed. On macOS, you can use Homebrew and pip:
brew install opencv
pip install opencv-python
pip install opencv-contrib-python
pip install opencv-python-headless
pip install opencv-contrib-python-headless
pip install matplotlib
pip install imutils
Note: Make sure to install OpenCV (version 3.3 or newer) and OpenCV-contrib to enable support for the Deep Neural Network (DNN) module.
Verify Video Devices
To check your connected video devices (e.g., webcam or FaceTime HD Camera), use the following commands in your terminal:
system_profiler SPCameraDataType
system_profiler SPCameraDataType | grep "^    [^ ]" | sed "s/    //" | sed "s/://"
Run Real-Time Object Detection
Start the video stream and begin object detection by executing:
python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
Need Help with Arguments?
To see available command-line arguments and their descriptions:
python real_time_object_detection.py --help
References and Useful Links
MobileNet-SSD GitHub Repository

OpenCV GitHub Repository

Understanding OpenCV’s blobFromImage Function

Imutils GitHub Repository

Overview
This project combines the lightweight MobileNet-SSD model for object detection with OpenCV for image processing and imutils for convenience functions. It serves as a hands-on implementation of real-time object detection and is ideal for getting started with computer vision applications.





