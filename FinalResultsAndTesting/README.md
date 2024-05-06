# Final Results and Testing

This repository contains the following: 
- finetuned_deit_classification_outputs: This folder contains the generated labels for individual food items indentified in the test scene images segmented using grounded-SAM. Two .txt files, one for each test dataset, can be found in the repository.
- g_sam_outputs: This repository contains folders for each test scene. Each folder contains all segments generated using grounded-SAM for that specific scene.
- FinalRecipeMatchingTesting.ipynb: Jupyter notebook containing code used to perform tests. Imports .txt files in finetuned_deit_classification_outputs and runs the recipe matching algorithm on the labels for each scene. 

Note that the code for the recipe matching algorithm is present in the above notebook. A version containing only the matching algorithm can be found in the 'Recipes and Matching' repository accessible from the root directory. The modified csv used for matching can also be found in 'Recipes and Matching.'

## References:
- Vanilla Epicurious Recipe Dataset: https://www.kaggle.com/datasets/pes12017000148/food-ingredients-and-recipe-dataset-with-images
