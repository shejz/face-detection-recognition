
# **dlib’s HOG + Linear SVM and MMOD face detectors**

NOTEBOOK DEMO:   [![Nbviewer](https://github.com/jupyter/design/blob/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/shejz/face-detection-recognition/blob/main/Face%20Detection%20with%20Dlib/face_detection_dlib.ipynb)

**dlib includes two face detection methods built into the library**:

1. A **HOG + Linear SVM face detector** that is accurate and computationally efficient.
2. A **Max-Margin (MMOD) CNN face detector** that is both highly accurate and very robust, capable of detecting faces from varying viewing angles, lighting conditions, and occlusion.



**HOG + Linear SVM face detection with dlib**

**Pros** 
- More accurate than Haar Cascades
- More stable detection than Haar cascade (ex. fewer parameter to tune)

**Cons**
- Only works on frontal views of the face due to nature of HOG descriptor (does not perform well under rotation or viewing angle changes.)
- Requires an additional library (dlib) be installed 
- Not as accurate as deep learning-based face detector
- For the accuracy, its actually quite expensive due to image pyramid construction, sliding windows and computing HOG Features at every stop of the window.


> The **HOG + Linear SVM** face detector will be faster than the **MMOD CNN** face detector but will also be less accurate as **HOG + Linear SVM** does not tolerate changes in the viewing angle rotation. For more robust face detection, use **dlib's MMOD CNN** face detector. This model requires significantly more computation (and is thus slower) but is much more accurate and robust to changes in face rotation and viewing angle.



