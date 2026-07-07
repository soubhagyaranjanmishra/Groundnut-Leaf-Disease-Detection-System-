# 🌿 Groundnut Leaf Disease Detection using Deep Learning

A Deep Learning-based image classification system that detects diseases in groundnut (peanut) leaves using **Transfer Learning (MobileNetV2)**. The model classifies leaf images into multiple disease categories and healthy leaves, enabling early disease detection for precision agriculture.

---

## 📌 Project Overview

Groundnut is one of the major oilseed crops, and its yield is significantly affected by fungal diseases and nutrient deficiencies. Early identification of these diseases helps farmers take timely preventive measures.

This project uses **MobileNetV2**, a lightweight pre-trained Convolutional Neural Network (CNN), to classify groundnut leaf images into different disease categories.

---

## 🎯 Features

- Image-based disease detection
- Transfer Learning using MobileNetV2
- Data Augmentation
- Multi-class Image Classification
- Model Evaluation using Accuracy, Precision, Recall & F1-Score
- Ready-to-use trained model (.h5)

---

## 🦠 Disease Classes

The dataset contains six classes:

- 🌱 Healthy Leaf
- 🍂 Early Leaf Spot
- 🍁 Late Leaf Spot
- 🟤 Rust
- 🟡 Nutrition Deficiency
- 🌿 Early Rust *(if available in your dataset)*

---

## 📂 Dataset

The complete dataset is included in this repository.

Dataset Structure

```
Groundnut-Leaf-Disease-Detection-System/
│
├── healthy leaf/
├── early_leaf_spot/
├── late leaf spot/
├── rust/
├── nutrition deficiency/
│
├── Background Masking.ipynb
├── MOBILENET V2 IMPLEMENTATION.ipynb
├── Final MOBILENET V2 IMPLEMENTATION.ipynb
├── best_groundnut_model.h5
├── README.md
```

---

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- MobileNetV2
- NumPy
- Pandas
- OpenCV
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## 🧠 Model Architecture

**Base Model**

- MobileNetV2 (ImageNet Weights)

**Custom Layers**

- GlobalAveragePooling2D
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

---

## 🔄 Data Preprocessing

- Image Resizing
- Normalization
- Data Augmentation
  - Rotation
  - Horizontal Flip
  - Zoom
  - Width Shift
  - Height Shift
  - Shear

---

## 📈 Model Evaluation

The model performance is evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## 🚀 Workflow

```
Leaf Image
     │
     ▼
Image Preprocessing
     │
     ▼
Data Augmentation
     │
     ▼
MobileNetV2
     │
     ▼
Model Training
     │
     ▼
Prediction
     │
     ▼
Disease Class
```

---

## 📁 Project Structure

```
Groundnut-Leaf-Disease-Detection-System/
│
├── .git/
├── healthy leaf/
├── early_leaf_spot/
├── late leaf spot/
├── rust/
├── nutrition deficiency/
│
├── Background Masking.ipynb
├── MOBILENET V2 IMPLEMENTATION.ipynb
├── Final MOBILENET V2 IMPLEMENTATION.ipynb
├── best_groundnut_model.h5
├── README.md
```

---

## 📦 Installation

Clone the repository

```bash
git clone https://github.com/soubhagyaranjanmishra/Groundnut-Leaf-Disease-Detection-System-.git
```

Move into the project directory

```bash
cd Groundnut-Leaf-Disease-Detection-System-
```

Install dependencies

```bash
pip install tensorflow keras numpy pandas matplotlib opencv-python scikit-learn
```

---

## ▶️ Running the Project

Open the notebook

```bash
jupyter notebook
```

Run

```
Final MOBILENET V2 IMPLEMENTATION.ipynb
```

or load the trained model

```python
from tensorflow.keras.models import load_model

model = load_model("best_groundnut_model.h5")
```

---

## 📊 Results

The trained MobileNetV2 model successfully classifies groundnut leaf images into different disease categories.

Evaluation Metrics include:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 📌 Future Enhancements

- Streamlit Web Application
- Flask API Deployment
- Mobile Application
- Real-time Camera Detection
- Larger Dataset
- EfficientNet / Vision Transformer (ViT)

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Push the branch.
5. Create a Pull Request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Soubhagya Ranjan Mishra**

B.Tech (Computer Science & Engineering)

Data Analytics & Machine Learning

Centurion University of Technology and Management

GitHub: https://github.com/soubhagyaranjanmishra

---

⭐ If you found this project useful, please consider giving it a Star.
