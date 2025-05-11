# <p align="center"> Blood Cell Analysis using Machine Learning <br> [Data Science Final Project] </p>

Classifying eight types of blood cells using image data. It covers data exploration, preprocessing, feature extraction comparison (HOG, ViT, PCA, t-SNE), model development (including DNNs, CNNs, ResNet, ViT), evaluation, and interpretability analysis.

## Live Preview & Project Access

You can access a live preview of the interactive HTML document here:

#### Via `htmlpreview.github`:

* **[Part 1](https://htmlpreview.github.io/?https://raw.githubusercontent.com/yehonatanke/Blood-Cell-Analysis-using-Machine-Learning/main/[Final_Version]_Blood_Cells_ML[Part_1].html)**
* **[Part 2](https://htmlpreview.github.io/?https://raw.githubusercontent.com/yehonatanke/Blood-Cell-Analysis-using-Machine-Learning/main/[Final_Version]_Blood_Cells_ML[Part_2].html)**

#### Via `NBViewer`:

* **[Part 1](https://nbviewer.org/github/yehonatanke/Blood-Cell-Analysis-using-Machine-Learning/blob/main/%5BFinal_Version%5D_Blood_Cells_ML%5BPart_1%5D.html)**
* **[Part 2](https://nbviewer.org/github/yehonatanke/Blood-Cell-Analysis-using-Machine-Learning/blob/main/[Final_Version]_Blood_Cells_ML[Part_2].html)**

*Note that it may take a few moments for the files to load.*

## Research Methodology
The project adopts a sequential methodology:
1. Initial data exploration and validation
2. Feature engineering (HOG vs. deep features with ViT)
3. Dimensionality reduction and feature space visualization
4. Baseline modeling with classical ML approaches
5. Deep learning with custom CNN architectures
6. Transfer learning with pre-trained models (ResNet18, ViT)
7. Model interpretability through SHAP analysis

The detailed research process, experimental notebooks, and in-depth analysis are available in the project's notebooks.

## Results
Transfer learning with robust architectures like ResNet18 and ViT proved superior to training simpler models or custom CNNs from scratch, achieving near-perfect classification accuracy by effectively learning discriminative visual patterns. The SHAP analysis confirmed that the models focused on biologically relevant features such as nuclear morphology and cell size.

## Core Project Structure

This system employs various deep learning architectures to enhance diagnostic accuracy.

#### `/src/main.py`
Entry point that coordinates all components of the blood cell classification system.

#### `/src/data/`
- **preprocessing.py**: Functions for image data processing, validation, and preparation.
- **dataset.py**: PyTorch dataset classes and data loading utilities for efficient data handling.

#### `/src/models/`
- **neural_networks.py**: Neural network architecture definitions including SimpleNN, LightCNN, CNNModel, ResNet18, and ViT implementations.
- **training.py**: Training and evaluation functions with support for early stopping and metrics tracking.

#### `/src/features/`
- **extraction.py**: Feature extraction methods including HOG and deep learning approaches using pre-trained vision transformers.

#### `/src/visualization/`
- **explorer.py**: Data exploration and visualization functions for dataset analysis and result interpretation.

#### `/src/metrics/`
- **evaluation.py**: Model evaluation metrics and performance visualization tools.

#### `/src/utils/`
- **setup.py**: Environment setup and installation utilities.
- **config.py**: Configuration management for consistent experiment parameters.

## Author 

Yehonatan Keypur

---

Grade: 100
