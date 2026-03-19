# Bell Pepper Disease Classification using Deep Learning

## Overview

This project builds a **Convolutional Neural Network (CNN)** model to classify **bell pepper leaf diseases** from images.

The model predicts one of the following classes:

* Blight
* Spot
* Virus
* Healthy

It uses image processing and deep learning techniques to assist in **early disease detection in agriculture**.

---

## Dataset

The dataset is **not included in this repository** due to its large size.

It is stored in Google Drive and accessed in the code using:

```
data_dir = "/content/drive/MyDrive/Bell_Pepper_Project/dataset"
```

### Dataset Structure

Your dataset must be organized like this:

```
dataset/
   Blight/
   Spot/
   Virus/
   Healthy/
```

Each folder should contain images of the respective class.

---

## How to Use Dataset

1. Upload your dataset to Google Drive
2. Place it inside:

```
MyDrive/Bell_Pepper_Project/dataset
```

3. Mount Google Drive in Colab:

```python
from google.colab import drive
drive.mount('/content/drive')
```

4. Use this path in your code:

```python
data_dir = "/content/drive/MyDrive/Bell_Pepper_Project/dataset"
```

---

## Features

* Image classification using CNN
* Data augmentation (rotation, zoom, flipping)
* Class imbalance handling using class weights
* Model evaluation using:

  * Accuracy
  * Confusion Matrix
  * Classification Report
  * Cohen’s Kappa Score
* Feature map visualization (understanding model behavior)

---

## Model Architecture

The model consists of:

* Convolutional layers (feature extraction)
* MaxPooling layers (dimension reduction)
* Dropout layers (prevent overfitting)
* Dense layers (classification)
* Softmax output layer (multi-class prediction)

---

## Training Details

* Image size: 128 × 128
* Batch size: 32
* Epochs: 20
* Optimizer: Adam
* Loss function: Categorical Crossentropy

---

## Evaluation Metrics

The model is evaluated using:

* Accuracy
* Precision, Recall, F1-score (Classification Report)
* Confusion Matrix
* Cohen’s Kappa Score

---

## Example Prediction

The model takes an image input and outputs:

* Predicted class (e.g., Blight)
* Confidence score (e.g., 95%)

---

## Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## Future Improvements

* Use Transfer Learning (ResNet, MobileNet)
* Deploy as a web application
* Real-time disease detection system
* Mobile app integration

---

## Author

**Suvedha T**
B.E Computer Science and Engineering
Specialization: Artificial Intelligence and Machine Learning

---

## License

This project is licensed under the MIT License.
