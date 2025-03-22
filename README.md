# 🖐️ Real-Time Finger Counting with OpenCV and MediaPipe

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![OpenCV](https://img.shields.io/badge/OpenCV-4.5%2B-green) ![MediaPipe](https://img.shields.io/badge/MediaPipe-0.9%2B-orange)

## 🚀 Project Overview
This project uses **OpenCV** and **MediaPipe** to detect and count fingers in real-time. It supports:
- 🎯 **One-hand detection** with finger counting.
- ✋ **Both-hand detection** with individual and total finger count.
- 🎥 **External camera support** (e.g., mobile camera) for better video quality.
- 💾 **Video recording** of the processed output with stable FPS and H.264 codec for high-quality playback.

---

## ⚙️ Features
✅ Real-time hand tracking with accurate finger counting.  
✅ Displays individual finger count for **left** and **right** hands.  
✅ Shows the **total finger count**.  
✅ Supports **external camera** (mobile) for better quality.  
✅ Saves the processed video in `.mp4` format.  

---

## 🛠️ Tech Stack
- **Language:** Python  
- **Libraries:**  
  - `OpenCV` → For real-time video processing.  
  - `MediaPipe` → For hand detection and finger tracking.  
- **Video Codec:** H.264 for high-quality recording.  

---

## 📝 Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/finger-counter.git
cd finger-counter
```

### 2. Create a virtual environment
#### Windows:
```bash
python -m venv env
env\Scripts\activate
```
#### Linux/Mac:
```bash
python3 -m venv env
source env/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

### 🎥 1. One-Hand Detection (Laptop Camera)
To detect and count fingers using your laptop camera:
```bash
python one_hand_laptop_cam.py
```

### ✋ 2. Both-Hands Detection (Laptop Camera)
To detect and count fingers for both hands using your laptop camera:
```bash
python both_hands_laptop_cam.py
```

### 📱 3. Both-Hands Detection (External Camera)
To use your mobile phone camera:
1. Connect your phone using **DroidCam** or **Iriun**.
2. Identify the camera ID (e.g., `2` or `3`).
3. Run:
```bash
python both_hands_external_cam.py
```

---

## 🔥 Code Explanation

### 🛠️ Finger Counting Logic
**Thumb Detection:**
- For **left hand**, thumb is open when `tip_x > base_x`.
- For **right hand**, thumb is open when `tip_x < base_x`.

**Other Fingers:**
- A finger is open if its tip is above its second joint.

### 🎥 Video Recording
- The program saves the processed video using the **H.264 codec** with stable FPS and resolution.
- The output is saved as:
  ```
  finger_counter_output.mp4
  ```

---

## 📸 Demo
✅ Real-time finger counting with both hands:
(Include a demo GIF or image here)

---

## 🙌 Acknowledgments
- **OpenCV** → For real-time video processing.
- **MediaPipe** → For hand and finger landmark detection.
- **DroidCam/Iriun** → For using external mobile camera as a webcam.

---

## ⭐ Contribute & Support
If you find this project useful:
✅ **Star** the repo ⭐  
✅ **Fork** it 🔥  
✅ Share your feedback!  

📬 For any questions or suggestions, feel free to reach out!

---

🔥 This README is clean, well-structured, and GitHub-ready! 🚀 Let me know if you want any modifications. 🎯
