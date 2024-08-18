✨Volume Controller: The volume controller uses hand gestures to adjust the system's volume. It leverages computer vision to detect hand movements and gestures, translating them into volume adjustments in real-time. Here's a brief overview of how it works:

Hand Detection: The system captures video from a webcam and uses a hand tracking module to detect the user's hand in the frame.
Distance Measurement: It measures the distance between the thumb and index finger to determine the volume level.
Volume Adjustment: The distance between these fingers is mapped to the system's volume range, and the volume is adjusted accordingly.
UI Feedback: It provides visual feedback through the user interface, showing the current volume level and a visual representation of the volume bar.

✨Packages Used : 

1. cv2 (OpenCV): Captures video from the webcam and processes images, including displaying frames and drawing shapes.
2. cvzone: Provides hand tracking and gesture recognition tools, specifically the HandDetector for detecting and tracking hands.
3. numpy: Handles numerical operations and array manipulations, used for mapping finger distances to volume levels.
4. pycaw: Interfaces with Windows audio settings to control the system volume.
5. ctypes and comtypes: Facilitate interaction with Windows COM interfaces used by pycaw for volume control.
6. time: Manages time-related tasks, such as calculating FPS and introducing delays.
