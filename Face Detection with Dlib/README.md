# **HOG + Linear SVM face detection with dlib**

Pros 
- More accurate than Haar Cascades
- More stable detection than Haar cascade (ex. fewer parameter to tune)

Cons
- Only works on frontal views of the face due to nature of HOG descriptor (does not perform well under rotation or viewing angle changes.)
- Requires an additional library (dlib) be installed 
- Not as accurate as deep learning-based face detector
- For the accuracy, its actually quite expensive due to image pyramid construction, sliding windows and computing HOG Features at every stop of the window.



