# Driver Drowsiness Detection System using dlib 68 landmarks and ear

This is a simple implementation of a driver drowsiness detection system that uses dlib's 68 landmarks and EAR (Eye Aspect Ratio) to detect if the driver is drowsy or not.

## Requirements
* Python 3.x
* dlib
* OpenCV
* imutils
* scipy
* pygame

## Installation

You can install the required libraries by running the following command:

pip install dlib opencv-python imutils scipy pygame

## Usage
To run the program, open your terminal or command prompt and navigate to the directory where the driver_drowsiness_detection.py file is located. Then run the following command:

python driver_drowsiness_detection.py

The program will start and it will access your default camera to capture the face. Once it detects the face, it will use dlib's 68 landmarks to detect the eyes and calculate the EAR.

If the eye closes for more than 20 frames and the EAR is less than the minimum threshold, an alert will be shown and an alarm will turn on. You can press the 'q' key to close or stop the program.

## How it works
The program works by using dlib's pre-trained facial landmark detector to detect the coordinates of the eyes. It then calculates the Eye Aspect Ratio (EAR) using scipy to find the euclidean distance between the average of the vertical landmarks of the eye and the euclidean distances of the horizontal landmarks of the eye.

If the EAR falls below a certain threshold and the eye is closed for more than 20 frames, an alert will be shown on the screen and an alarm sound will turn on using pygame.







