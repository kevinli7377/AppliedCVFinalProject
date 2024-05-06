# Final Results and Testing

This repository contains the following: 
- finetuned_deit_classification_outputs: This folder contains the generated labels for individual food items indentified in the test scene images segmented using grounded-SAM. Two .txt files, one for each test dataset, can be found in the repository.
- g_sam_outputs: This repository contains folders for each test scene. Each folder contains all segments generated using grounded-SAM for that specific scene.
- FinalRecipeMatchingTesting.ipynb: Jupyter notebook containing code used to perform tests. Imports .txt files in finetuned_deit_classification_outputs and runs the recipe matching algorithm on the labels for each scene. 

Note that the code for the recipe matching algorithm is present in the above notebook. A version containing only the matching algorithm can be found in the 'Recipes and Matching' repository accessible from the root directory. The modified csv used for matching can also be found in 'Recipes and Matching.'

## Results

The final architecture was evaluated based on the following metric: 

Accuracy =Sc/St

Sc = Number of scenes with correctly matched recipes

St = Total number of scenes 

The criterion for a correctly matched recipe: A recipe is considered correctly matched if the pre-labeled recipe for the scene is within the top N returned recipes.

All scene images were segmented using the segmentation model and subsequently classified using the fine-tuned DeiT model. Finally, the generated list labels were processed by turning the list into a set to remove duplicates and passed into the RecipeMatcher. 

**Test Batch 1:** Scenes that contained natural images of ingredients. Consist of live scenes (assembled in the “wild” on counter) and augmented scenes (from Google Photos, DALL-E).

Total number of scenes: 92
![Screenshot 2024-05-05 at 10 52 31 PM](https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/ad18f238-f41e-4f49-ac9b-c580d7c7e6e6)



**Test Batch 2**: Augmented test scenes created by splicing individual images of ingredients from the validation portion of the Fruits-360 Kaggle dataset.

Total number of scenes: 40
![Screenshot 2024-05-05 at 10 52 57 PM](https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/c8345980-da86-4cc1-9e66-fe4a10785e72)


## References:
- Vanilla Epicurious Recipe Dataset: https://www.kaggle.com/datasets/pes12017000148/food-ingredients-and-recipe-dataset-with-images
