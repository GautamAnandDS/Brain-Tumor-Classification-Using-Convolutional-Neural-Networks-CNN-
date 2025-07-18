# 🧠 Brain Tumor Classification from MRI Scans using Deep Learning

This project presents a deep learning-based solution for classifying brain MRI images into four distinct categories:

* **Glioma Tumor**
* **Meningioma Tumor**
* **Pituitary Tumor**
* **No Tumor**

Built using **DenseNet121** and advanced techniques like **transfer learning**, **data augmentation**, and **fine-tuning**, the model achieves **state-of-the-art performance** on both validation and test datasets. This work is intended to support clinical decision-making and accelerate the diagnostic workflow in medical imaging.

---

## 📂 Dataset Overview

The dataset includes T1-weighted contrast-enhanced MRI images, divided into training and test sets:

| Class      | Training Images | Testing Images |
| ---------- | --------------- | -------------- |
| Glioma     | 1,321           | 300            |
| Meningioma | 1,339           | 306            |
| Pituitary  | 1,457           | 300            |
| No Tumor   | 1,595           | 405            |

Images were preprocessed through resizing, normalization, and label encoding for optimal training conditions.

---

## 🚀 Model Highlights

* ✅ **Architecture**: Pretrained **DenseNet121** used as a base model
* 🔁 **Transfer Learning**: Leveraged pretrained weights from ImageNet
* 🧪 **Fine-Tuning**: Last 30 layers unfrozen to learn task-specific patterns
* 🔄 **Data Augmentation**: Applied to boost generalization across MRI variability
* 🧠 **Batch Normalization & Dropout**: For stable and regularized training
* ⏱️ **Early Stopping & LR Scheduling**: To avoid overfitting and manage learning rate decay

---

## 📈 Model Performance

### 🔍 Validation Set

* **Accuracy**: 95.28%
* **Loss**: 0.1501

| Class      | Precision | Recall | F1-Score |
| ---------- | --------- | ------ | -------- |
| No Tumor   | 0.98      | 0.99   | 0.98     |
| Glioma     | 0.95      | 0.95   | 0.95     |
| Meningioma | 0.94      | 0.89   | 0.92     |
| Pituitary  | 0.93      | 0.98   | 0.95     |

---

### 🧾 Test Set

* **Accuracy**: 97.03%

| Class      | Precision | Recall | F1-Score |
| ---------- | --------- | ------ | -------- |
| No Tumor   | 0.99      | 1.00   | 0.99     |
| Glioma     | 0.98      | 0.92   | 0.95     |
| Meningioma | 0.92      | 0.97   | 0.94     |
| Pituitary  | 0.98      | 0.97   | 0.97     |

---

## 💾 Model Export

The trained model is saved as:

```bash
Brain_Tumor_Scanner_MRI.h5
```

Easily load it using:

```python
from tensorflow.keras.models import load_model
model = load_model('Brain_Tumor_Scanner_MRI.h5')
```

---

## 💡 Business & Clinical Impact

* 🔬 **Faster Diagnosis**: Assists radiologists in quickly identifying tumor types
* 🌍 **Scalability**: Can be deployed in hospitals, cloud systems, or edge devices
* 📉 **Operational Efficiency**: Reduces workload on medical professionals, especially in underserved regions
* 📡 **Remote Healthcare**: Supports telemedicine by enabling remote, automated MRI analysis

---

## 🛠️ Tech Stack

* **Python**, **TensorFlow/Keras**
* **OpenCV**, **Matplotlib**, **Seaborn**
* **Scikit-learn**
* **DenseNet121 (Transfer Learning)**

---

## 📌 Project Status

✅ Model development, tuning, and evaluation completed

✅ Achieved 97% test accuracy

✅ Model ready for deployment or integration into diagnostic pipelines

---

## 👋 Contact

For questions, collaborations, or job opportunities:

📧 [anandgautam023@gmail.com](anandgautam023@gmail.com)
💼 [LinkedIn](https://www.linkedin.com/in/gautam-anand-ds/)

---

