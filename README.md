## Real-Time Face Detection  and counter Script

This Python script captures live video from your default webcam and performs real-time face detection using dlib’s HOG-based frontal face detector and OpenCV.

With this project I intended to apply what I have learnt about OpenCV 

**Key Functionality**  
- Initializes a video stream (`cv2.VideoCapture(0)`) and flips each frame horizontally for a mirror-view display.  
- Converts incoming frames to grayscale and applies `dlib.get_frontal_face_detector()` to locate faces.  
- Draws a red bounding box around each detected face and labels them sequentially (e.g., “face1”, “face2”).  
- Displays the annotated video in a window titled **faces**, updating in real time.  
- Exits cleanly when the user presses the **q** key.  

**Dependencies**  
- OpenCV (`cv2`) for video capture, image processing, and display  
- NumPy (`numpy`) for array handling  
- dlib for the pretrained HOG + Linear SVM face detector
