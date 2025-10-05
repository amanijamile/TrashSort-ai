# TrashSort-ai
Deep learning-based automated waste classification system using Convolutional Neural Networks (CNN) trained on the TrashNet dataset. Includes an interactive image classifier and recycling FAQ chatbot.

# ♻️ TrashSort AI – Automated Waste Classification

A deep learning project that classifies household waste images into six categories using a **Convolutional Neural Network (CNN)**.  
Built and trained on the [TrashNet dataset](https://github.com/garythung/trashnet.git), this model assists in automating waste sorting and promoting recycling awareness.

---

## 🧩 Overview
Effective waste management is critical for sustainability.  
This project implements a custom CNN trained to recognize six classes of waste:
`cardboard`, `glass`, `metal`, `paper`, `plastic`, and `trash`.

It also includes:
- 🖼️ **Waste Classification Interface** — Upload an image to get predictions and bin suggestions  
- 💬 **Recycling FAQ Chatbot** — Ask recycling-related questions powered by semantic search

---

## 🧠 Model & Methods
- **Frameworks:** TensorFlow / Keras, scikit-learn, OpenCV  
- **Dataset:** [TrashNet](https://github.com/garythung/trashnet) (2,520 labeled images)  
- **Preprocessing:**  
  - Image resizing (128×128×3)  
  - Normalization (0–1 scaling)  
  - Data augmentation (rotation, shift, zoom, flip)  
- **Architecture:**  
  4 convolutional blocks → Dense(512) → Dropout(0.5) → Softmax(6)  
- **Validation Accuracy:** 71.08%

---

## ⚙️ Installation & Setup

```bash
# Clone this repository
git clone https://github.com/yourusername/trashsort-ai.git
cd trashsort-ai

# Install dependencies
pip install tensorflow opencv-python scikit-learn matplotlib sentence-transformers ipywidgets
