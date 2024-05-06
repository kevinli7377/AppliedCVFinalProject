# Ingredient Detection and Recipe Recommendation System

This repository contains all code files, notebooks, and a select number of dataset used for our Ingredient Detection and Recipe Recommendation System. This system leverages segmentation and classification models (namely a fine-tuned DeiT and a grounded-SAM model) to generate labels for ingredients in a scene image containing individual ingredients. The labels are then inputted into a recipe matching algorithm (leveraging Sentence Transformers) to output potential recipes. Below is a detailed breakdown of the repository structure and contents:

<img width="1298" alt="Project Framework 1" src="https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/4105f0bf-1d01-4f0f-87c4-2a19bc55a8b3">

<img width="2849" alt="Project Framework 2" src="https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/f94aad49-8d73-4817-8ad6-40dc6c14c498">

<img width="1780" alt="Project Framework 3" src="https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/c4369cf3-ffb1-4482-b1f6-b25cef66a80b">

<img width="2052" alt="Project Framework 4" src="https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/0aa14153-a8bb-4b09-b28e-815363cc1c20">


## Repository Structure

### Core Architecture Folders

- **Expanded Fruits-360 Detection**: This folder includes a Jupyter notebook that documents the fine-tuning of a Data-efficient Image Transformer (DeiT) model on the expanded Fruits-360 dataset. It provides insights into model adjustments and performance metrics.

- **Segmentation: Segmentation**: This directory houses Jupyter notebooks for experimenting with various segmentation models on our test dataset. The chosen model for our final architecture, along with additional processing scripts, is located in the grounded-sam folder.

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
