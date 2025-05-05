# Face Detection Using OpenCV – Project Report

## 1. Introduction

This project implements a real-time face detection system using OpenCV in Python. The purpose of the system is to detect human faces in a video stream captured from a webcam. Face detection is a fundamental step in many computer vision applications, such as facial recognition, emotion detection, and human-computer interaction.

## 2. Objective

- To develop a face detection application using OpenCV and Haar Cascade Classifiers.
- To demonstrate real-time detection performance using live webcam video input.
- To visualize detected faces by drawing bounding boxes around them.

## 3. Tools and Technologies

- **Programming Language**: Python
- **Libraries Used**:
  - OpenCV (`cv2`) – for image processing and real-time video capture
  - NumPy – for numerical operations (implicitly used by OpenCV)
  - Jupyter Notebook – for interactive coding and visualization

## 4. Methodology

The project uses Haar feature-based cascade classifiers, which is an effective object detection method proposed by Paul Viola and Michael Jones. The model is pre-trained on thousands of positive and negative images and is capable of detecting faces with reasonable accuracy and speed.

### Steps Followed:
1. Load Haar cascade XML file from OpenCV’s data directory.
2. Start capturing video from the webcam using `cv2.VideoCapture`.
3. Convert each frame to grayscale for efficient processing.
4. Apply `detectMultiScale` to locate faces.
5. Draw rectangles around the detected faces in the original frame.
6. Display the output in a separate window.

## 5. Implementation

The implementation is provided in the `FACE_DETECTION.ipynb` notebook file. It includes:
- Initialization of the face detector.
- Real-time video feed processing loop.
- Termination condition when the user presses a specific key (e.g., 'q').


## 6. Conclusion

This project successfully demonstrates the implementation of a real-time face detection application using OpenCV. It can serve as a foundation for more advanced projects such as face recognition, attendance systems, or emotion analysis.

## 7. Future Enhancements

- Add face recognition using LBPH or deep learning models.
- Detect multiple facial features (eyes, smile, etc.).
- Deploy the application as a desktop or web-based app.

## 8. References

- OpenCV Documentation: https://docs.opencv.org
- Haar Cascade Classifiers: https://github.com/opencv/opencv/tree/master/data/haarcascades


