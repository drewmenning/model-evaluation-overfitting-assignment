# model-evaluation-overfitting-assignment

## Overview
This project compares a baseline neural network and an improved neural network on the Fashion-MNIST dataset. The goal is to show how proper data splitting and overfitting mitigation techniques improve model generalization.

## Dataset
- Fashion-MNIST
- 10 grayscale image classes
- 28x28 images

## Data Splitting
The dataset was split into:
- 70% training
- 15% validation
- 15% testing

I used `train_test_split` with:
- `stratify` to preserve class balance
- `random_state=42` for reproducibility

## Models
### Baseline Model
- Flatten layer
- Dense hidden layer
- Softmax output layer

### Improved Model
- Convolutional layers
- L1/L2 regularization
- Data augmentation
- Dropout
- Batch normalization
- Early stopping

## Results Summary
The improved model performed better on the validation and test sets than the baseline model. It also showed better generalization by reducing overfitting and narrowing the gap between training and validation performance.

## Main Findings
- Stratified splitting made evaluation more reliable
- Dropout and regularization helped reduce overfitting
- Data augmentation improved robustness
- Early stopping prevented unnecessary training after validation performance stopped improving

## Files Included
- `m12_assignment.ipynb`
- `README.md`
