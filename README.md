# Face Detection using Haar Cascades with OpenCV and Matplotlib

**Developed by:** C J Rohit
**Register No:** 212224243005

---

## Aim

To write a Python program using OpenCV to perform the following image manipulations:

1. Extract Region of Interest (ROI) from an image.
2. Perform face detection using Haar Cascades in static images.
3. Perform eye detection in images.
4. Perform face detection with labels in real-time video using a webcam.

---

## Software Required

* **Anaconda** – Python 3.7 or above
* **Python**
* **OpenCV** (`opencv-python`)
* **NumPy**
* **Matplotlib**
* **Jupyter Notebook** or any Python IDE such as VS Code or PyCharm

---

## Libraries Used

```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
```

---

## Algorithm

### I. Load and Display Images

1. Import the required Python libraries.
2. Load the image in grayscale using `cv2.imread()` with flag `0`.
3. Display the image using `matplotlib.pyplot.imshow()`.
4. Use `cmap='gray'` to display the image in grayscale.

### II. Load Haar Cascade Classifiers

1. Load the Haar Cascade XML file for face detection.
2. Load the Haar Cascade XML file for eye detection.
3. Create cascade classifier objects using OpenCV.

### III. Perform Face Detection in Images

1. Define a function `detect_face()`.
2. Create a copy of the input image.
3. Use `detectMultiScale()` to detect faces.
4. Draw rectangles around the detected faces.
5. Return the processed image.

### IV. Perform Eye Detection in Images

1. Define a function `detect_eyes()`.
2. Create a copy of the input image.
3. Use `detectMultiScale()` to detect eyes.
4. Draw rectangles around the detected eyes.
5. Return the processed image.

### V. Display Detection Results

1. Load the required image.
2. Call the `detect_face()` function for face detection.
3. Call the `detect_eyes()` function for eye detection.
4. Display the processed image using Matplotlib.

### VI. Real-Time Face Detection Using Webcam

1. Open the webcam using `cv2.VideoCapture(0)`.
2. Continuously read frames from the webcam.
3. Convert each frame to grayscale.
4. Detect faces using the Haar Cascade classifier.
5. Draw rectangles around detected faces.
6. Display the detected faces in real time.
7. Press the **ESC key (27)** to stop the video.
8. Release the webcam and close all OpenCV windows.

---

## Haar Cascade Classifiers

Haar Cascade is an object detection method provided by OpenCV. It uses pre-trained XML classifiers to detect specific objects.

### Classifiers Used

* `haarcascade_frontalface_default.xml` – Detects human faces.
* `haarcascade_eye.xml` – Detects human eyes.

---

## Functions Used

| Function                  | Purpose                          |
| ------------------------- | -------------------------------- |
| `cv2.imread()`            | Loads an image                   |
| `cv2.CascadeClassifier()` | Loads Haar Cascade classifier    |
| `detectMultiScale()`      | Detects faces or eyes            |
| `cv2.rectangle()`         | Draws rectangles                 |
| `cv2.cvtColor()`          | Converts image color space       |
| `cv2.VideoCapture()`      | Captures webcam video            |
| `cv2.imshow()`            | Displays video frames            |
| `cv2.putText()`           | Adds text labels                 |
| `cv2.waitKey()`           | Waits for keyboard input         |
| `cap.release()`           | Releases webcam                  |
| `cv2.destroyAllWindows()` | Closes OpenCV windows            |
| `plt.imshow()`            | Displays images using Matplotlib |

---

## Expected Output

* Original grayscale image.
* <img width="389" height="409" alt="download" src="https://github.com/user-attachments/assets/ff1f3af3-8df1-4e9d-a460-d23b4e94ec4d" />

* Face detected image with rectangles.
* <img width="389" height="409" alt="download" src="https://github.com/user-attachments/assets/fd2cea6f-0e7e-4f9b-b1a9-160b981cf24f" />

* Eye detected image with rectangles.
* <img width="389" height="409" alt="download" src="https://github.com/user-attachments/assets/c90cc881-25fd-4f23-96fd-6eec30ce1a23" />

* Real-time webcam face detection.
* <img width="389" height="409" alt="download" src="https://github.com/user-attachments/assets/ce3ba615-ab31-4554-8a88-2efc92864344" />

* **"Face Detected"** label above the detected face.
* <img width="482" height="502" alt="download" src="https://github.com/user-attachments/assets/1928a649-e2e4-487e-b066-4bdfd4e0d6ef" />


---

## Result

Thus, the Python program was successfully implemented using **OpenCV and Haar Cascade classifiers** to detect faces and eyes in static images and detect and label faces in real-time webcam video.

---

## Conclusion

Haar Cascade classifiers provide a simple and efficient method for detecting faces and eyes in images and real-time video. OpenCV enables image processing, object detection, and real-time webcam-based face detection.

---

**Developed by:** C J Rohit
**Register No:** 212224243005
