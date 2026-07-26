#  AI Personal Stylist

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-MediaPipe-green.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange.svg)
![RAG](https://img.shields.io/badge/RAG-FAISS-purple.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

##  Overview

**AI Personal Stylist** is an AI-powered fashion recommendation system that analyzes a user's body proportions from an image and generates personalized outfit recommendations.

The project combines **Computer Vision**, **Machine Learning**, **Similarity Search (FAISS)**, and **Large Language Models (Gemini)** to build a Retrieval-Augmented Generation (RAG) pipeline for intelligent fashion styling.

---

##  Features

-  Body landmark detection using **MediaPipe Pose**
-  Automatic body measurement and feature extraction
-  Feature engineering and dimensionality reduction (PCA)
-  Similar body-type retrieval using **FAISS**
-  Fashion knowledge base creation from DeepFashion2
-  RAG-based personalized fashion recommendations using Gemini
-  End-to-end recommendation pipeline

---

##  Project Structure

```
AI_Personal_Stylist/
│
├── datasets/
│   ├── landmarks.csv
│   ├── features.csv
│   ├── body_features_with_metadata.csv
│   ├── knowledge_base.csv
│   └── fashion_knowledge_base.csv
│
├── models/
│   ├── faiss_index.bin
│   ├── metadata.pkl
│   ├── scaler.pkl
│   ├── pca.pkl
│   ├── training_features.pkl
│   └── category_encoder.pkl
│
├── notebooks/
│   ├── 00_Run_Entire_Pipeline.ipynb
│   ├── 01_Pose_Detection.ipynb
│   ├── 02_Feature_Engineering.ipynb
│   ├── 03_Parse_DeepFashion2.ipynb
│   ├── 04_Knowledge_Base.ipynb
│   └── 05_AIStylist_RAG.ipynb
│
├── requirements.txt
├── fashion_knowledge_base.csv
└── .gitignore
```

---

##  Workflow

```
Input Image
      │
      ▼
MediaPipe Pose Detection
      │
      ▼
Body Landmark Extraction
      │
      ▼
Feature Engineering
      │
      ▼
Scaling + PCA
      │
      ▼
FAISS Similarity Search
      │
      ▼
Retrieve Similar Fashion Knowledge
      │
      ▼
Gemini (RAG)
      │
      ▼
Personalized Outfit Recommendations
```

---

##  Technologies Used

### Programming

- Python

### Computer Vision

- OpenCV
- MediaPipe

### Machine Learning

- Scikit-learn
- PCA
- StandardScaler

### Similarity Search

- FAISS

### LLM & RAG

- Google Gemini API

### Data Processing

- NumPy
- Pandas

### Visualization

- Matplotlib

---

##  Datasets

This project uses:

- DeepFashion2 Dataset
- Custom body feature dataset
- Fashion knowledge base

---

##  Installation

Clone the repository

```bash
git clone https://github.com/<your-username>/AI_Personal_Stylist.git

cd AI_Personal_Stylist
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

##  Running the Project

Open the notebook:

```
notebooks/00_Run_Entire_Pipeline.ipynb
```

Run all cells sequentially.

The pipeline performs:

1. Pose Detection
2. Body Feature Extraction
3. Feature Engineering
4. PCA Transformation
5. FAISS Retrieval
6. Knowledge Base Search
7. AI-powered Fashion Recommendation

---

##  Models

The project includes pre-trained artifacts:

- StandardScaler
- PCA
- FAISS Index
- Metadata
- Feature Embeddings
- Category Encoder

No model retraining is required for inference.

---

##  Sample Output

### Input

![pretty-young-woman](images/pretty-young-woman.avif)

### Final Fashion Recommendation

![Gemini recommendation1](images/Gemini recommendation1.png)

---

##  Future Improvements

- Streamlit Web Application
- Multi-person image support
- Seasonal recommendations
- Shopping link integration
- Explainable AI recommendations
- Fine-tuned Fashion LLM
- Virtual Try-On Integration


---

##  Author
**Riya Dey**  
*National Institute of Technology Durgapur*  

📧 [Email](mailto:riyadey3134@gmail.com)  
🌐 [LinkedIn](https://www.linkedin.com/in/riya-dey-a31b43286)
