# 🧠 Brain Tumor Classification using Deep Learning

This project implements a deep learning model using **Keras Sequential API** to classify brain MRI images into two categories:

* `0`: Normal (No tumor)
* `1`: Diseased (Tumor present)

---

## 📁 Dataset

The dataset consists of brain MRI images pre-labeled as either normal or tumorous. Images are preprocessed for input into a convolutional neural network.

> 📌 *Ensure your dataset is organized into two folders within a `train/` and `test/` directory, e.g.:*

```
data/
🔺 train/
🔺🔺 0/   # Normal images
🔺🔺 1/   # Tumor images
🔺 test/
🔺🔺 0/
🔺🔺 1/
```

---

## 🧪 Methodology

### ✅ Preprocessing

* Image resizing and normalization
* Data augmentation using `ImageDataGenerator`

### 🧠 Model Architecture

* Built using **Keras Sequential API**
* Layers:

  * Conv2D → MaxPooling → Dropout
  * Flatten → Dense → Dropout → Output (sigmoid)
* Binary classification (`0`: Normal, `1`: Tumor)

### ⚙️ Loss & Optimizer

* **Loss Function:** `binary_crossentropy`
* **Optimizer:** `adam`
* **Metrics:** `accuracy`

---

## 📈 Training and Evaluation

* Trained over several epochs on training data
* Validation performed on test data
* Accuracy and loss curves plotted
* Confusion matrix and classification report included

---

## 🧠 Requirements

Install the required dependencies using:

```bash
pip install -r requirements.txt
```

Basic dependencies include:

* `tensorflow` (or `keras`)
* `numpy`
* `matplotlib`
* `sklearn`
* `opencv-python` (optional for manual preprocessing)

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/yourusername/brain-tumor-classification.git
cd brain-tumor-classification
```

2. Run the notebook:

```bash
jupyter notebook Brain_tumor_data_image_processing.ipynb
```

---

## 📊 Results

* Achieved **XX%** validation accuracy (replace with actual)
* Confusion matrix and classification metrics shown in the notebook

---

## 📌 Future Improvements

* Implement transfer learning using pre-trained models (e.g., VGG16, ResNet50)
* Hyperparameter tuning using `KerasTuner` or `Optuna`
* Deploy model as a web app using `Streamlit` or `Flask`

---


