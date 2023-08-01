# Hand Gesture Based Cursor Control System

This project is a hand gesture-based cursor control system using computer vision. It allows the user to control the cursor on the screen using their hand movements captured by the webcam. The system is implemented in Python and uses the OpenCV library for image processing and the Mediapipe library for hand tracking.

### Summary of the Project:

#### Objective:
The main objective of the project is to provide a hands-free and intuitive way to control the cursor on a computer screen using hand gestures.

#### Libraries Used:

- **OpenCV**: For capturing video frames from the webcam and image processing tasks.
- **Mediapipe**: For hand tracking and detecting landmarks on the hand.
- **NumPy**: For numerical and array operations.
- **Time**: For measuring frame rate and time-related operations.
- **Pyautogui**: For controlling the cursor and performing mouse-related actions.

#### Functionality:

The system uses the webcam to capture live video frames. It detects and tracks the user's hand in real-time using the Mediapipe hand tracking module. Hand landmarks, including the coordinates of specific fingertips and other points, are detected.
The system recognizes various hand gestures, such as an open hand, pointing, and finger pinching.
The cursor on the computer screen is controlled based on the movements of the user's hand:

- When the forefinger is up and the middle finger is down, the cursor follows the movements of the forefinger tip, enabling cursor control by hand movement.

- When the forefinger and middle finger are both up and close to each other, the system simulates a mouse click, allowing the user to interact with the computer without touching the mouse.

#### User Interface:

The system displays the video stream from the webcam, with hand landmarks drawn on the hand for visual feedback.
The frame rate (FPS) is shown in the top-left corner of the video stream.

#### Control Parameters:

- **FrameRate**: A parameter that sets the boundary box size for the hand within the video frame.
smoothening: A factor used to smooth the cursor movement for a more natural interaction.

- **Interaction**: The user can control the cursor by moving their hand while keeping the middle finger down.
To perform a mouse click, the user needs to bring the forefinger and middle finger close to each other.
