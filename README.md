Real-Time Finger Counting with OpenCV and MediaPipe

🚀 Project Overview
This project detects and counts fingers in real time using OpenCV and MediaPipe, providing the following functionalities:

🎯 One-hand detection with finger counting.

✋ Both-hand detection with individual and total finger count.

🎥 External camera support (e.g., mobile camera) for better video quality.

💾 Video recording of the processed output with stable FPS and H.264 codec for high-quality playback.

⚙️ Features
✅ Real-time hand tracking with accurate finger counting.
✅ Displays individual finger count for left and right hand.
✅ Shows the total finger count.
✅ Saves the processed video in .mp4 format.
✅ Supports external camera (mobile) for better quality.

🛠️ Tech Stack
Language: Python

Libraries:

OpenCV → For real-time video processing.

MediaPipe → For hand detection and finger tracking.

Video Codec: H.264 for high-quality recording.

📝 Installation
Clone the repository

bash
Copy
Edit
git clone https://github.com/your-username/finger-counter.git
cd finger-counter
Create a virtual environment

bash
Copy
Edit
# For Windows
python -m venv env
env\Scripts\activate

# For Linux/Mac
python3 -m venv env
source env/bin/activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
🚀 Usage
📹 1. One-Hand Detection (Laptop Camera)
Run the following script to detect and count fingers using your laptop camera:

python
Copy
Edit
python one_hand_laptop_cam.py
✋ 2. Both-Hands Detection (Laptop Camera)
Run the following script to detect and count fingers for both hands:

python
Copy
Edit
python both_hands_laptop_cam.py
📱 3. Both-Hands Detection (External Camera)
To use your mobile phone camera:

Connect your phone using DroidCam or Iriun.

Identify the camera ID (e.g., 2 or 3).

Run:

python
Copy
Edit
python both_hands_external_cam.py
🔥 Code Explanation
📌 Finger Counting Logic
Thumb Detection:

For left hand, thumb is open when tip_x > base_x.

For right hand, thumb is open when tip_x < base_x.

Other Fingers:

A finger is open if its tip is above its second joint.

📌 Video Recording
The program saves the processed video using the H.264 codec with stable FPS and resolution.

The output is saved as:

Copy
Edit
finger_counter_output.mp4
📸 Demo
✅ Real-time finger counting with both hands:

🚀 Contributing
Contributions are welcome! Feel free to:

🛠️ Fork the repository.

🔥 Create a new branch.

🚀 Submit a pull request.

📄 License
This project is licensed under the MIT License. You’re free to modify and distribute it with attribution.

🙌 Acknowledgments
OpenCV → For real-time video processing.

MediaPipe → For hand and finger landmark detection.

DroidCam/Iriun → For using external mobile camera as webcam.

✅ Star the repo ⭐ and fork it 🔥 if you find it useful!
📬 For any questions or suggestions, feel free to reach out!

