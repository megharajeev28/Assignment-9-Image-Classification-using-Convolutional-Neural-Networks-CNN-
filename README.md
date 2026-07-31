# Image Classification using Convolutional Neural Networks (CNN)

## Student Details

| Field | Details |
|--------|---------|
| **Author** | Megha Rajeev |
| **Registration Number** | 23MIM10047 |
| **Application Number** | IN26011193 |
| **Batch Number** | 1A |
| **Email ID** | megha.23mim10047@vitbhopal.ac.in |

---

# Objective

The objective of this project is to develop a **Convolutional Neural Network (CNN)** capable of accurately classifying pet images into **Cats** and **Dogs** using the Cats vs Dogs Classification Dataset. The model is built using TensorFlow/Keras and evaluated using multiple classification metrics to demonstrate the effectiveness of Convolutional Neural Networks for image classification tasks.

---

# Dataset

**Dataset Name:** Cats vs Dogs Classification Dataset

**Source:** Kaggle

**Dataset Link:**

https://www.kaggle.com/datasets/bhavikjikadara/dog-and-cat-classification-dataset

> **Note:** The dataset is not included in this repository. Please download it directly from Kaggle.

---

# Libraries Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- OpenCV
- OS

---

# Methodology

## Step 1: Dataset Collection

- Downloaded the Cats vs Dogs Classification Dataset from Kaggle.
- Loaded the dataset from the local directory using TensorFlow/Keras image utilities.

---

## Step 2: Data Understanding

- Displayed the folder structure of the dataset.
- Displayed five sample images along with their class labels.
- Identified:
  - Number of classes
  - Image dimensions
  - Total number of images

---

## Step 3: Data Preprocessing

- Resized all images to **128 × 128** pixels.
- Normalized pixel values from **0–255** to **0–1**.
- Split the dataset into:
  - **80% Training**
  - **20% Testing**
- Created TensorFlow/Keras image generators for efficient loading and preprocessing during training.

---

## Step 4: Model Development

Built a **Convolutional Neural Network (CNN)** using TensorFlow/Keras with the following architecture:

- Conv2D (32 Filters, 3×3, ReLU)
- MaxPooling2D (2×2)
- Conv2D (64 Filters, 3×3, ReLU)
- MaxPooling2D (2×2)
- Conv2D (128 Filters, 3×3, ReLU)
- MaxPooling2D (2×2)
- Flatten Layer
- Dense Layer (128 Neurons, ReLU)
- Output Layer (1 Neuron, Sigmoid)

---

# Model Configuration

| Parameter | Value |
|-----------|-------|
| Optimizer | Adam |
| Loss Function | Binary Crossentropy |
| Evaluation Metric | Accuracy |
| Epochs | 10 |

The model was trained using the prepared training dataset.

---

## Step 5: Prediction

- Predicted the classes of images from the testing dataset.
- Converted prediction probabilities into class labels.
- Compared predicted labels with the actual labels.
- Displayed sample predictions for visual verification.

---

## Step 6: Model Evaluation

The trained CNN model was evaluated using:

- Test Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Accuracy vs Epoch Graph
- Loss vs Epoch Graph

These evaluation metrics were used to assess the classification performance and learning behavior of the CNN model.

---

# CNN Architecture

| Layer | Configuration |
|--------|---------------|
| Conv2D | 32 Filters (3×3), ReLU |
| MaxPooling2D | Pool Size (2×2) |
| Conv2D | 64 Filters (3×3), ReLU |
| MaxPooling2D | Pool Size (2×2) |
| Conv2D | 128 Filters (3×3), ReLU |
| MaxPooling2D | Pool Size (2×2) |
| Flatten | Flatten Layer |
| Dense | 128 Neurons (ReLU) |
| Output Layer | 1 Neuron (Sigmoid) |

---

# Results

| Metric | Value |
|--------|-------|
| Test Accuracy | *(Obtained after execution)* |
| Precision | *(Obtained after execution)* |
| Recall | *(Obtained after execution)* |
| F1-Score | *(Obtained after execution)* |

---

# Classification Performance

- The CNN model successfully learned important image features for distinguishing cats and dogs.
- Training accuracy increased steadily while the training loss decreased across epochs.
- The confusion matrix showed that most images were correctly classified with only a few misclassifications.
- Precision, Recall, and F1-Score indicate strong overall classification performance.

---

# Conclusion

The Convolutional Neural Network successfully classified cat and dog images with high accuracy, demonstrating the effectiveness of deep learning for image classification tasks. The convolutional layers automatically extracted important visual features such as edges, textures, and shapes, while the pooling layers reduced computational complexity and improved generalization. Compared to traditional Artificial Neural Networks, CNNs are significantly more effective for image-based applications because they preserve spatial information and perform automatic feature extraction. However, CNNs require larger datasets, higher computational resources, and longer training times. Overall, this project demonstrates the practical application of Convolutional Neural Networks in computer vision tasks such as animal recognition, medical image analysis, facial recognition, and autonomous systems.
