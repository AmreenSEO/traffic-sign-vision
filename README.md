# 🚦 Traffic Sign Vision

A deep learning-based project for traffic sign recognition using Keras and TensorFlow. It uses a custom dataset of traffic signs organized in a structured directory and labeled using a CSV file. This project demonstrates how to preprocess image data, train a Convolutional Neural Network (CNN), and evaluate model performance.

---

## 📁 Project Structure

```
traffic-sign-vision/
├── images/ # (Currently empty or unused)
├── data/
│ ├── train/ # Training images (can be organized by class folders)
│ ├── test/ # Test images
│ └── test.csv # CSV with filenames and labels
├── traffic_sign_recognizer.ipynb # Main Jupyter Notebook
└── labels.txt # List of traffic sign class names (optional)
```

---

## 🔧 Features

- Preprocessing with `ImageDataGenerator`
- Training/validation split with real image data
- CNN model for classification
- Evaluation metrics (loss & accuracy)
- Support for both folder-structured and CSV-labeled datasets

---

## 🧠 Model

A simple CNN model is used:

- Conv2D + MaxPooling
- Dropout
- Dense layers
- Softmax activation for multi-class output

---

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy & Pandas
- Matplotlib
- Jupyter Notebook

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/traffic-sign-vision.git
   cd traffic-sign-vision
``
2. **Install dependencies**
```bash
pip install -r requirements.txt
```
3. **Run the notebook**
Open traffic_sign_recognizer.ipynb in Jupyter or VS Code and run all cells step-by-step.
---
## 📊 Dataset Notes
+ Training data is in `data/train/`

+ Test data is in `data/test/`

+ Labels for test data are found in `data/test.csv`

+ Each image should be resized to `(32, 32)` before training.
---
### ✅ To-Do
 + Add early stopping and learning rate scheduler

 + Evaluate with test set

 + Add confusion matrix and visualization

 + Export model as .h5 or TFLite

 + Improve model accuracy with data augmentation
    ---
## 🧪 Data Augmentation

To improve model generalization and performance on unseen data, the following augmentation techniques were applied using `ImageDataGenerator`:

- `rotation_range=15`
- `width_shift_range=0.1`
- `height_shift_range=0.1`
- `zoom_range=0.2`
- `horizontal_flip=True`
- `rescale=1./255`

These help the model become robust to real-world variations in traffic sign appearances.

---

## 👨‍💻 Author

**Muawiya Amir**  
AI Student & Developer  
YouTube: [@Coding_Moves](https://youtube.com/@Coding_Moves)

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

## ⭐ If you like this project, consider giving it a star!



