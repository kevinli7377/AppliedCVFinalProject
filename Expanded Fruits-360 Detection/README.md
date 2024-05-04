# Fine-Tuned DeiT on Expanded Fruits-360 Dataset

This repository contains a Jupyter notebook documenting the fine-tuning process of a Data-efficient Image Transformer (DeiT) model on the expanded Fruits-360 dataset. The expanded dataset includes the original 131 classes from the vanilla Fruits-360 dataset along with an additional 12 classes:

1. Beef 🥩
2. Butter 🧈
3. Chicken 🍗
4. Egg 🥚
5. Eggs 🥚
6. Flour 🍞
7. Lamb 🐑
8. Milk 🥛
9. Pasta 🍝
10. Pork 🐖
11. Rice 🍚
12. Salmon 🐟

## Notebook Overview

- **Expanded_Fruits_360_DeiT.ipynb**: This notebook details the fine-tuning procedure of the DeiT model on the expanded Fruits-360 dataset.

## Steps in the Notebook

1. **Data Acquisition**: The expanded Fruits-360 dataset, including the new classes, is obtained and prepared for training.
2. **Model Loading**: The DeiT pre-trained model is loaded for fine-tuning.
3. **Fine-Tuning**: The DeiT model is fine-tuned on the expanded Fruits-360 dataset, considering the additional classes, for a specified number of epochs.
4. **Training Scheduler**: A scheduler is utilized to dynamically adjust learning rates during training.
5. **Validation and Evaluation**: The fine-tuned DeiT model's performance is evaluated on the validation set, providing insights into its effectiveness in recognizing the expanded range of fruit and non-fruit classes.

## Results and Insights

The fine-tuned DeiT model exhibits robust performance on the expanded Fruits-360 dataset, showcasing its capability to generalize across a diverse range of classes. Through experimentation, insights into the model's behavior and its ability to accurately classify fruits and other food items are gained.

## Best Model Weights
If you want to work with the best DeiT model's weights, the .pth file is available here: https://drive.google.com/file/d/1--KUyiK6GICBemEnD7ItEMDESg8C7KkO/view?usp=sharing


Happy fine-tuning and classifying! 🥩🧈🍗🥚🥚🍞🐑🥛🍝🐖🍚🐟
