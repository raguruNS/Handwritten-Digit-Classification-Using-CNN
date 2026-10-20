# Project 11: Handwritten Digit Classification Using CNN

## 📌 Project Overview

This project implements a Convolutional Neural Network (CNN) to classify handwritten digits using the MNIST dataset. The model recognizes digits from 0 to 9 by learning visual patterns from grayscale images.

The project demonstrates image preprocessing, CNN architecture, model training, performance evaluation, and handwritten digit prediction using Python and TensorFlow/Keras.

## 🎯 Objectives

- Load and preprocess the MNIST handwritten digit dataset.
- Build a CNN model using convolutional and pooling layers.
- Train the model to classify handwritten digits.
- Evaluate model performance using accuracy and loss.
- Generate a confusion matrix and classification report.
- Display sample predictions with actual and predicted labels.
- Save the trained model for future use.

## 📊 Dataset

The MNIST dataset contains 70,000 grayscale images of handwritten digits.

| Feature | Description |
|---|---|
| Total images | 70,000 |
| Training images | 60,000 |
| Testing images | 10,000 |
| Image dimensions | 28 × 28 pixels |
| Image type | Grayscale |
| Number of classes | 10 |
| Classes | Digits 0–9 |

The dataset is loaded directly using `tensorflow.keras.datasets.mnist`.

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook / Google Colab

## 🧠 CNN Architecture

The model consists of the following layers:

1. **Input Layer:** Accepts 28 × 28 grayscale images.
2. **Convolutional Layer 1:** Extracts image features using 32 filters.
3. **Max Pooling Layer 1:** Reduces feature-map dimensions.
4. **Convolutional Layer 2:** Extracts more complex features using 64 filters.
5. **Max Pooling Layer 2:** Further reduces feature-map dimensions.
6. **Flatten Layer:** Converts feature maps into a one-dimensional vector.
7. **Dense Layer:** Learns patterns using 128 neurons and ReLU activation.
8. **Dropout Layer:** Reduces overfitting with a dropout rate of 0.3.
9. **Output Layer:** Uses 10 neurons and softmax activation to classify digits from 0 to 9.

### Model Configuration

- **Optimizer:** Adam
- **Loss Function:** Sparse Categorical Crossentropy
- **Evaluation Metric:** Accuracy
- **Batch Size:** 128
- **Epochs:** 5
- **Validation Split:** 10%

## ⚙️ Installation

Install the required libraries:

```bash
pip install tensorflow numpy matplotlib scikit-learn seaborn
```

Alternatively, open the notebook in Google Colab, where these libraries are generally available.

## 🚀 How to Run the Project

1. Clone or download this repository.
2. Open `handwritten_digit_classification.ipynb` in Jupyter Notebook or Google Colab.
3. Install any missing dependencies.
4. Run the notebook cells in sequence.
5. Load and preprocess the MNIST dataset.
6. Build and train the CNN model.
7. Evaluate the model on the test dataset.
8. Generate the confusion matrix and classification report.
9. Visualize sample predictions.
10. Save the trained model as `mnist_cnn_model.keras`.

## 📈 Model Evaluation

The model is evaluated using the following techniques:

### 1. Accuracy and Loss
Measures the model's overall classification performance on unseen test images.

### 2. Confusion Matrix
Shows correct predictions and misclassifications for each digit class.

### 3. Classification Report
Provides:
- **Precision:** Proportion of correct predictions among predicted instances of a class.
- **Recall:** Proportion of actual instances correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **Support:** Number of actual samples in each class.

### 4. Sample Predictions
Displays handwritten test images with their actual and predicted digit labels.

## 📁 Project Structure

```text
Project-11-MNIST-CNN/
│
├── handwritten_digit_classification.ipynb
├── mnist_cnn_model.keras
├── README.md
└── requirements.txt
```

## ✅ Expected Results

After successfully running the notebook, the project generates:

- A trained CNN model for handwritten digit classification.
- Training and validation accuracy/loss graphs.
- Test accuracy and loss.
- A confusion matrix.
- A classification report.
- Sample digit predictions.
- A saved model file for future use.

Actual performance metrics should be recorded after executing the notebook.

## 🎓 Learning Outcomes

By completing this project, students will understand:

- Image preprocessing and pixel normalization.
- The fundamentals of convolutional neural networks.
- Feature extraction using convolutional layers.
- Dimensionality reduction using max pooling.
- Multiclass image classification.
- Model evaluation using classification metrics.
- Visualization of model predictions.
- Saving and loading trained deep learning models.

## 🏁 Conclusion

This project demonstrates how CNNs can recognize handwritten digits using deep learning. The MNIST dataset provides a practical introduction to image classification, while the confusion matrix and classification report help analyze the model's strengths and errors.

The project establishes a foundation for more advanced computer vision applications, including object recognition, character recognition, and image classification.

## 👨‍💻 Author

**Name:** Nitheesh

**Project:** Deep Learning – Project 11

**Topic:** Handwritten Digit Classification Using CNN
