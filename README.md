# 🧠 Cognivue: AI-Based Multimodal Fatigue Detection System

Cognivue is an AI-driven multimodal system designed to monitor **fatigue, emotional state, and attention levels** in real-time using computer vision and deep learning techniques. The system provides actionable insights such as **break recommendations and intelligent workload management** to improve productivity and wellbeing.

---

## 📌 Features

- 🎯 Real-time fatigue detection using webcam
- 😴 Eye tracking using Eye Aspect Ratio (EAR)
- 👁️ PERCLOS-based drowsiness estimation
- 😮 Yawn detection using Mouth Aspect Ratio (MAR)
- 😊 Facial emotion recognition (CNN-based)
- 🧭 Attention tracking using gaze and head pose
- 📊 Interactive dashboard with live metrics
- ⚡ Real-time streaming using Server-Sent Events (SSE)
- 🧠 Intelligent decision engine for recommendations

---

## 🧠 System Architecture

The system follows a multimodal pipeline:

1. **Data Acquisition**
   - Captures real-time video using webcam (20–30 FPS)

2. **Preprocessing**
   - Face detection
   - Facial landmark extraction
   - Face alignment and normalization

3. **Feature Extraction**
   - Eye Aspect Ratio (EAR)
   - Blink rate
   - PERCLOS
   - Mouth Aspect Ratio (MAR)
   - Head pose estimation

4. **Emotion Recognition**
   - CNN-based model for facial emotion classification

5. **Attention Analysis**
   - Gaze tracking
   - Face presence detection
   - Head orientation analysis

6. **Multimodal Fusion**
   - Combines fatigue, emotion, and attention scores

7. **Decision Engine**
   - Generates:
     - Break suggestions
     - Wellbeing alerts
     - Task reallocation recommendations

---

## 🛠️ Tech Stack

- **Languages:** Python
- **Libraries:** OpenCV, NumPy, Pandas, Dlib / Mediapipe
- **Deep Learning:** TensorFlow / Keras / PyTorch
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Django / Flask
- **Visualization:** Chart.js / Matplotlib
- **Streaming:** Server-Sent Events (SSE)

---

## 📊 Key Metrics

- Real-time processing at ~20–30 FPS  
- High accuracy in fatigue detection using PERCLOS and EAR  
- Stable predictions using temporal smoothing techniques  

---

## 💡 Use Cases

- Workplace productivity monitoring  
- Driver fatigue detection  
- Employee wellbeing systems  
- Smart workforce management  

---

## ⚙️ Installation

```bash
git clone https://github.com/YOUR_USERNAME/cognivue.git
cd cognivue
pip install -r requirements.txt
python app.py
