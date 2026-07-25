# Cat vs Dog Image Classification using CNN and VGG16

## Overview

This project implements image classification for cats and dogs using Deep Learning.

Two approaches are explored:

- A Convolutional Neural Network (CNN) built from scratch.
- Transfer Learning using the pretrained VGG16 model.

The notebook demonstrates dataset preparation, image preprocessing, model training, evaluation, and performance comparison.

---

## Features

- Dataset preparation and train/validation/test split
- Image preprocessing using ImageDataGenerator
- CNN built from scratch
- Transfer Learning using VGG16
- Model evaluation using Confusion Matrix
- Accuracy and Loss visualization
- Model saving for future inference

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn
- Pillow
- Jupyter Notebook

---

## Dataset

Download the dataset from Kaggle:

https://www.kaggle.com/datasets/karakaggle/kaggle-cat-vs-dog-dataset

Project structure after extraction:

```
Cat_Dog/
│
└── dataset/
    ├── Cat/
    └── Dog/
```

The notebook automatically creates the `train`, `valid`, and `test` directories.

---

## Model Architecture

### CNN

- Conv2D
- MaxPooling2D
- Conv2D
- MaxPooling2D
- Flatten
- Dense (Softmax)

### Transfer Learning

- Pretrained VGG16
- Frozen convolutional layers
- Custom Dense output layer
- Softmax classifier

---

## Results

### CNN

- Training Accuracy: ~100%
- Validation Accuracy: ~69%

### VGG16

- Training Accuracy: ~98%
- Validation Accuracy: ~97%.

Transfer Learning significantly outperformed the custom CNN on this dataset.

---

## Future Improvements

- Data augmentation
- EarlyStopping
- ModelCheckpoint
- Hyperparameter tuning
- MobileNet/EfficientNet comparison

---

## How to Run

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Install dependencies.

```bash
pip install -r requirements.txt
```

3. Download the Kaggle dataset.

4. Place it inside

```
dataset/
├── Cat
└── Dog
```

5. Run the notebook.

---
