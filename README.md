Educational Assistant System
An intelligent system that combines automated assignment grading with classroom emotion detection to provide comprehensive educational insights.

 Features ✨

- Automated Assignment Grading: Evaluate student submissions against rubric criteria
- Multi-Format Support: Process text files, Word docs, PDFs, and even images with OCR
- Emotion Detection: Analyze student engagement through facial expressions
- Real-Time Monitoring: Use webcam feed for live classroom analysis
- Detailed Feedback: Generate personalized feedback and improvement suggestions

 Installation 🛠️

1. Clone this repository:
   bash
   git clone https://github.com/yourusername/educational-assistant.git
   cd educational-assistant
   

2. Install required packages:
   bash
   pip install -r requirements.txt
   

3. For additional OCR capabilities (optional):
   bash
   sudo apt-get install tesseract-ocr
   

 Usage Guide 📚

 Assignment Grading
python
from educational_assistant import EducationalAssistant

assistant = EducationalAssistant()
results = assistant.upload_and_process_files()

print(f"Grade: {results['grade']['letter_grade']}")
print(f"Feedback:\n{results['feedback']}")


 Emotion Detection
python
# For single image analysis
emotion_results = assistant.process_uploaded_image_for_emotions()

# For real-time classroom monitoring (30 seconds)
assistant.monitor_classroom_using_colab_camera()

# For continuous monitoring
face_detect()


 System Components 🧩

 1. Document Processing
- Extracts text from multiple formats (DOCX, PDF, images)
- Uses OCR for handwritten/textual images
- Processes rubric criteria for evaluation

 2. AI Grading Engine
- Semantic analysis using RoBERTa and BERT models
- Grammar and structure evaluation
- Customizable rubric-based scoring

 3. Emotion Detection
- Real-time facial expression analysis
- Classroom engagement scoring
- Mood distribution visualization

 Example Output 📊

Grading Report:

Grade: B (82.5%)

Strengths:
• Research Depth: Your work shows strong understanding in this area.
• Argument Structure: Well-organized presentation of ideas.

Areas for improvement:
• Citations: Consider enhancing your work by focusing more on this aspect.
• Conclusion: Could be more comprehensive.

Grammar and Structure:
• Check your grammar and sentence structure for clarity.


Classroom Analysis:

 Classroom Emotional Analysis Report

 Emotion Distribution:
- Happy: 8 students
- Neutral: 3 students
- Surprise: 2 students

 Engagement Score: 0.73
(-1.0 = completely disengaged, 1.0 = fully engaged)

 Dominant Mood: Happy

 Recommendations:
• Students appear stimulated - good time for introducing new concepts


 Requirements 📋

- Python 3.7+
- See [requirements.txt](requirements.txt) for full package list
- Webcam (for real-time analysis)

 Contributing 🤝

We welcome contributions! Please fork the repository and create a pull request with your improvements.

 License 📜

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



Note for Colab Users: When running in Google Colab, you'll need to authorize camera access for real-time features. The system is optimized for Colab's environment but can be adapted for local use.

