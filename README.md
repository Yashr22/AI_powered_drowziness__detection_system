#  Eye Open/Close Detection using Deep Learning

This project implements a **Convolutional Neural Network (CNN)** to classify whether a person’s eyes are **Open** or **Closed** using image data.  
The model serves as a core component for **AI-powered drowsiness detection systems**.

---

##  Project Overview

Detecting eye closure is a critical step in fatigue and drowsiness monitoring systems used in:

-  Driver safety systems  

This notebook demonstrates:

✔ Data preprocessing  
✔ CNN model training  
✔ Validation & evaluation  
✔ Saving trained models  

---

## Dataset Structure

data/
└── archive/
└── train/
├── Closed_Eyes/
└── Open_Eyes/


###  Classes
- `Closed_Eyes`
- `Open_Eyes`

---

## Technologies Used

- Python 🐍  
- TensorFlow / Keras  
- NumPy & Pandas  
- Matplotlib  
- Jupyter Notebook  

---

## Model Architecture

The CNN model includes:

- Convolutional layers  
- MaxPooling layers  
- Batch Normalization  
- Dropout (prevents overfitting)  
- Fully connected Dense layers  
- Softmax output layer  

### Input Shape


---

## Workflow

### 1️⃣ Data Loading
- Uses `image_dataset_from_directory`
- Automatic train/validation split (80/20)

### 2️⃣ Preprocessing
- Resizing images to 84×84  
- Normalization  
- Batching  

### 3️⃣ Model Training
- CNN learns eye features  
- Validation used to monitor performance  

### 4️⃣ Model Saving
Trained models saved as:

model/eye_detection_model.keras
model/eye_detection_model2.keras

---

## Output

The model predicts:

Closed_Eyes
Open_Eyes


Used later in real-time systems for:

- Blink detection  
- Drowsiness monitoring  
- Attention tracking  

---

## ▶How to Run

### Install dependencies
```bash
pip install -r requirements.txt
