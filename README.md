# **Face Detection and Recognition**

**How face recognition is different from face detection**

> Face detection and face recognition are distinctly different algorithms. 
- **Face detection** will tell you where in a given image/frame a face is (but not who the face belongs to) 
- **Face recognition** is the process of taking a face in an image and actually identifying who the face belongs to. Face recognition is thus a form of person identification that actually identifies the detected face.

**Face Detection Methods**:
1. [OpenCV Haar Cascades](https://github.com/shejz/face-detection-recognition/tree/main/Face%20Detection%20with%20Haar%20Cascades)
2. [OpenCV SSD Face Detector](https://github.com/shejz/face-detection-recognition/tree/main/SSD%20Face%20Detector)
3. [Dlib HOG + Linear SVM and MMOD CNN](https://github.com/shejz/face-detection-recognition/tree/main/Face%20Detection%20with%20Dlib)
4. [Local Binary Patterns (LBPs)](https://github.com/shejz/face-detection-recognition/tree/main/Face%20Recognition%20with%20Local%20Binary%20Patterns)
5. [OpenCV Eigenfaces](https://github.com/shejz/face-detection-recognition/tree/main/OpenCV%20Eigenfaces%20for%20Face%20Recognition)

- Haar cascade not anywhere near as accurate as its HOG + Linear SVM and deep learning-based face detection counterparts. Highly prone to false-positive detections. 
- HOG + Linear SVM more accurate than Haar cascades but not as accurate as deep learning-based face detectors. Only works on frontal views of the face it will not be detected as the HOG descriptor does not tolerate changes in rotation or viewing angle well.
- SSD more accurate than Haar cascades and HOG + Linear SVM, but not as accurate as dlib’s CNN MMOD face detector. May have unconscious biases in the training set that may not detect darker-skinned people as accurately as lighter-skinned people.
- Dlib’s CNN MMOD face detector is the most accurate of the bunch but is quite slow and cannot run in real-time without GPU acceleration.


**Sample Output**

![](https://github.com/shejz/face-detection-recognition/blob/main/face_detection_summary.jpg)

![](https://github.com/shejz/face-detection-recognition/blob/main/face_detection_summary2.jpg)

