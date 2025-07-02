# 🧠 Project AI – Image Classification with Transfer Learning

This project is a deep learning-based image classification system built using **TensorFlow** and **Keras**, focusing on leveraging **transfer learning** with pre-trained models: **ResNet50**, **DenseNet121**, and **MobileNetV3Small**.

It processes a set of labeled images, augments training data, builds multiple CNN architectures, and evaluates classification performance across different models.

---

## 📂 Project Structure

Project-AI/
├── ProjectAIFInalized.ipynb # Main notebook
├── updated_images/ # Folder with train, valid, test datasets
│ ├── train/
│ ├── valid/
│ └── test/
├── requirements.txt # (You can create this based on the packages below)
└── README.md # This file

yaml
Copy
Edit

---

## ⚙️ Models Implemented

Each model uses frozen convolutional base layers from ImageNet and a custom top classifier:

- ✅ **ResNet50**
- ✅ **DenseNet121**
- ✅ **MobileNetV3Small**

Each model includes:
- `GlobalAveragePooling2D`
- `BatchNormalization`
- `Dropout`
- `Dense` output layer with softmax

---

## 🛠️ Setup Instructions

1. **Install Required Packages**

```bash
pip install tensorflow numpy matplotlib seaborn scikit-learn h5py
Prepare Dataset

Your dataset should be organized like this:

bash
Copy
Edit
updated_images/
├── train/
│   ├── class_1/
│   ├── class_2/
│   └── ...
├── valid/
│   ├── class_1/
│   ├── class_2/
│   └── ...
└── test/
    ├── class_1/
    ├── class_2/
    └── ...
Run the Notebook

Open ProjectAIFInalized.ipynb in Jupyter or Google Colab, then execute all cells.

📈 Evaluation Metrics
Each model is evaluated using:

Accuracy on test set

Confusion matrix

Classification report (precision, recall, F1-score)

Visualization using matplotlib and seaborn

📊 Sample Output
text
Copy
Edit
Classes: {'cat': 0, 'dog': 1, ...}
Test Accuracy: 94.2%
Confusion Matrix:
[ [87, 3],
  [5, 85] ]
✍️ Author
Ikhwan Tukiran
