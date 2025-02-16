# IC Counterfeit Detection

This repository contains a deep learning-based approach for detecting counterfeit ICs using PyTorch and ResNet101.

## **Project Overview**
- The project is divided into two phases:
  1. **Phase 1 (Training and Testing on Seen Data)**: Train a ResNet101 model on a dataset of IC images.
  2. **Phase 2 (Testing on Unseen Data)**: Evaluate model performance on a separate test dataset.

## **Files in this Repository**
- **`train_test_seen.py`**: Script for training and testing the model on the seen dataset.
- **`test_unseen.py`**: Script for evaluating the trained model on unseen data.
- **`model.pth`**: Trained ResNet101 model weights.
- **`README.md`**: Documentation for the project.

## **Features**
- **Custom Dataset Handling**: Uses `torch.utils.data.Dataset` to handle image data.
- **Data Augmentation**: Uses transforms like rotation, flipping, and color jittering.
- **ResNet101 Model**: Pretrained ResNet101 is fine-tuned for binary classification.
- **Model Training**: Uses `CrossEntropyLoss` and `AdamW` optimizer.
- **Performance Visualization**: Includes confusion matrices and accuracy charts.

## **Installation**
1. Clone the repository:
   ```bash
   git clone https://github.com/vinay23is/ic-counterfeit-detection.git
   cd ic-counterfeit-detection
