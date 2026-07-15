# Cats vs Dogs Image Classification using Support Vector Machine (SVM)

## Overview

This project implements a **Support Vector Machine (SVM)** to classify images of cats and dogs from the Kaggle Cats vs Dogs dataset. Images are preprocessed, resized, converted to grayscale, and transformed into **Histogram of Oriented Gradients (HOG)** features before being classified using an **RBF Kernel SVM**.

## Objective

To build an image classification model capable of distinguishing between **cats** and **dogs** using traditional machine learning techniques.

---

## Dataset

The project uses the **Kaggle Cats vs Dogs** dataset.

### Dataset Structure

```
PetImages_Small/
├── Cat/
│   ├── 0.jpg
│   ├── 1.jpg
│   └── ...
└── Dog/
    ├── 0.jpg
    ├── 1.jpg
    └── ...
```

### Dataset Used

- 5,000 Cat images
- 5,000 Dog images
- Total Images: **10,000**

---

## Technologies Used

- Python
- Google Colab
- OpenCV
- NumPy
- Matplotlib
- Scikit-learn
- scikit-image

---

## Image Preprocessing

- Resized all images to **64 × 64** pixels.
- Converted images to grayscale.
- Extracted **Histogram of Oriented Gradients (HOG)** features.
- Standardized feature vectors using **StandardScaler**.

---

## Machine Learning Model

- **Support Vector Machine (SVM)**
- **Kernel:** Radial Basis Function (RBF)
- **Feature Extraction:** HOG (Histogram of Oriented Gradients)

---

## Steps Performed

1. Imported the required libraries.
2. Loaded the Cats and Dogs image dataset.
3. Resized and converted images to grayscale.
4. Extracted HOG features from each image.
5. Split the dataset into training and testing sets.
6. Standardized the extracted features.
7. Trained the SVM classifier.
8. Predicted the class labels for the test images.
9. Evaluated the model using performance metrics.
10. Visualized the confusion matrix and sample predictions.

---

## Evaluation Metrics

The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Model Performance

| Metric | Score |
|---------|------:|
| Accuracy | **77.35%** |
| Precision | **0.77** |
| Recall | **0.77** |
| F1-Score | **0.77** |

---

## Output

The notebook generates:

- Classification Report
- Confusion Matrix
- Sample Test Image Predictions (Actual vs Predicted Labels)

---

## Project Structure

```
├── PetImages_Small/
│   ├── Cat/
│   └── Dog/
├── Cats_Dogs_SVM.ipynb
└── README.md
```

---

## Requirements

Install the required libraries:

```bash
pip install numpy opencv-python matplotlib scikit-learn scikit-image
```

---

## How to Run

1. Upload the `PetImages_Small` dataset to Google Colab.
2. Install the required libraries.
3. Run all notebook cells.
4. The SVM model will be trained on the training dataset.
5. View the classification report, confusion matrix, and prediction results.

---

## Future Improvements

- Perform hyperparameter tuning using **GridSearchCV**.
- Use color-based feature extraction.
- Compare SVM with Random Forest and K-Nearest Neighbors.
- Use deep feature extraction with **MobileNetV2** or **ResNet50** while keeping SVM as the classifier.
- Increase image resolution for richer feature representation.

---

## Results

The HOG + SVM approach achieved an overall **77.35% classification accuracy**, demonstrating that traditional machine learning techniques combined with handcrafted image features can effectively classify cats and dogs without using deep learning models.

---

## Author

**Deepak Singh**

B.Tech Computer Science and Engineering  
Dr. B.R. Ambedkar National Institute of Technology (NIT) Jalandhar
