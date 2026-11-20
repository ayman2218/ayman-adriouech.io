# Fall-detection mobile robot — vision and edge computing

**Technology:** Raspberry Pi 5, OpenCV, MediaPipe Pose, Python, ROS Noetic, MQTT, Android.

This project explores a robot companion that detects changes of posture using 33 MediaPipe Pose landmarks. Rather than running a recurrent classifier, it computes interpretable geometric indicators: torso orientation, vertical anthropometric ratio and hip displacement. Sustained detections trigger an alert; the design prioritizes stopping motors during a suspected fall.

**System architecture:** camera acquisition → pose extraction → fall decision → motion control → MQTT notification to an Android app.

The technical portfolio describes a five-node ROS Noetic architecture and the MediGuard Pro prototype. **No clinical validation or safety certification is claimed.** This is a research prototype, not a certified medical device.

**Code:** [fall repository](https://github.com/ayman2218/fall), including Python detector variants and Raspberry Pi setup notes.
