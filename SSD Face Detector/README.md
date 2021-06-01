# **Face detection in images with OpenCV and Deep learning**

NOTEBOOK DEMO:  [![Nbviewer](https://github.com/jupyter/design/blob/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/shejz/face-detection-recognition/blob/main/SSD%20Face%20Detector/ssd_face%20detector.ipynb)

The more accurate OpenCV face detector is deep learning based, and in particular, utilizes the **Single Shot Detector** (SSD) framework with **ResNet** as the base network.

**Pros**
- Accurate face detector
- Utilizes modern deep learning algorithms
- No parameter tuning required
- Can run in real-time on modern laptops and desktop
- Model is reasonably sized (just over 10MB)
- Relies on OpenCV's cv2.dnn module
- Can be made faster on embedded devices by using OPENVINO  and Movidius NCS

**Cons**
- Much accurate than Haar cascades and HOG + Linear SVM, but not as accurate as dlib's CNN NMOD Face Detector.
- May have unconscious biases in the training set - may not detect darker-skinned people as accurate as lighten-skinned people.
