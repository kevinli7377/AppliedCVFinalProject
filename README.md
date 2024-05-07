# Ingredient Detection and Recipe Recommendation System

This repository contains all code files, notebooks, and a select number of dataset used for our Ingredient Detection and Recipe Recommendation System. This system leverages segmentation and classification models (namely a fine-tuned DeiT and a grounded-SAM model) to generate labels for ingredients in a scene image containing individual ingredients. The labels are then inputted into a recipe matching algorithm (leveraging Sentence Transformers) to output potential recipes. Below is a detailed breakdown of the repository structure and contents:

![Project Framework](https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/631d5ae9-6692-4bf6-892c-ed997391c225)
![Project Framework 2](https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/966561b6-f790-4f74-acc0-ec421626ada1)

## Repository Structure

### Core Architecture Folders

- **Expanded Fruits-360 Detection**: This folder includes a Jupyter notebook that documents the fine-tuning of a Data-efficient Image Transformer (DeiT) model on the expanded Fruits-360 dataset. It provides insights into model adjustments and performance metrics.

- **Segmentation**: This directory houses Jupyter notebooks for experimenting with various segmentation models on our test dataset. The chosen model for our final architecture, along with additional processing scripts, is located in the grounded-sam folder.

- **Recipes and Matching**: This folder contains CSV files for both original and modified recipe datasets, along with a Jupyter notebook that features classes 'RecipeCSVParser' and 'RecipeSearcher,' integral to the recipe recommendation functionality of our system. 

- **FinalResultsAndTesting**: Contains notebooks for analyzing the outputs from the fine-tuned DeiT model. This folder also includes results from the 'Grounded-SAM' segmentation model and integrated outputs necessary for the final testing and result demonstration.

### Experimental and Dataset Preparation Folders

- **CLIP**: Includes notebooks that test the CLIP model on the extended Fruits-360 dataset and additional datasets, exploring its capabilities and limitations in ingredient detection.
- **Fruits-360 Detection Experiments**: Contains notebooks focused on fine-tuning various pre-trained models on the vanilla Fruits-360 dataset, detailing experiments and findings.
- **dataset_preparation_code**: This folder contains a collection of notebooks used for preparing image datasets. These include scripts for Google Image Scraping, JSON file creation, and training/test data splitting.

## Links to Datasets:

- Extended-fruits-360 Dataset: https://drive.google.com/drive/folders/1MPE5mmMRz5GdFZicR0Ep4Cg9CF24c3yx?usp=sharing
- Test Batch 1: https://drive.google.com/drive/folders/1VqU8GrjYOhxsaUCuLiXNZh6iTUnG5mRA?usp=share_link
- Test Batch 2: https://drive.google.com/drive/folders/1meIHyuWd2kGOChNONTshH6FeOW9HFitU?usp=share_link
- Vanilla fruits-360 Kaggle Dataset: https://www.kaggle.com/datasets/moltean/fruits
- Vanilla Epicurious Recipe Dataset: https://www.kaggle.com/datasets/pes12017000148/food-ingredients-and-recipe-dataset-with-images
