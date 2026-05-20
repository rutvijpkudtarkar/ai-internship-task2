# Image Classification Using Transfer Learning with TensorFlow

## Project Overview
This project is an image classification model built using Deep Learning and Transfer Learning.

The model classifies images from the CIFAR-10 dataset into 10 categories:
- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

## Technologies Used
- Python
- TensorFlow
- NumPy
- Matplotlib
- Scikit-learn

## Dataset
Dataset used: CIFAR-10

Loaded directly from TensorFlow:

```python
tf.keras.datasets.cifar10.load_data()
```

## Model Architecture
This project uses Transfer Learning with:
- MobileNetV2 pretrained model

Additional layers:
- GlobalAveragePooling2D
- Dense Layer
- Dropout Layer
- Softmax Output Layer

## Data Augmentation
Applied:
- Rotation
- Horizontal Flip
- Zoom

## Training Details
- Epochs: 10
- Batch Size: 32
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy

## Results
- Test Accuracy: 76%

## Evaluation Metrics
- Accuracy Score
- Confusion Matrix
- Classification Report

## Project Structure
project/
│
├── train_model.ipynb
├── saved_model/
│   └── image_classifier.keras
├── prediction.ipynb
├── requirements.txt
└── README2.md

## How to Run

Install dependencies:

```bash
pip install tensorflow matplotlib numpy scikit-learn
```

Run training notebook:

```bash
jupyter notebook train_model.ipynb
```

Run prediction:

```bash
python sample_prediction.py
```

## Author
Rutvij Kudtarkar
