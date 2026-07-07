# 🌿 Groundnut Leaf Disease Detection using Deep Learning

## 📌 Project Overview

Groundnut (Peanut) is one of the most important oilseed crops, but its productivity is greatly affected by various leaf diseases. Early detection of these diseases helps farmers take timely preventive measures and reduce crop losses.

This project uses **Deep Learning** with **Transfer Learning (MobileNetV2)** to automatically classify groundnut leaf images into different disease categories.

---

## 🎯 Objectives

- Detect groundnut leaf diseases using image classification.
- Improve disease diagnosis using Deep Learning.
- Assist farmers with early disease identification.
- Compare model performance using evaluation metrics.

---

## 🦠 Disease Classes

The model classifies images into the following categories:

1. Healthy Leaf
2. Early Leaf Spot
3. Late Leaf Spot
4. Rust
5. Early Rust
6. Nutrition Deficiency

---

## 📂 Dataset

**Source:** Kaggle Groundnut Leaf Disease Dataset

Dataset contains images of:

- Healthy leaves
- Diseased leaves
- Multiple disease categories

### Dataset Structure

```
dataset/
│
├── train/
│   ├── healthy_leaf/
│   ├── early_leaf_spot/
│   ├── late_leaf_spot/
│   ├── rust/
│   ├── early_rust/
│   └── nutrition_deficiency/
│
├── validation/
│
└── test/
```

---

## 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- MobileNetV2
- NumPy
- Pandas
- Matplotlib
- OpenCV
- Scikit-learn
- Google Colab / Jupyter Notebook

---

## 🧠 Deep Learning Model

Transfer Learning Model:

- MobileNetV2
- ImageNet Pretrained Weights

Additional Layers:

- Global Average Pooling
- Dense Layer
- Dropout
- Softmax Output Layer

---

## ⚙️ Training Configuration

| Parameter | Value |
|-----------|-------|
| Image Size | 128 × 128 |
| Batch Size | 32 |
| Epochs | 20 |
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Learning Rate | 0.001 |

---

## 🔄 Data Preprocessing

- Image resizing
- Image normalization
- Data augmentation
  - Rotation
  - Horizontal Flip
  - Zoom
  - Shear
  - Width Shift
  - Height Shift

---

## 📈 Evaluation Metrics

The model is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## 📊 Workflow

```
Groundnut Leaf Images
          │
          ▼
Data Preprocessing
          │
          ▼
Image Augmentation
          │
          ▼
Train / Validation Split
          │
          ▼
MobileNetV2 Transfer Learning
          │
          ▼
Model Training
          │
          ▼
Prediction
          │
          ▼
Disease Classification
```

---

## 📁 Project Structure

```
Groundnut-Leaf-Disease-Detection/
│
├── dataset/
├── notebooks/
│   └── Groundnut_Disease_Detection.ipynb
│
├── models/
│   └── mobilenetv2_model.h5
│
├── images/
│
├── results/
│   ├── accuracy.png
│   ├── loss.png
│   ├── confusion_matrix.png
│   └── predictions.png
│
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Groundnut-Leaf-Disease-Detection.git
```

Move into the project folder

```bash
cd Groundnut-Leaf-Disease-Detection
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

Open the notebook

```bash
jupyter notebook
```

or

```bash
python predict.py
```

---

## 📷 Sample Predictions

| Input Image | Predicted Disease |
|-------------|------------------|
| Healthy Leaf | Healthy |
| Rust Leaf | Rust |
| Early Leaf Spot | Early Leaf Spot |
| Nutrition Deficiency | Nutrition Deficiency |

---

## 📌 Future Improvements

- Deploy using Streamlit or Flask
- Mobile Application for farmers
- Real-time disease detection
- Increase dataset size
- Use EfficientNet or Vision Transformer (ViT)
- Improve model accuracy with hyperparameter tuning

---

## 👨‍💻 Author

**Soubhagya Ranjan Mishra**

B.Tech CSE (Data Analytics & Machine Learning)

Centurion University of Technology and Management

---

## ⭐ If you found this project useful, don't forget to Star the repository!
