
# 🎓 Educational Assistant System

An intelligent system that combines **automated assignment grading** with **classroom emotion detection** to provide comprehensive educational insights aligned with [UN SDG 4: Quality Education](https://sdgs.un.org/goals/goal4).

![Python](https://img.shields.io/badge/Python-3.7+-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-orange)

---

## ✨ Features

- 📄 **Automated Assignment Grading**: Evaluate student submissions against rubric criteria
- 📦 **Multi-Format Support**: Process `.txt`, `.docx`, `.pdf`, and image files with OCR
- 😃 **Emotion Detection**: Analyze student engagement through facial expressions
- 📹 **Real-Time Monitoring**: Use webcam for live classroom mood tracking
- 📬 **Detailed Feedback**: Personalized suggestions for academic improvement


  <img src="https://github.com/raahulmaurya1/Procoder/blob/f766861df5dba890cc8df0e8732efdd02dcb0096/Feature.jpg" width="1000"/>

---



## 🏗️ Architecture

<img src="https://raw.githubusercontent.com/raahulmaurya1/Procoder/48f27a4667fa9c6a8b4663116a5fd765d5bd0996/diagram-export-4-5-2025-10_26_12-PM.png" alt="System Architecture" width="700"/>

## 🛠️ Installation

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/educational-assistant.git
cd educational-assistant

# 2. Install dependencies
pip install -r requirements.txt

# 3. (Optional) For OCR support
sudo apt-get install tesseract-ocr
```

---

## 📚 Usage Guide

### ✏️ Assignment Grading

```python
from educational_assistant import EducationalAssistant

assistant = EducationalAssistant()
results = assistant.upload_and_process_files()

print(f"Grade: {results['grade']['letter_grade']}")
print(f"Feedback:\n{results['feedback']}")
```

### 😊 Emotion Detection

```python
# Single image emotion detection
emotion_results = assistant.process_uploaded_image_for_emotions()

# 30-second webcam-based monitoring
assistant.monitor_classroom_using_colab_camera()

# Continuous monitoring
face_detect()
```

---

## 🧩 System Components

### 1️⃣ Document Processing
- OCR-enabled text extraction
- Supports DOCX, PDF, handwritten or printed images

### 2️⃣ AI Grading Engine
- RoBERTa + BERT-based semantic evaluation
- Customizable rubric
- Grammar and structural analysis

### 3️⃣ Emotion Detection
- Facial expression recognition
- Mood distribution + engagement score
- Real-time webcam support (Colab optimized)

---

## 📊 Example Outputs

### 🧠 Grading Report

**Grade**: B (82.5%)  
**Strengths**:
- Research Depth: Strong understanding
- Argument Structure: Well-organized

**Areas for Improvement**:
- Citations: Needs more attention
- Conclusion: Could be improved

**Grammar**: Minor clarity issues

---

### 😊 Classroom Emotional Analysis

**Emotion Distribution**:
- Happy: 8 students
- Neutral: 3 students
- Surprise: 2 students

**Engagement Score**: `0.73`  
**Dominant Mood**: `Happy`

**Recommendation**:  
Students are engaged – great time for interactive or new concepts!


---


## 🎥 Real-Time Emotion & Face Detection Output

🖼️ **Real-Time Output:**  
<img src="https://raw.githubusercontent.com/raahulmaurya1/Procoder/6aa3bd98bf85364346e95b51bec1f154d1c7564e/Screenshot%202025-04-06%20225311.jpg" width="1000"/>

🧠 **Emotion Detection:**  
<img src="https://raw.githubusercontent.com/raahulmaurya1/Procoder/48f27a4667fa9c6a8b4663116a5fd765d5bd0996/face_detect.png" width="600"/>



---

### 📉 Confusion Matrix

<img src="https://raw.githubusercontent.com/raahulmaurya1/Procoder/48f27a4667fa9c6a8b4663116a5fd765d5bd0996/confusion%20matrix.png" alt="Confusion Matrix" width="500"/>

### 📈 Loss & Accuracy

<img src="https://raw.githubusercontent.com/raahulmaurya1/Procoder/48f27a4667fa9c6a8b4663116a5fd765d5bd0996/loss%20%26%20accuracy.png" alt="Training Performance" width="500"/>

---

## 📋 Requirements

- Python 3.7+
- All dependencies listed in [`requirements.txt`](requirement.txt)
- Webcam (for real-time emotion detection)

---

## 🤝 Contributing

We ❤️ contributions!  
Fork the repo → make your changes → submit a PR.

---

## 📜 License

Licensed under the [MIT License](LICENSE)

---

## ⚠️ Note for Colab Users

This project supports Google Colab.  
📸 For real-time features, make sure to **authorize your webcam**.

---

## 📬 Contact

Created by Rahul Maurya 
📧 Email: raahulmaurya2@gmail.com  
🔗 GitHub: @raahulmaurya1
