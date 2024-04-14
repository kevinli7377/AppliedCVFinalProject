# Fine-Tuning Pre-Trained Models on Fruits-360 Dataset

This repository contains Jupyter notebooks for fine-tuning various pre-trained models on the vanilla Fruits-360 dataset. In each notebook, we utilize the Kaggle API to download the dataset directly within Google Colab environment, enabling seamless integration of data acquisition and model training.

## Notebooks Overview

1. **Fruits360_ResNet18.ipynb**: This notebook fine-tunes a ResNet18 model on the Fruits-360 dataset.
2. **Fruits360_VGG16.ipynb**: Here, we fine-tune a VGG16 model on the same dataset.
3. **Fruits360_ViT.ipynb**: This notebook focuses on fine-tuning a Vision Transformer (ViT) model.
4. **Fruits360_DeiT.ipynb**: Lastly, we fine-tune a Data-efficient Image Transformer (DeiT) model.

## Steps in Each Notebook

1. **Data Acquisition**: We utilize the Kaggle API to download the Fruits-360 dataset directly within Google Colab.
2. **Model Loading**: In each notebook, we load one of the pre-trained models: ResNet18, VGG16, ViT, or DeiT.
3. **Fine-Tuning**: The pre-trained model is fine-tuned on the Fruits-360 dataset for 3 epochs.
4. **Training Scheduler**: A scheduler is employed to adjust learning rates during training.
5. **Validation Evaluation**: We evaluate the model's performance on the validation set in between epochs to monitor training stability.

## Results

Based on the experiments conducted, the fine-tuned DeiT model demonstrated the most stable training behavior, showing promise for our expanded dataset with additional ingredients.
