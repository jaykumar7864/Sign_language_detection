# Sign_language_detection
About the Project
This project aims to achieve American Sign Language Detection using Deep Learning. Also, real time webcam detection is a major aim of this project which will be refined from time to time.

# Dataset Used

The dataset used can be found on Kaggle.

# Specific Packages
PyTorch >= 1.4.

Albumentations >= 0.4.3.

Scikit-Learn >= 0.22.1.

# Using the Repository
Download the zip file


# Get Started
You can run this model on your system by installing a couple of things :

Python
Mediapipe
Python libraries and modules like OpenCV, Time, and OS.
You can get started by checking out any of the setup guides for their installation. However, links to official sites and guides have been attached.

# Working of the project:
# 1. Input data:
The module takes in video or image data as input, which contains one or more hands to be tracked.

# 2. Pre-processing:
The input data is pre-processed to prepare it for analysis. This may involve resizing, normalization, or any other required data transformations.

# 3. Architecture
The hand landmarker model bundle contains a palm detection model and a hand landmarks detection model.

# 4. Hand detection:
The first step in hand tracking is to detect the presence of a hand in the input data. The imported module (mediapipe) uses a machine-learning model to detect the hand in each frame of the video or image. The Palm detection model locates hands within the input image, and the hand landmarks detection model identifies specific hand landmarks on the cropped hand image defined by the palm detection model.

# 5. Hand landmark estimation:
Once a hand has been detected, the MediaPipe Hand Tracking module uses another machine-learning model to estimate the positions of 21 landmarks on the hand, such as the fingertips, knuckles, and wrist.

# 6. Hand tracking:
The estimated hand landmarks are then tracked across frames of the video or image data to determine the hand's movements and gestures.
![image](https://github.com/user-attachments/assets/bba445a1-9287-4560-b4a7-4ddfe7e4f724)


# 7. Post-processing:
Once the hand has been tracked, the output data is post-processed to make it easier to understand or use. In our code, we have returned a list of tuples of id no. , x,y, and z coordinates of each of the 21 landmarks for further use in sign detection.

# 8. Output visualization:
Finally, the results of the hand-tracking analysis are visualized as text on the user’s screen.
![image](https://github.com/user-attachments/assets/ad925ffb-1ab3-4790-8d2f-818322fd336f)

![image](https://github.com/user-attachments/assets/2fe1bad2-dd77-4f38-a52d-a51c62c490a4)

![image](https://github.com/user-attachments/assets/44e491f1-ed26-4af6-9f89-fde9abca9814)

![image](https://github.com/user-attachments/assets/2f2bb9a7-47f1-4069-972b-6204a4fd127b)



# System Requirements
The operating system should be compatible with the MediaPipe framework and any additional software or libraries used in the application.
The processor should have sufficient processing power to handle real-time video data and machine learning computations.
A camera with at least 720p resolution and 30 frames per second (fps) is recommended for capturing video data.
However, the model uses the Mediapipe framework which is a lightweight framework and can be used for mobile ML solutions.
