# Unleashing the Potential of Synthetic Images: Histopathology Image Classification

Welcome to the repository for the dataset used in the paper titled **"Unleashing the Potential of Synthetic Images: A Study on Histopathology Image Classification"**. 

The dataset can be downloaded  [here](https://zenodo.org/records/13928371).

Please find the preprint link [here](https://arxiv.org/abs/2409.16002)

## Overview

This repository hosts synthetic histopathology images generated for research purposes. The dataset includes synthetic histopathology images and the subsets of real images employed to train the generative models. 

It is intended for use in exploring and evaluating histopathology image classification methods.

## Dataset structure

The dataset is organized into real and synthetic folders. 

The real/ folder contains .pt files, each representing a subset of the real images used to train the generative models.

The synthetic/ folder is structured by generative model type (e.g., DiT, GAN, U_Net) and further subdivided into categories based on the image selection approach:
  - Class_based_rs/: the realism score is calculated per class.
  - None/: all the synthetic images are used.
  - Realism_score/: images with R ≥ 1 are selected.

Each category contains subsets corresponding to different partitions.

<pre>
dataset
├── real/
│   ├── subset_1.pt
│   ├── subset_2.pt
│   ├── subset_3.pt
│   ├── subset_4.pt
│   └── subset_5.pt
└── sinthetic/
    ├── DiT
    │   ├── Class_based_rs/
    │   │   ├── Subset_1/
    │   │   ├── Subset_2/
    │   │   ├── Subset_3/
    │   │   ├── Subset_4/
    │   │   └── Subset_5/
    │   ├── None/
    │   │   ├── Subset_1/
    │   │   ├── Subset_2/
    │   │   ├── Subset_3/
    │   │   ├── Subset_4/
    │   │   └── Subset_5/
    │   └── Realism_score/
    │   │   ├── Subset_1/
    │   │   ├── Subset_2/
    │   │   ├── Subset_3/
    │   │   ├── Subset_4/
    │   │   └── Subset_5/
    ├── GAN
    │   ├── Class_based_rs/
    │   │   ├── Subset_1/
    │   │   ├── Subset_2/
    │   │   ├── Subset_3/
    │   │   ├── Subset_4/
    │   │   ├── Subset_1/
    │   │   ├── Subset_2/
    │   │   ├── Subset_3/
    │   │   ├── Subset_4/
    │   │   └── Subset_5/
    │   └── Realism_score/
    │   │   ├── Subset_1/
    │   │   ├── Subset_2/
    │   │   ├── Subset_3/
    │   │   ├── Subset_4/
    │   │   └── Subset_5/
    └── U_Net
        ├── Class_based_rs/
        │   ├── Subset_1/
        │   ├── Subset_2/
        │   ├── Subset_3/
        │   ├── Subset_4/
        │   └── Subset_5/
        ├── None/
        │   ├── Subset_1/
        │   ├── Subset_2/
        │   ├── Subset_3/
        │   ├── Subset_4/
        │   └── Subset_5/
        └── Realism_score/
            ├── Subset_1/
            ├── Subset_2/
            ├── Subset_3/
            ├── Subset_4/
            └── Subset_5/

</pre>

## Original Dataset Reference

The synthetic images in this repository were generated using the [PCam dataset](https://github.com/basveeling/pcam). Please refer to the original dataset for more details.
    
## Citations
<pre>
 @misc{benitodelvalle2024unleashingpotentialsyntheticimages,
      title={Unleashing the Potential of Synthetic Images: A Study on Histopathology Image Classification}, 
      author={Leire Benito-Del-Valle and Aitor Alvarez-Gila and Itziar Eguskiza and Cristina L. Saratxaga},
      journal={arXiv:2409.16002},
      year={2024}
}
</pre>

## Contact
For problems and questions not fit for a github issue, please email [Leire Benito del Valle](mailto:leire.benitodelvalle@tecnalia.com).




