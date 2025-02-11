# Real-time-face-blurring
Real-Time Face Detection &amp; Blurring: Python script using OpenCV to detect faces in webcam video, applying Gaussian blur for privacy. Easy to use, adjustable parameters. Ideal for privacy protection in image/video processing.

This repository contains a Python script that performs real-time face detection and blurring using a webcam. It utilizes the OpenCV library and a pre-trained Haar cascade classifier to detect faces in video frames and applies a Gaussian blur to those faces.

How it Works:-
The script initializes the video capture object to stream video from the default camera.
It loads the Haar cascade classifier file, which is used to detect faces in the video frames.
In a continuous loop, the script reads frames from the video capture object.
For each frame, it uses the face cascade classifier to detect faces.
Detected faces are isolated as regions of interest (ROIs) within the frame.
A Gaussian blur filter is applied to each ROI, effectively blurring the faces.
The blurred ROIs are inserted back into the original frame.
If no faces are detected in the frame, a text overlay is added to indicate this.
The modified frame, with blurred faces and any text overlays, is displayed in a window.
The loop continues until the user presses 'q' to quit.
Finally, the video capture object is released, and the OpenCV windows are closed.
Dependencies,
Python 3.x,
OpenCV library (cv2),
Haar cascade classifier file (haarcascade_frontalface_default.xml).
Usage :-
Install Python 3.x if you haven't already.
Install the required dependencies by running the command: pip install opencv-python.
Download the Haar cascade classifier file and place it in the same directory as the Python script.
Run the script using the command: python face_detection.py.
A window will open showing the webcam feed with faces blurred in real-time.
Press 'q' to exit the program.
Feel free to modify the parameters such as scaling factor and minimum neighbors in the detectMultiScale method to fine-tune the face detection. You can also adjust the kernel size and standard deviation in the GaussianBlur method to control the level of blurring.

Contributions:-
Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
