# Real-Time Facial Recognition for Classroom Attendance 🎓📸

> An AI-based system using FaceNet and deep learning to automate student attendance via real-time facial recognition.

## 📌 Project Overview
This project replaces traditional manual attendance with a real-time face recognition system. It uses a webcam to detect faces, extract embeddings with **FaceNet**, and identify students through **cosine similarity**. The output is a live display with the student’s name and a saved attendance report.

## 🎯 Goals
- Detect and identify students in real-time.
- Replace manual roll-call with automated recognition.
- Handle low-data environments (only 1–4 pictures per student).

## 📽️ Demo
▶️ Watch the system in action:  
`Application_Demo.mp4` (included in repo)

## 🛠️ Tech Stack
- **Language**: Python
- **Libraries**: TensorFlow, Keras-Facenet, OpenCV, MTCNN, NumPy
- **Models**: FaceNet, VGGFace (for experimentation)


## 🔍 Methodology
**Phase 1: CNN Classifier**  
- Custom CNN, VGG16, and MobileNet attempts  
- Severe overfitting with small dataset

**Phase 2: Embedding-Based System (Final Solution)**  
- MTCNN for face detection  
- FaceNet for 128-dim embeddings  
- Cosine similarity for identity comparison  
- Real-time webcam pipeline using OpenCV

## ✅ Features
- 📷 Real-time face detection via webcam
- 👥 Embedding matching using FaceNet
- 📊 Attendance list generated at session end
- ⚡ Lightweight and fast (runs on laptops)

## 🧪 Evaluation
- Dataset: Labeled Faces in the Wild (LFW) + 1–4 pictures/student
- Metrics: Cosine similarity thresholding, recognition rate, false positives/negatives

## 📚 Documentation
- [✔️ Final Report (PDF)](./Final_Report.docx)
- [🧠 Presentation Slides](./Final_Presentation.pptx)
- [📄 Project Proposal](./Facial_Recognition_Project_Proposal.pdf)

## 🔧 Install & Run
```bash
pip install -r requirements.txt
python src/main.py
open Untitled (1).ipynb in Jupyter.
````

## 👨‍💻 Authors
Kevin Truong – ktruong@ltu.edu
Guillermo Garcia de Celis – ggarciade@ltu.edu
