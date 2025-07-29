AlertCam – Real-Time Motion Detection with Audio Alerts
AlertCam is a Python-based project that uses OpenCV to detect motion in real-time through your webcam and plays a pre-recorded audio alert when movement is detected. It’s ideal for simple security monitoring or as a base for advanced surveillance systems.

Features
Real-time motion detection using webcam feed

Draws bounding boxes around moving objects

Plays custom audio alerts (e.g., “Motion Detected!”)

Lightweight and easy to set up

Can be adapted for video files or live streaming feeds

Demo
(Add a screenshot or GIF of the running project here if possible)

Requirements
Python 3.7 or later

Libraries:

bash
Copy
Edit
pip install opencv-python playsound==1.2.2
Setup & Installation
Clone this repository:

bash
Copy
Edit
git clone https://github.com/swapnendukolay031/alertcam.git
cd alertcam
Place your pre-recorded audio file (e.g., motion_detected.wav) in the project folder.

Run the script:

bash
Copy
Edit
python live_motion.py
Usage
The webcam feed will open automatically.

When motion is detected:

A bounding box will appear on the object.

Your audio alert will play.

Press ESC to exit.

Customization
Replace motion_detected.wav with any audio file (e.g., siren, custom voice).

Adjust motion sensitivity by changing the contour area threshold in the code:

python
Copy
Edit
if cv2.contourArea(contour) < 900:  # Lower = more sensitive
    continue
Project Structure
bash
Copy
Edit
├── live_motion.py        # Main script
├── motion_detected.wav   # Pre-recorded alert sound
└── README.md             # Project documentation
Future Improvements
Add support for recording detected motion to a video file

Add cooldown timer for alerts to avoid repeated triggers

Implement email/SMS notification on motion detection

License
This project is licensed under the MIT License.