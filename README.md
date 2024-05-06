# Ingredient Detection and Recipe Recommendation System

This repository contains all code files that were used as part of the designed system. A breakdown of the repository is as follows:

Folders containing files used for the final architecture:

- Expanded Fruits-360 Detection: Contains a Jupyter notebook documenting the fine-tuning process of a Data-efficient Image Transformer (DeiT) model on the expanded Fruits-360 dataset.

- Segmentation: Contains Jupyter notebooks for various segmentation models on the testing dataset. The final segmentation model and additional processing code used in the combined model can be found in the 'grounded-sam' folder.

- Recipes and Matching: Contains original and modified recipe dataset CSVs, as well as a Jupyter notebook containing two classes, RecipeCSVParser and RecipeSearcher, both used in the final architecture.

- FinalResultsAndTesting: Contains Jupyter notebook to process fine-tuned DeiT classification outputs. Grounded-SAM outputted segments and DeiT outputs can also be found in this folder.

Additional folders containing experimental code and dataset preparation:

- CLIP: Contains notebooks used to test CLIP on extended-fruits-360 and additional datasets.
- Fruits-360 Detection Experiments: Contains Jupyter notebooks for fine-tuning various pre-trained models on the vanilla Fruits-360 dataset.
- dataset_preparation_code: Contains various notebooks used for image dataset preparation, including GoogleImageScraping, json_creation, and Training_Test_Split.
