# Emotion Recognition in Video Frames with Object Detection
This project demonstrates the process of detecting emotions in video frames where objects have been previously identified using YOLOv8. It utilizes a pre-trained emotion recognition model to label the detected faces in each frame with their corresponding emotions.

# Overview
The project consists of several steps:

## Data Preparation:

The project begins with extracting frames from a given video file. These frames are stored as individual images.
## Object Detection:

YOLOv8 model is used to detect objects in each frame of the video. The detected objects are then utilized to localize faces for emotion recognition.
## Emotion Recognition:

A pre-trained deep learning model for emotion recognition is employed to analyze each face detected in the frames.
The model predicts the dominant emotion expressed in each face, assigning it a label.
## Visualization:

The emotion labels are added to the frames, providing a visual representation of the detected emotions.
Optionally, the frames can be compiled back into a video with the emotion labels for further analysis or presentation.

## Requirements
Python 3.x
OpenCV
Keras
NumPy
Ultralytics (for YOLOv8 object detection)
Usage
## Setup:

Install the required dependencies mentioned in the requirements.txt file.
## Data Preparation:

Place the video file you want to analyze in the appropriate directory.
Run the provided code to extract frames from the video.
## Object Detection:

Utilize YOLOv8 to detect objects in the frames. Ensure that YOLOv8 model (yolov8m.pt) is present in the correct directory.
Detected objects will be localized, assisting in face detection.
## Emotion Recognition:

Employ the pre-trained emotion recognition model (model.h5) to analyze faces in the frames.
The model predicts the dominant emotion for each face.
## Visualization:

Visualize the emotion labels added to each frame.
Optionally, compile the frames into a video with emotion labels for further analysis.
## Reproduction:

The code is designed to be easily reproducible. Simply follow the instructions provided and adjust parameters as needed.
## Notes
Ensure proper file paths and directory structures are maintained.
Adjust hyperparameters and model configurations as required for specific use cases.
Additional preprocessing or post-processing steps can be incorporated for enhanced results.
## Credits
This project utilizes Ultralytics for YOLOv8 object detection.
The emotion recognition model is based on a pre-trained deep learning model.
## References
Ultralytics YOLOv5: GitHub Repository
