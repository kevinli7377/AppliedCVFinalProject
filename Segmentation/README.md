# Segmentation Models

This repository contains Jupyter notebooks for various segmentation models on the testing dataset. 

## Notebooks Overview

1. **SegmentAnything.ipynb**: This notebook applies Vanilla SAM on the test dataset.
2. **./grounded-sam/extended_automated_dataset_annotation_and_evaluation_with_grounding_dino_and_sam.ipynb**: This notebook applies Grounded-SAM to the same test datset.
3. **Post_SAM_Detection.ipynb**: This notebook applies the detection model (fine-tuned DEiT) to the output individual masks from Vanilla SAM.
4. **Post_Grounded_SAM_Detection.ipynb**: This notebook applies the detection model (fine-tuned DEiT) to the output individual masks from Grounded-SAM.

## Results

Based on the experiments conducted, the Grounded-SAM model demonstrated the best segmentation results, allowing for the most accurate detection.

## Links to Source Code
- Grounding Dino: https://github.com/IDEA-Research/GroundingDINO
