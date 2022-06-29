# Capstone
A Capstone project investigating the influence of Post-Impressionism in Modern Art. 

# Goals
This repository contains the accompanying code to a Capstone final thesis project that seeks to use deep learning methods to investigate the influence of Post-Impressionism on subsequent movements in Modern Art. 

# Dataset and Project 
The code is based on a subset of the WikiArt dataset. These were sourced from cs-chan's ARTGAN repository. The folders of paintings from the relevant movement were then extracted into a smaller data file. This smaller dataset consists of paintings from the following movements: (1) Post-Impressionism, (2) Fauvism, (3) Expressionism, (4) Cubism, (5) Abstract Expressionism, (6) Pop Art.

# Project Details
After initial preprocessing of the dataset, a VGG16 model is cut to the flatten layer to remove the fully-connected layers and leave only the convolutional layers. This model architecture is then used to extract visual features from paintings in each movement. The extracted features are linked to both movement labels and their original filenames (for visualization purposes). The extent of the visual similarity is calculated using three distance measures applied between feature vectors: cosine distance, correlation distance, and Euclidean distance. The resulting distances of paintings of later movements from Post-Impressionism is then visualied using histogram plots and density plots. The paintings at the extremes of the histogram distributions for each movement are also visualized in order to observe key visual features of the most similar and most different paintings to Post-Impressionism for each subsequent movement.

