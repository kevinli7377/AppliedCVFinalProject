# Recipe and Matching Algorithm

This repository contains the original and modified recipe dataset CSVs. Additionally, this repository also contains a Jupyter notebook containing two classes, RecipeCSVParser and RecipeSearcher, both used in the final architecture of the ingredient detection and recipe matching model.

![Project Framework 3](https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/ceb977c0-2792-46cd-9304-62852da085ba)
![Project Framework 4](https://github.com/kevinli7377/AppliedCVFinalProject/assets/56395320/f663b965-c621-4ee2-8cd5-ca18ef6dec8f)

## Notebook Overview

- **RecipeMatchingFinal.ipynb**: This notebook contains two classses, RecipeCSVParser and RecipeSearcher. This notebook is a finalized version of all code used in 'RecipeMatchingWorking.ipynb,' a working notebook that can be found in 'Testing Code.'

## Notebook Explanation

1. **RecipeCSVParser**: This class contains all functions used to parse the original recipe CSV file. It utilizes NTLK and Re modules to remove stopwords, numbers, and punctuation from the original recipe ingredients lists. After removing redundant words, the ingredients are sorted in alphabetical order. This sorting standardizes the structure of the ingredients lists, facilitating more consistent and effective comparison and matching of subsequently generated embeddings. Sentences are then construcgted in the form 'A recipe containing...' for each cleaned list. Sentence transformers were then used to create embeddings for each of the constructed sentences. All clean ingredients lists, sentences, and embeddings were appended as an additional column to the original CSV. The modified CSV (Epicurious_Processed_Recipes_With_Embedding_alphabetical.csv) should be used with the RecipeSearcher to query recipes.

2. **RecipeSearcher**: This class contains functions for querying recipes from the database. The hybrid matching algorithm first uses sentence similarity to narrow down the scope of candidate recipes before matching ingredients with a brute-force method.

## Comments

- Many ingredient lists include adjectives (e.g., 'shortgrain rice'), which are challenging to remove without manually cleaning all data entries. Nevertheless, the RecipeCSVParser effectively eliminates most redundant text and successfully maps queries to appropriate recipes.
- Recipes in the 'Food Ingreidents and Recipes Dataset with Images' dataset are from Epicurious and contain many additional ingredients untrained on the detection models.
- Existing solutions utilizing Word2Vec were consulted and tested on the recipe dataset. Unfortunately, results were rather poor. The Sentence Transformers better capture context and produce better results based on preliminary tests.
- The original images accompanying the dataset can be found at the link below. 

## References

https://www.kaggle.com/datasets/pes12017000148/food-ingredients-and-recipe-dataset-with-images
