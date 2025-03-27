# Fox Eye / Cat Eye Filter

This is a web-based real-time face detection and visual filter application that uses TensorFlow.js's FaceMesh model to detect facial landmarks in the user's video feed. The application can be used to apply various filters or visual effects based on the detected facial keypoints (such as the "Fox Eye" or "Cat Eye" effect). Currently, it visualizes the facial landmarks as orange dots on the user's face in the video stream.

## Features
- Real-time face detection using TensorFlow.js's FaceMesh model.
- Visualizes facial landmarks on the canvas overlaid on the live video feed.
- Displays a message when no face is detected.
- Fully responsive design: canvas and video scale with the viewport.

## Technologies Used
- **HTML5**: Provides the structure of the webpage with video and canvas elements.
- **CSS3**: Styles the video and canvas elements to fit the full page and ensure smooth interaction.
- **JavaScript**: Handles video stream setup, face detection logic, and rendering the face keypoints onto the canvas.
- **TensorFlow.js**: A JavaScript library for running machine learning models in the browser.
- **FaceMesh (TensorFlow.js model)**: Detects and tracks facial landmarks in real-time.
- **Web APIs**: 
  - `navigator.mediaDevices.getUserMedia()` to access the webcam and stream video.
  - `requestAnimationFrame()` to continuously render the detected faces.

## Setup

1. Clone or download the repository.
2. Open the `index.html` file in a modern web browser that supports WebGL and access to the camera (such as Chrome, Firefox, or Safari).
3. The browser will request permission to access the webcam. Once granted, the video stream will be displayed, and the face detection will begin.

## How It Works
1. **Camera Setup**: The `setupCamera()` function uses `navigator.mediaDevices.getUserMedia()` to access the user's webcam and display the video feed in the `<video>` element.
2. **Face Detection**: The `facemesh.load()` function loads the FaceMesh model, which detects facial landmarks from the video feed.
3. **Canvas Drawing**: The canvas element is used to draw the detected face landmarks in real-time. Orange circles are drawn over each keypoint on the detected face.
4. **No Face Detection**: If no face is detected, the message "No face detected" is displayed on the canvas.

## Publisher Information
- **Publisher**: Jiners Enoheart
- **Published On**: 03/15/2025

## License
This resource is open for educational and non-commercial use. Feel free to modify it for your own purposes.

---

## Screenshots

(Include some screenshots of the application in action here if needed.)

---

## Future Improvements
- Implementing customizable filters (like Fox Eye or Cat Eye effects).
- Optimizing face detection performance for mobile devices.
- Adding support for multiple face detection.

---

Feel free to submit issues or pull requests if you'd like to contribute to the project!