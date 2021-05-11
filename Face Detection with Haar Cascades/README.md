## **Pros and Cons of OpenCV's Haar Cascade Face Detector**:

**Pros**:
- Very fast, capable of running in super real-time
- Low computational requirements - can easily be run on a embedded, resource-constrained devices.
- Small model size (just over 400kb; for reference, most deep neural networks will be anywhere between 20-200MB)

**Cons**:
- Highly prone to false-positive detections
- Typically requires manual tuning to the detectMultiScale function
- Not anywhere near as accurate as its HOG + Linear SVM and Deep Learning-based face detection 
  counterparts
