# Part 2: Computer Vision Problem Formulation and CNN Prototype

## Dataset
Synthetic Manufacturing Defect Image Dataset  
Source: Masai School Shared Drive — Part 2 folder  
480 images × 4 classes × 96×96 RGB PNG

## Problem Type
Multi-class Image Classification (4 classes: normal, scratch, dent, stain)

## Model Architecture
3-block CNN (Conv2D + MaxPool) → Flatten → Dense(256, ReLU) → Dropout(0.4) → Dense(4, Softmax)

## Results
| Metric | Value |
|---|---|
| Training Accuracy | 91.93% |
| **Testing Accuracy** | **95.83%** |
| Test Loss | 0.153 |

## Repository Structure
```
part-2-cnn-computer-vision/
├── README.md
├── notebook.ipynb
├── requirements.txt
├── sample_predictions/
│   ├── class_samples.png
│   └── prediction_outputs.png
└── results/
    ├── accuracy_loss_curves.png
    └── confusion_matrix.png
```

## How to Run
```bash
pip install -r requirements.txt
# Place part_2_cnn_computer_vision/ folder in same directory as notebook
jupyter notebook notebook.ipynb
```
